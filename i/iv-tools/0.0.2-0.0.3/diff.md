# Comparing `tmp/iv_tools-0.0.2.tar.gz` & `tmp/iv_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iv_tools-0.0.2.tar", last modified: Thu Jul 13 08:51:24 2023, max compression
+gzip compressed data, was "iv_tools-0.0.3.tar", last modified: Fri Jul 14 05:23:55 2023, max compression
```

## Comparing `iv_tools-0.0.2.tar` & `iv_tools-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 08:51:24.836063 iv_tools-0.0.2/
--rw-rw-rw-   0        0        0      511 2023-07-13 08:51:24.835066 iv_tools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       73 2023-07-13 08:22:18.000000 iv_tools-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 08:51:24.825093 iv_tools-0.0.2/iv_tools/
--rw-rw-rw-   0        0        0      116 2023-07-12 14:35:18.000000 iv_tools-0.0.2/iv_tools/__init__.py
--rw-rw-rw-   0        0        0    20652 2023-07-13 08:17:54.000000 iv_tools-0.0.2/iv_tools/iv_tools.py
-drwxrwxrwx   0        0        0        0 2023-07-13 08:51:24.834070 iv_tools-0.0.2/iv_tools.egg-info/
--rw-rw-rw-   0        0        0      511 2023-07-13 08:51:24.000000 iv_tools-0.0.2/iv_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-07-13 08:51:24.000000 iv_tools-0.0.2/iv_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 08:51:24.000000 iv_tools-0.0.2/iv_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 08:51:24.000000 iv_tools-0.0.2/iv_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 08:51:24.836063 iv_tools-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-07-13 08:51:13.000000 iv_tools-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:23:55.579843 iv_tools-0.0.3/
+-rw-rw-rw-   0        0        0      511 2023-07-14 05:23:55.578846 iv_tools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-07-13 08:22:18.000000 iv_tools-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 05:23:55.565879 iv_tools-0.0.3/iv_tools/
+-rw-rw-rw-   0        0        0      116 2023-07-12 14:35:18.000000 iv_tools-0.0.3/iv_tools/__init__.py
+-rw-rw-rw-   0        0        0    26710 2023-07-14 05:19:54.000000 iv_tools-0.0.3/iv_tools/iv_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:23:55.577850 iv_tools-0.0.3/iv_tools.egg-info/
+-rw-rw-rw-   0        0        0      511 2023-07-14 05:23:55.000000 iv_tools-0.0.3/iv_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-14 05:23:55.000000 iv_tools-0.0.3/iv_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 05:23:55.000000 iv_tools-0.0.3/iv_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 05:23:55.000000 iv_tools-0.0.3/iv_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 05:23:55.579843 iv_tools-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-07-14 05:20:58.000000 iv_tools-0.0.3/setup.py
```

### Comparing `iv_tools-0.0.2/iv_tools/iv_tools.py` & `iv_tools-0.0.3/iv_tools/iv_tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -111,14 +111,32 @@
                     final_strike = next_strike
                     final_price = next_price['SETTLE_PR'].sum()
                     break
          
 
         return final_price
 
+
+def match_delta(opt_bhav, expiry_date_str, opt_delta, dte, fut, opt_type = 'p'):
+    opt_type = (opt_type+'e').upper()
+    final_price = np.nan
+    
+    temp = opt_bhav[(opt_bhav['EXPIRY_DT']==expiry_date_str)&(opt_bhav['OPTION_TYP'] == opt_type)]
+    if opt_type == 'PE':
+        temp = temp[temp['STRIKE_PR']<=1.01*fut]
+    else:
+        temp = temp[temp['STRIKE_PR']>=0.99*fut]
+        
+    temp['IV'] = temp.apply(lambda x: implied_vol(fut, x['STRIKE_PR'], dte/365, 0.07, x['SETTLE_PR'], flag = opt_type[0].lower()), axis = 1)
+    temp['DELTA']= abs(temp.apply(lambda x: delta(opt_type[0].lower(), fut, x['STRIKE_PR'], dte/365, 0.07, x['IV']), axis = 1))
+    
+    temp['DELTA_DIFF'] = abs(temp['DELTA'] - opt_delta)
+    iv = temp.set_index('STRIKE_PR').sort_values('DELTA_DIFF').iloc[0]['IV']
+    return iv
+
 def interpolate_iv(term, dte_near, dte_far, iv_near, iv_far):
     """
     Uses the interpolation formula used in the VIX white paper    
 
     Parameters
     ----------
     term : INT
@@ -145,15 +163,15 @@
 
     iv = np.sqrt((((tte_near*(iv_near**2))*((tte_far - tte_term)/(tte_far - tte_near)))+((tte_far*(iv_far**2))*((tte_term - tte_near)/(tte_far - tte_near))))*(365/term))
     return iv
 
 
 
 
-def retrieve_iv(symbol, date, index = True, method = 'straddle', front_back = 'interpolate', next_contract_skip = 1, interpolate_term = 5, index_opt = 'weekly'):
+def retrieve_atm_iv(symbol, date, index = True, method = 'straddle', front_back = 'interpolate', next_contract_skip = 1, interpolate_term = 5, index_opt = 'weekly'):
     call_put_dict = {'put': 'p', 'call': 'c'}
     final_iv = np.nan
     try:
         date_str  = date.strftime('%Y-%m-%d')
         bhav = pd.read_csv(rf'C:\Users\varun\Documents\Raw Data\Bhavcopies\Bhavcopy_fno_{date_str}.csv')
         bhav = bhav[bhav['SYMBOL']==symbol]
         
@@ -239,14 +257,17 @@
                 back_expiry_date = dt.datetime.strptime(back_expiry_date_str, '%Y-%m-%d')
                 back_dte = (back_expiry_date - date).days
                 back_fut = fut_bhav['SETTLE_PR'].iloc[2]
                 
                 if ((index) & (index_opt == 'weekly')):
                     back_expiry_date_str = weekly_expiry_dates_str.iloc[2]
                     back_expiry_date = weekly_expiry_dates.iloc[2]
+                    back_dte = (back_expiry_date - date).days
+                    back_fut = find_synthetic_forward(symbol, opt_bhav, back_fut, back_expiry_date_str, back_dte)
+                            
                 
             strike_list = pd.Series(opt_bhav[opt_bhav['EXPIRY_DT']==back_expiry_date_str]['STRIKE_PR'].unique())
             back_strike_diff = abs(strike_list - back_fut) # finding the closest strikes to the forward
             back_strike_diff.index = strike_list
             back_closest_strike = back_strike_diff[back_strike_diff == back_strike_diff.min()].index[0]
             
             if method == 'straddle':
@@ -369,7 +390,108 @@
                 
                 final_iv = (interpolated_straddle_iv + interpolated_call_iv + interpolated_put_iv)/3
                 
             return final_iv
     except Exception as e:
         return final_iv
         print(f'error {e} for {date} for {symbol}')
+
+
+
+def retrieve_otm_iv(symbol, date, opt_delta = 0.25, index = True, front_back = 'interpolate', next_contract_skip = 1, interpolate_term = 5, index_opt = 'weekly', opt_type = 'p'):
+
+    call_put_dict = {'put': 'p', 'call': 'c'}
+    final_iv = np.nan
+    try:
+        date_str  = date.strftime('%Y-%m-%d')
+        bhav = pd.read_csv(rf'C:\Users\varun\Documents\Raw Data\Bhavcopies\Bhavcopy_fno_{date_str}.csv')
+        bhav = bhav[bhav['SYMBOL']==symbol]
+        
+        if index:   # filtering depending on index or single stock   
+            fut_bhav = bhav[bhav['INSTRUMENT']=='FUTIDX']
+            opt_bhav = bhav[bhav['INSTRUMENT']=='OPTIDX']
+            
+            weekly_expiry_dates_str = pd.Series(opt_bhav['EXPIRY_DT'].unique()).sort_values()
+            weekly_expiry_dates= weekly_expiry_dates_str.apply(lambda x: dt.datetime.strptime(x, '%Y-%m-%d'))
+            monthly_expiry_dates_str = pd.Series(fut_bhav['EXPIRY_DT'].unique()).sort_values()
+            monthly_expiry_dates = monthly_expiry_dates_str.apply(lambda x: dt.datetime.strptime(x, '%Y-%m-%d'))
+            
+        else:
+            fut_bhav = bhav[bhav['INSTRUMENT']=='FUTSTK']
+            opt_bhav = bhav[bhav['INSTRUMENT']=='OPTSTK']
+                    
+
+        front_fut = fut_bhav['SETTLE_PR'].iloc[0]
+        back_fut = fut_bhav['SETTLE_PR'].iloc[1]
+        
+        
+        front_expiry_date_str = fut_bhav['EXPIRY_DT'].iloc[0]
+        front_expiry_date = dt.datetime.strptime(front_expiry_date_str, '%Y-%m-%d')
+        back_expiry_date_str = fut_bhav['EXPIRY_DT'].iloc[1]
+        back_expiry_date = dt.datetime.strptime(back_expiry_date_str, '%Y-%m-%d')
+                            
+        front_dte = (front_expiry_date - date).days
+        back_dte = (back_expiry_date - date).days
+        
+        # modifications for index options
+        
+        if ((index) & (index_opt == 'weekly')):
+            front_expiry_date_str = weekly_expiry_dates_str.iloc[0]
+            front_expiry_date = weekly_expiry_dates.iloc[0]
+            back_expiry_date_str = weekly_expiry_dates_str.iloc[1]
+            back_expiry_date = weekly_expiry_dates.iloc[1]
+                                
+            front_dte = (front_expiry_date - date).days
+            back_dte = (back_expiry_date - date).days
+            
+            front_fut = find_synthetic_forward(symbol, opt_bhav, front_fut, front_expiry_date_str, front_dte)
+            back_fut = find_synthetic_forward(symbol, opt_bhav, front_fut, back_expiry_date_str, back_dte)
+                    
+    
+                  
+        if front_back == 'front':
+            if front_dte <= next_contract_skip: # This is rolling to the next contract
+                front_expiry_date_str = back_expiry_date_str
+                front_expiry_date = back_expiry_date
+                front_dte = back_dte
+                front_fut = back_fut
+                
+            final_iv = match_delta(opt_bhav, front_expiry_date_str, opt_delta, front_dte, front_fut, opt_type = opt_type)
+            return final_iv
+        
+        elif front_back == 'back':
+            if back_dte <= next_contract_skip: # This is rolling to the next contract
+                back_expiry_date_str = fut_bhav['EXPIRY_DT'].iloc[2]
+                back_expiry_date = dt.datetime.strptime(back_expiry_date_str, '%Y-%m-%d')
+                back_dte = (back_expiry_date - date).days
+                back_fut = fut_bhav['SETTLE_PR'].iloc[2]
+                  
+                if ((index) & (index_opt == 'weekly')):
+                    back_expiry_date_str = weekly_expiry_dates_str.iloc[2]
+                    back_expiry_date = weekly_expiry_dates.iloc[2]
+                     
+                    back_dte = (back_expiry_date - date).days
+                    back_fut = find_synthetic_forward(symbol, opt_bhav, back_fut, back_expiry_date_str, back_dte)
+                     
+                           
+            final_iv = match_delta(opt_bhav, back_expiry_date_str, opt_delta, back_dte, back_fut, opt_type = opt_type)
+            return final_iv
+          
+        else: # when front_back == 'interpolate'
+
+            if front_dte > 0:
+                front_iv = match_delta(opt_bhav, front_expiry_date_str, opt_delta, front_dte, front_fut, opt_type = opt_type)
+                back_iv = match_delta(opt_bhav, back_expiry_date_str, opt_delta, back_dte, back_fut, opt_type = opt_type)
+             
+                if back_iv != np.nan:
+                    final_iv = interpolate_iv(interpolate_term, front_dte, back_dte, front_iv, back_iv)
+                else:
+                    final_iv = front_iv
+            
+            else:
+                final_iv = match_delta(opt_bhav, back_expiry_date_str, opt_delta, back_dte, back_fut, opt_type = opt_type)
+            
+            return final_iv 
+        
+    except Exception as e:
+        return final_iv
+        print(f'error {e} for {date} for {symbol}')
```

### Comparing `iv_tools-0.0.2/setup.py` & `iv_tools-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @author: varun
 """
 
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'IV Tools'
 LONG_DESCRIPTION = 'Implied Volatility Tools'
 
 # Setting up
 setup(
     name="iv_tools",
     version=VERSION,
```

