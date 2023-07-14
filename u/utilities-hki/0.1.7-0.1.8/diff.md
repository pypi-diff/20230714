# Comparing `tmp/utilities_hki-0.1.7.tar.gz` & `tmp/utilities_hki-0.1.8.tar.gz`

## Comparing `utilities_hki-0.1.7.tar` & `utilities_hki-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/requirements.txt
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/__init__.py
--rwxr-xr-x   0        0        0    71817 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/analy_utils.py
--rwxr-xr-x   0        0        0     2729 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/db_utils.py
--rwxr-xr-x   0        0        0     2944 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/email_utils.py
--rwxr-xr-x   0        0        0     5268 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/fb_utils.py
--rwxr-xr-x   0        0        0   142582 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/data/gmm_2022-10-23.joblib
--rwxr-xr-x   0        0        0    36982 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/data/gmm_2023-04-02.joblib
--rwxr-xr-x   0        0        0     1743 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib
--rwxr-xr-x   0        0        0     1423 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/.gitignore
--rwxr-xr-x   0        0        0    34522 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/LICENSE.txt
--rwxr-xr-x   0        0        0     4424 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/README.md
--rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/PKG-INFO
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/.gitignore
+-rwxr-xr-x   0        0        0    35182 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/LICENSE.txt
+-rwxr-xr-x   0        0        0     4496 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/README.md
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/pyproject.toml
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/requirements.txt
+-rwxr-xr-x   0        0        0   142321 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/dist/utilities_hki-0.1.3-py3-none-any.whl
+-rwxr-xr-x   0        0        0   140729 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/dist/utilities_hki-0.1.3.tar.gz
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/__init__.py
+-rwxr-xr-x   0        0        0    73470 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/analy_utils.py
+-rwxr-xr-x   0        0        0     2839 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/db_utils.py
+-rwxr-xr-x   0        0        0     4978 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/email_utils.py
+-rwxr-xr-x   0        0        0     5420 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/fb_utils.py
+-rwxr-xr-x   0        0        0     1344 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/test.py
+-rwxr-xr-x   0        0        0   142582 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/data/gmm_2022-10-23.joblib
+-rwxr-xr-x   0        0        0    36982 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/data/gmm_2023-04-02.joblib
+-rwxr-xr-x   0        0        0     1743 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib
+-rwxr-xr-x   0        0        0     1423 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 utilities_hki-0.1.8/PKG-INFO
```

### Comparing `utilities_hki-0.1.7/src/utilities_hki/analy_utils.py` & `utilities_hki-0.1.8/src/utilities_hki/analy_utils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,1653 +1,1653 @@
-"""
-Analysis utility functions.
-Copyright (C) 2022 Humankind Investments.
-"""
-
-import os, sys
-from joblib import load
-import pathlib
-import re
-
-from datetime import datetime
-import calendar
-import pytz
-eastern = pytz.timezone('US/Eastern')
-
-import requests
-from bs4 import BeautifulSoup
-import json
-
-import pandas as pd
-import numpy as np
-
-from .db_utils import database_connect
-
-
-# CLEANING DUPLICATE AND SPLIT VISITS +++++++++++++++++++++++++++++++++++++++++++++++++++++++
-def drop_false_splits(df):
-    """
-    Drop false splits.
-    
-    Drop extraneous false splits, i.e. visits with duplicate visit counts per visitor
-    occurring more than thirty minutes from each other. For each set of false splits, 
-    the visit with the most activity is kept.
-    
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Dataframe of false splits.
-        
-    Returns
-    -------
-    pd.DataFrame
-        Dataframe of remaining splits after drops.
-    """
-    
-    # keep visit among false splits with longest visit duration or most actions
-    cdf = df.sort_values(by=['visit_duration', 'actions'],
-                         ascending=[False, False]).drop_duplicates(
-                             subset=['visitor_id', 'visit_count']).reset_index(drop=True)
-    
-    return cdf
-
-
-def combine_true_splits(df, dt0=True):
-    """
-    Combine true splits.
-    
-    Combine and return true split visits, i.e. visits with duplicate visit counts 
-    per visitor occurring within thirty minutes of one another.
-    
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Dataframe of true splits.
-    dt0 : bool
-        Whether delta-dt between visits is 0, indicating split visits occur at same time.
-        
-    Returns
-    -------
-    pd.DataFrame
-        Dataframe of combined splits.
-    """
-    
-    # separate columns by how data to be aggregated
-    mean_cols = [col for col in df.columns if col.split('_')[0] == 'avg']
-    sum_cols = [col for col in df.columns if col.split('_')[-1] in [
-        'actions', 'pages', 'downloads', 'outlinks', 'buyetfs', 'brokerlinks', 
-        'plays', 'pauses', 'resumes', 'seeks', 'finishes', 
-        'time', 'submissions', 'duration'] and col != 'time' and col not in mean_cols]
-    first_cols = [col for col in df.columns if col not in
-                  mean_cols + sum_cols and col.split('_')[0] not in [
-                      'first', 'last', 'entry', 'exit'] and col.split('_')[-1] not in [
-                          'flow', 'ts', 'list'] and not col.endswith('video_resolution')]
-    manual_cols = [col for col in df.columns if col not in sum_cols + mean_cols + first_cols]
-
-    # convert numeric columns to proper type
-    df[mean_cols] = df[mean_cols].astype(float)
-    
-    # combine split visits with same visitor id and visit count
-    # --> sort by visit id for split visits occurring at same time; split by datetime otherwise
-    sort_col = 'visit_id' if dt0 else 'datetime'
-    grp_cols = ['visitor_id', 'visit_count']
-    # --> also group by datetime for split visits occurring at same time
-    if dt0: grp_cols.append('datetime')
-    grp = df.sort_values(by=sort_col).groupby(grp_cols)
-    
-    # apply basic aggregates for appropriate columns (first/last, sum, mean)
-    first_grp = grp[[col for col in first_cols if col not in grp.keys]]
-    # --> pull basic visit info from last visit info in half hour window if delta-t != 0
-    first_df = first_grp.first() if dt0 else first_grp.last()
-    sum_df = grp[[col for col in sum_cols if col not in grp.keys]].sum()
-    mean_df = grp[[col for col in mean_cols if col not in grp.keys]].mean()
-    cdf = pd.concat([first_df, sum_df, mean_df], axis=1)
-
-    # combine remaining columns manually ...
-    
-    # select first and last non-empty action, and combine non-empty action flows in order
-    actgrp = df[df['first_action'] != 'None'].sort_values(by=sort_col).groupby(
-        grp_cols, group_keys=False)
-    acts_df = pd.concat([actgrp['first_action'].first(), 
-                         actgrp['last_action'].last(),
-                         actgrp['action_flow'].apply(lambda x: ','.join(x)),
-                         actgrp['action_ts'].apply(lambda x: ','.join(x)),
-                         actgrp['action_site_flow'].apply(lambda x: ','.join(x)), 
-                         actgrp['action_path_flow'].apply(lambda x: ','.join(x))], axis=1)
-    
-    # select first/last entry/exit pages, and fill in missing values based on first/last actions
-    pgs_df = pd.concat([actgrp['entry_page'].first(), actgrp['exit_page'].last()], axis=1)
-    pgs_df.loc[(pgs_df['entry_page'] == 'None') &
-               (acts_df['first_action'].str.rsplit('_', n=1).str[0].isin(
-                   ['humankind_video', 'humankind-short_video', 'getstarted_form'])),
-               'entry_page'] = 'humankind'
-    pgs_df.loc[(pgs_df['entry_page'] == 'None') &
-               ((acts_df['first_action'].str.rsplit('_', n=1).str[0].isin(
-                   ['wtf_video', 'wtf-short_video', 'buyetf'])) |
-                (acts_df['first_action'].str.split('_', n=1).str[-1].isin(
-                    ['brokerlink_click', 'download']))), 'entry_page'] = 'humankindfunds'
-    pgs_df.loc[(pgs_df['exit_page'] == 'None') &
-               (acts_df['last_action'].str.rsplit('_', n=1).str[0].isin(
-                   ['humankind_video', 'humankind-short_video', 'getstarted_form'])),
-               'exit_page'] = 'humankind'
-    pgs_df.loc[(pgs_df['exit_page'] == 'None') &
-               ((acts_df['last_action'].str.rsplit('_', n=1).str[0].isin(
-                   ['wtf_video', 'wtf-short_video', 'buyetf'])) |
-                (acts_df['last_action'].str.split('_', n=1).str[-1].isin(
-                    ['brokerlink_click', 'download']))), 'exit_page'] = 'humankindfunds'
-
-    # combine non-empty page flows
-    pggrp = df[df['page_flow'] != 'None'].sort_values(by=sort_col).groupby(
-        grp_cols, group_keys=False)
-    pgs_df = pd.concat([
-        pgs_df, pggrp['page_flow'].apply(lambda x: ','.join(x)), 
-        pggrp['page_ts'].apply(lambda x: ','.join(x))], axis=1).fillna('None')
-    
-    # combine non-empty article post and ranked company page lists
-    for pg in ['article-post', 'ranked-company']:
-        pg += '_page_list'
-        pgs_df = pd.concat([pgs_df, df[df[pg].fillna('None').replace(
-            'NaN', 'None') != 'None'].sort_values(by=sort_col).groupby(
-                grp_cols, group_keys=False)[pg].apply(
-                    lambda x: ','.join(x))], axis=1).fillna('None')
-        
-    # combine non-empty download flows
-    dlgrp = df[df['download_flow'] != 'None'].sort_values(by=sort_col).groupby(
-        grp_cols, group_keys=False)
-    dls_df = pd.concat([
-        dlgrp['download_flow'].apply(lambda x: ','.join(x)), 
-        dlgrp['download_ts'].apply(lambda x: ','.join(x))], axis=1).fillna('None')
-    
-    # combine non-empty outlink flows
-    olgrp = df[df['outlink_flow'] != 'None'].sort_values(by=sort_col).groupby(
-        grp_cols, group_keys=False)
-    ols_df = pd.concat([
-        olgrp['outlink_flow'].apply(lambda x: ','.join(x)), 
-        olgrp['outlink_ts'].apply(lambda x: ','.join(x))], axis=1).fillna('None')
-
-    # combine non-empty outlink lists
-    for ol in ['social', 'crs', 'disclosures', 'articles']:
-        ol += '_outlink_list'
-        ols_df = pd.concat([ols_df, df[df[ol].fillna('None').replace(
-            'NaN', 'None') != 'None'].sort_values(by=sort_col).groupby(
-                grp_cols, group_keys=False)[ol].apply(
-                    lambda x: ','.join(x))], axis=1).fillna('None')
-           
-    # combine non-empty buy-etf timestamps
-    etfs_df = df[df['buyetf_ts'].fillna('None').replace(
-        'NaN', 'None') != 'None'].sort_values(by=sort_col).groupby(
-            grp_cols, group_keys=False)['buyetf_ts'].apply(lambda x: ','.join(x))
-    
-    # combine non-empty broker link flows
-    brkgrp = df[df['brokerlink_flow'] != 'None'].sort_values(by=sort_col).groupby(
-        grp_cols, group_keys=False)
-    brks_df = pd.concat([
-        brkgrp['brokerlink_flow'].apply(lambda x: ','.join(x)), 
-        brkgrp['brokerlink_ts'].apply(lambda x: ','.join(x))], axis=1).fillna('None')
-    
-    # combine non-empty video flows and non-empty video resolutions
-    vidgrp = df[df['video_action_flow'] != 'None'].sort_values(by=sort_col).groupby(
-        grp_cols, group_keys=False)
-    vids_df = pd.concat([
-        vidgrp['video_action_flow'].apply(lambda x: ','.join(x)), 
-        vidgrp['video_action_ts'].apply(lambda x: ','.join(x))], axis=1).fillna('None')
-
-    # combine non-empty form flows
-    frmgrp = df[df['form_action_flow'] != 'None'].sort_values(by=sort_col).groupby(
-        grp_cols, group_keys=False)
-    frms_df = pd.concat([
-        frmgrp['form_action_flow'].apply(lambda x: ','.join(x)), 
-        frmgrp['form_action_ts'].apply(lambda x: ','.join(x))], axis=1).fillna('None')
-    
-    # combine all split visit columns
-    cdf = pd.concat([cdf, acts_df, pgs_df, dls_df, ols_df, etfs_df,
-                     brks_df, vids_df, frms_df], axis=1).fillna('None')
-    
-    # reset missing values in appropriate columns
-    cdt = cdf.index.get_level_values(2) if dt0 else cdf['datetime']
-    for pg in [col[:-1] for col in df.isnull().sum()[df.isnull().sum() > 0].index
-               if col.endswith('_pages')]:
-        cdf.loc[cdt <= df[df[pg + 's'].isnull()].sort_values(
-            by='datetime', ascending=False)['datetime'].iloc[0],
-                [col for col in cdf.columns if pg in col]] = np.nan
-    for dl in [col[:-1] for col in df.isnull().sum()[df.isnull().sum() > 0].index
-               if col.endswith('_downloads')]:
-        cdf.loc[cdt <= df[df[dl + 's'].isnull()].sort_values(
-            by='datetime', ascending=False)['datetime'].iloc[0],
-                [col for col in cdf.columns if col == dl + 's'
-                 or col == dl + '_duration']] = np.nan
-    for ol in [col[:-1] for col in df.isnull().sum()[df.isnull().sum() > 0].index
-               if col.endswith('_outlinks')]:
-        cdf.loc[cdt <= df[df[ol + 's'].isnull()].sort_values(
-            by='datetime', ascending=False)['datetime'].iloc[0],
-                [col for col in cdf.columns if ol in col]] = np.nan
-    if any(df['buyetfs'].isnull()):
-        cdf.loc[cdt <= df[df['buyetfs'].isnull()].sort_values(
-            by='datetime', ascending=False)['datetime'].iloc[0],
-                [col for col in cdf.columns if 'buyetf' in col]] = np.nan
-    for vid in [col.rsplit('_', 1)[0] for col in df.isnull().sum()[df.isnull().sum() > 0].index
-                if col.endswith('_video_plays')]:
-        cdf.loc[cdt <= df[df[vid + '_plays'].isnull()].sort_values(
-            by='datetime', ascending=False)['datetime'].iloc[0],
-                [col for col in cdf.columns if vid in col]] = np.nan
-    for frm in [col.rsplit('_', 1)[0] for col in df.isnull().sum()[df.isnull().sum() > 0].index
-                if col.endswith('_form_actions')]:
-        cdf.loc[cdt <= df[df[frm + '_actions'].isnull()].sort_values(
-            by='datetime', ascending=False)['datetime'].iloc[0],
-                [col for col in cdf.columns if frm in col]] = np.nan
-    
-    return cdf
-    
-    
-def clean_split_visits(df, true_split=True, same_time=True):
-    """
-    Clean split visits, combining true splits and dropping false splits.
-    
-    Combine true split visits, i.e. visits with duplicate visit counts per visitor 
-    occurring within thirty minutes of one another, and drop extraneous false splits,
-    i.e. visits with duplicate visit counts per visitor occurring more than thirty 
-    minutes from each other.
-    
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Dataframe of split visits.
-    true_split : bool
-        Whether split visits are true splits or false splits.
-    same_time : bool
-        Whether true splits occur at same time or different times.
-        
-    Returns
-    -------
-    pd.DataFrame
-        Cleaned dataframe of split visits.
-    """
-
-    # calculate differences in time between split visits
-    grp = df.sort_values(by='datetime').groupby(['visitor_id', 'visit_count'])
-    # --> deltadt = time between each split visit for given visitor ID and visit count
-    deltadt = grp['datetime'].apply(list).apply(
-        lambda x: [(x[i+1] - x[i]).total_seconds() for i in range(len(x)-1)]).rename('deltadt')
-    # --> visit_id_pairs = split visit pairs for which delta-dt calculated
-    visit_id_pairs = grp['visit_id'].unique().apply(
-        lambda x: [(x[i], x[i+1]) for i in range(len(x)-1)] if len(x) > 1 else
-        [(x[0], x[0])]).rename('visit_id_pairs')
-    split_dt = pd.concat([deltadt, visit_id_pairs], axis=1)
-    
-    # filter out split visits already cleaned (no duplicates)
-    split_mask = split_dt['deltadt'].str.len() > 0
-    split_dt = pd.concat([split_dt[split_mask]['deltadt'].explode(),
-                          split_dt[split_mask]['visit_id_pairs'].explode()], axis=1)
-    
-    # sum up total delta-dt for true splits occurring at different times or false splits
-    if not true_split or not same_time:
-        split_dt = pd.concat([
-            split_dt.reset_index().groupby(['visitor_id', 'visit_count'])['deltadt'].sum(),
-            split_dt['visit_id_pairs'].apply(
-                lambda x: list(x)).explode().drop_duplicates().reset_index().groupby([
-                    'visitor_id', 'visit_count'])['visit_id_pairs'].unique()], axis=1)
-    # set delta-dt thresholds for selecting split visits of given type
-    if true_split:
-        deltadt_mask = split_dt['deltadt'] == 0 if same_time else split_dt['deltadt'] < 1800
-    else:
-        deltadt_mask = split_dt['deltadt'] >= 1800
-    # isolate split visits of given type
-    split_ids = split_dt[deltadt_mask]['visit_id_pairs'].apply(
-        lambda x: list(x)).explode().drop_duplicates()
-    split_visits = df[df['visit_id'].isin(split_ids)].reset_index(drop=True)
-    
-    # combine true splits or drop false splits
-    if true_split: clean_splits = combine_true_splits(split_visits, same_time).reset_index()
-    else: clean_splits = drop_false_splits(split_visits)
-
-    # drop split visits of given type, and add newly cleaned split visits
-    df = df.drop(df.loc[df['visit_id'].isin(split_visits['visit_id'])].index)
-    df = pd.concat([df, clean_splits]).sort_values(by='visit_id').reset_index(drop=True)
-    
-    return df
-
-
-def get_split_visits(df):
-    """
-    Get split visits from visit-level data.
-    
-    Identify and return all split visits from visit-level data set, where split visits
-    are those with duplicate visit counts per visitor.
-    
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Dataframe of visits.
-    
-    Returns
-    -------
-    pd.DataFrame
-        Dataframe of split visits.
-    """
-
-    # count number of visit IDs associated with each visitor ID - visit count pair
-    visit_count = df.groupby(['visitor_id', 'visit_count'])['visit_id'].count()
-    
-    # isolate visitor ID - visit count pairs with multiple visit IDs
-    dupl_visit_count = visit_count[visit_count > 1]
-    
-    # pull out split visits from visit-level data set
-    split_visits = df.loc[df[['visitor_id', 'visit_count']].apply(
-        tuple, axis=1).isin(dupl_visit_count.index)].reset_index(drop=True)
-    
-    return split_visits
-
-
-def clean_duplicate_visits(df):
-    """
-    Clean duplicate visits from visit-level data.
-    
-    The real-time visits logged in the visit-level data set are sometimes prone to 
-    tracking errors by Matomo that result in duplicate visits. Such duplicate visits 
-    can take the form of true duplicates, where multiple rows contain identical entries 
-    but for the visit IDs attached to them. Alternatively, duplicate visits can appear 
-    in the form of split visits, where a single visit is split into multiple entries with 
-    different visit IDs and visit metrics for the same visit count and visitor ID. 
-    When such split visits occur within a small window of time, i.e. within thirty minutes 
-    of one another, such split visits represent true splits that should be recombined into 
-    the original visits from which they were split. On the other hand, when split visits 
-    are spread across large amounts of time, i.e. hours or days, they represent false splits, 
-    or truly unique visits that Matomo erroneously attributed the same visit count to, which 
-    are cleaned by dropping all but those with the longest visit durations or most activity.
-    
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Dataframe of visits.
-    
-    Returns
-    -------
-    pd.DataFrame
-        Dataframe of visits with cleaned duplicates.
-    """
-
-    # clean action ts columns: replace '0.0' with 'None'
-    for col in [col for col in df.columns if col.endswith('_ts')]:
-        df[col] = df[col].astype(str).replace('0.0', 'None')
-
-    # DROP DUPLICATE VISITS +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-    # duplicate visits = entries with identical metrics except for visit IDs
-    df = df.drop_duplicates(subset=[col for col in df.columns if
-                                    col != 'visit_id']).reset_index(drop=True)
-
-    
-    # IDENTIFY SPLIT VISITS +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-    # split visits = visits with duplicate visit counts per visitor
-    
-    # isolate split visits to be combined or cleaned
-    split_df = get_split_visits(df)
-
-    # keep track of initial split visit IDs (for dropping later)
-    split_visit_ids = split_df['visit_id']
-
-    # drop split visits with no actions (no use in combining these if nothing to combine)
-    split_df = split_df.drop(split_df[split_df['actions'] == 0].index).reset_index(drop=True)
-
-    # add datetime column
-    split_df['datetime'] = pd.to_datetime(split_df['date'].astype(str) + ' ' + split_df['time'])
-    
-    # COMBINE SAME-TIME TRUE SPLITS +++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-    # same-time true splits = split visits occurring at exact same time
-    if not split_df.empty:
-        split_df = clean_split_visits(split_df, true_split=True, same_time=True)
-    
-    # COMBINE DIFFERENT-TIME TRUE SPLITS ++++++++++++++++++++++++++++++++++++++++++++++++++++
-    # different-time true splits = split visits occurring within 30 minutes of one another
-    if not split_df.empty:
-        split_df = clean_split_visits(split_df, true_split=True, same_time=False)
-    
-    # CLEAN FALSE SPLITS ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-    # false splits = split visits occurring more than 30 minutes from each other
-    if not split_df.empty:
-        split_df = clean_split_visits(split_df, true_split=False)
-    
-    # DROP SPLIT VISITS AND REPLACE WITH CLEANED SPLITS +++++++++++++++++++++++++++++++++++++
-    df = df.drop(df[df['visit_id'].isin(split_visit_ids)].index)
-    df = pd.concat([df, split_df.drop(columns='datetime')],
-                   ignore_index=True).sort_values(by='visit_id').reset_index(drop=True)
-
-    # drop remaining duplicate visits, if any
-    df = df.drop(df[df.duplicated(subset='visit_id')].index).reset_index(drop=True)
-    
-    return df
-
-
-# CLEANING ATYPICAL VISITS ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-def drop_hki(df, db_dict):
-    """
-    Drop visits from Humankind employees and third-party vendors.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Visit-level data.
-    db_dict : dict
-        Dictionary of database credentials.
-    """
-
-    # DROP HUMANKIND EMPLOYEE VISITS ++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-
-    # read in ip addresses and locations of humankind employees
-    cursor, conn = database_connect('hkisocial', db_dict)
-    query = """SELECT * FROM ips ORDER BY name, description, start_date"""
-    ips = pd.read_sql(query, conn)
-    ips.ip = ips.ip.str.rsplit('.', n=2).str[0] + '.0.0'  # anonymize ips
-    cursor.close()
-    conn.close()
-
-    # merge with visits of same ips and locations
-    ip_grp = ips.groupby(['name', 'description', 'ip', 'city', 'region', 'country'])
-    vis_grp = df.groupby(['ip', 'city', 'region', 'country', 'date'])
-    ipvis = pd.merge(pd.concat([ip_grp.start_date.first(),
-                                ip_grp.end_date.last().fillna('9999-99-99')],
-                               axis=1).droplevel(['name', 'description']).reset_index(),
-                     vis_grp.visit_id.unique().reset_index(), how='left',
-                     on=['ip', 'city', 'region', 'country'])
-
-    # isolate visits with select ip-locations within relevant date ranges
-    ipvis = ipvis.drop(ipvis[(ipvis.date.astype(str) < ipvis.start_date) |
-                             (ipvis.date.astype(str) > ipvis.end_date)].index)
-    hki_visits = ipvis.visit_id.explode().tolist()
-
-    # isolate visitors with offending visits
-    hki_visitors = df[(df.referrer_type != 'campaign') &  # exclude campaign referrals
-                      (df.visit_id.isin(hki_visits))].visitor_id.tolist()
-
-    # drop non-campaign referral entries from humankind employees
-    df.drop(df[(df.visitor_id.isin(hki_visitors))].index, inplace=True)
-
-    # DROP VENDORS ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-
-    # drop yellow.system visitors
-    ys_visits = df[df.country.isin(['Belarus', 'Armenia', 'Georgia'])].visit_id.tolist()
-    ys_visitors = df[df.visit_id.isin(ys_visits)].visitor_id.tolist()
-    df.drop(df[(df.visitor_id.isin(ys_visitors))].index, inplace=True)
-    df.reset_index(drop=True, inplace=True)
-
-
-def drop_dev(df, db_dict):
-    """
-    Drop visitors with any visits to the dev sites.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Visit-level data.
-    db_dict : dict
-        Dictionary of database credentials.
-    """
-
-    # get list of unique visitors to dev sites from action log
-    cursor, conn = database_connect('hkiweb', db_dict)
-    query = """SELECT distinct visitor_id
-                 FROM action_log
-                WHERE split_part(regexp_replace(url, '(https?://)?(www.)?', ''), '/', 1)
-               NOT IN ('humankind.co', 'humankindfunds.com', 'rankings.humankind.co')
-            """
-    dev = pd.read_sql(query, conn)
-    cursor.close()
-    conn.close()
-
-    # drop dev-site visitors
-    df.drop(df[df.visitor_id.isin(dev.visitor_id)].index, inplace=True)
-    df.reset_index(drop=True, inplace=True)
-
-
-def drop_foreign(df):
-    """
-    Drop foreign visitors.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Visit-level data.
-    """
-
-    # count number of domestic and foreign visits per visitor
-    domestic = df.groupby('visitor_id').country.apply(
-        lambda x: [i for i in x if i == 'United States']).rename('domestic')
-    foreign = df.groupby('visitor_id').country.apply(
-        lambda x: [i for i in x if i != 'United States']).rename('foreign')
-
-    # count visitors with more foreign than domestic visits as foreign
-    foreign_visitors = foreign[foreign.str.len() > domestic.str.len()].index
-
-    # drop foreign visitors
-    df.drop(df[df.visitor_id.isin(foreign_visitors)].index, inplace=True)
-    df.reset_index(drop=True, inplace=True)
-
-
-# CLEANING ACTION FLOWS +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-def clean_flow(df, action_type, actions, deltat=0):
-    """
-    Clean action flows for individual action type.
-
-    Remove duplicate actions, i.e. consecutive actions of same type occurring
-    within given time range, from action flows. Update action flow, timestamp, 
-    count, and average duration columns with duplicate actions removed.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Dataframe of website visits.
-    action_type : str
-        Type of action for which to clean flows. Valid options are 'pageview',
-        'download', 'outlink_click', 'buyetf_click', 'brokerlink_click', 'video_action',
-        and 'form_action'. An invalid action flow will cause the
-        function to return without making any modifications to the dataframe.
-    actions : pd.DataFrame
-        Dataframe of individual actions of all type over all visits.
-    deltat : int
-        Maximum time difference, in seconds, between consecutive actions for which to 
-        apply cleaning. Consecutive actions occurring within delta-t seconds of one 
-        another will be cleaned, with the latter of the two being removed from the action flow. 
-        Default of 0 cleans consecutive actions occurring at exactly the same time only.
-    """
-
-    # exit if action type not valid option
-    if action_type not in ['pageview',
-                           'download',
-                           'outlink_click',
-                           'buyetf_click',
-                           'brokerlink_click',
-                           'video_action',
-                           'form_action',
-                          ]: return df
-
-    # get action string
-    action_str = action_type
-    if action_type == 'pageview': action_str = 'page'
-    elif action_type.split('_')[-1] == 'click': action_str = action_type.split('_')[0]
-
-    # get individual actions and timestamps of given type per visit
-    acts_mask = (actions.action_flow.str.endswith('_' + action_type))
-    if action_type == 'buyetf_click':
-        acts_mask = (actions.action_flow == 'buyetf_click')
-    elif action_type.split('_')[-1] == 'action':
-        acts_mask = (actions.action_flow.str.split('_', n=1).str[-1].str.split('_').str[0] ==
-                     action_type.split('_')[0])  # *_video/form_*
-    acts = actions[acts_mask].rename(
-        columns={col : col.replace('action', action_str) for col in actions.columns})
-    acts[action_str + '_flow'] = acts[action_str + '_flow'].replace(
-        '_' + action_type, '', regex=True)
-
-    # find duplicate actions of given type and update action type flow/ts columns
-    dupl_mask = ((actions.visit_id == actions.visit_id.shift()) &  # same visit id
-                 (actions.action_flow == actions.action_flow.shift()) &  # same action 
-                 (actions.action_ts_int - actions.action_ts_int.shift() <= deltat)  # time in range
-                )        
-    dupl_acts = actions.loc[dupl_mask & acts_mask]
-    act_grp = acts.drop(dupl_acts.index).groupby('visit_id', group_keys=False)
-    flow_cols = [action_str + '_ts']
-    if action_type != 'buyetf_click': flow_cols = [action_str + '_flow'] + flow_cols
-    for col in flow_cols:
-        df[col] = act_grp[col].apply(lambda x: ','.join(x))
-        df[col] = df[col].fillna('None')
-
-    # update action type counts and average durations
-    df[action_str + 's'] = df[action_str + '_ts'].apply(
-        lambda x: 0 if x == 'None' else len(x.split(',')))
-    if action_type != 'form_action':
-        if action_type != 'pageview':  # modify page action duration instead
-            df[action_str + '_duration'] = act_grp[action_str + '_duration'].sum()
-            df[action_str + '_duration'] = df[action_str + '_duration'].fillna(0).astype(int)
-        df['avg_' + action_str + '_duration'] = (df[action_str + '_duration'] /
-                                                 df[action_str + 's']).fillna(0)
-    if action_type == 'pageview':
-        df.page_action_duration = act_grp[action_str + '_duration'].sum()
-        df.page_action_duration = df.page_action_duration.fillna(0).astype(int)
-        df.avg_page_action_duration = (df.page_action_duration / df.pages).fillna(0)
-    elif action_type == 'form_action':
-        df.avg_form_interaction_time = (df.form_interaction_time / df.form_actions).fillna(0)
-
-    # update individual action type counts: subtract duplicate actions from corresponding columns
-    dupl_acts = dupl_acts.drop(columns=['action_path_flow', 'action_ts'])
-    if action_type == 'buyetf_click': return  # no further columns to update
-    elif action_type.split('_')[-1] != 'action':
-        dupl_acts.action_flow = dupl_acts.action_flow.str.replace(action_type, action_str + 's')
-        if action_type == 'pageview':  # combine individual article post / company ranking pages
-            dupl_acts.action_flow = dupl_acts.action_flow.apply(
-                lambda x: re.sub('articles-.*_pages', 'article-post_pages', x)).apply(
-                lambda x: re.sub('rankings-.*_pages', 'ranked-company_pages', x))
-            dupl_acts.action_flow = np.select(  # map socially responsible pages to site homepages
-                [(dupl_acts.action_flow == 'socially_responsible_pages') &
-                 (dupl_acts.action_site_flow == 'humankind.co'),
-                 (dupl_acts.action_flow == 'socially_responsible_pages') &
-                 (dupl_acts.action_site_flow == 'humankindfunds.com')],
-                ['humankind_pages', 'humankindfunds_pages'], default=dupl_acts.action_flow)
-            dupl_acts = dupl_acts.loc[dupl_acts.action_flow != 'page-not-found_pages']
-        elif action_type == 'outlink_click':  # combine categories of outlinks
-            dupl_acts.action_flow = dupl_acts.action_flow.apply(
-                lambda x: re.sub('(linkedin|instagram|youtube|facebook|twitter)_outlinks',
-                                 'social_outlinks', x)).apply(
-                lambda x: re.sub('(investor|adviserinfo.sec)_outlinks', 'crs_outlinks', x)).apply(
-                lambda x: re.sub('(finra|sipc)_outlinks', 'disclosures_outlinks', x))
-            # drop article outlinks: no good way to track this category
-            df.drop(columns = [col for col in df.columns if
-                               col.startswith('articles_outlink')], inplace=True)
-        actcols = [col for col in df.columns if col.endswith('_' + action_str + 's')]
-        dupl_actcts = dupl_acts.groupby('visit_id').action_flow.apply(lambda x: [i for i in x])
-        dupl_actcts = pd.concat([dupl_actcts, pd.DataFrame(columns=actcols)], axis=1).fillna(0)
-        for col in actcols:
-            dupl_actcts[col] = dupl_actcts.action_flow.apply(
-                lambda x: len([i for i in x if i == col]))
-            df.loc[df.index.isin(dupl_actcts.index), col] = df[col] - dupl_actcts[col]
-            df[col] = df[col].astype(float)
-    else:  # handle video and form actions separately
-        actpre = action_type.split('_')[0]
-        if actpre == 'video': subs = ['play', 'pause', 'resume', 'seek', 'finish']
-        elif actpre == 'form': subs = ['submission']
-        subs = [actpre + '_' + i for i in subs]
-        subcols = [col for col in df.columns for i in subs if
-                   col == (i + 'es' if i.endswith('sh') else i + 's')]
-        actcols = [col for col in df.columns for i in subcols if col.endswith('_' + i)]
-        for icol, col in enumerate(subcols):
-            dupl_acts.action_flow = dupl_acts.action_flow.str.replace(subs[icol], col)
-        dupl_actcts = dupl_acts.groupby(
-            'visit_id', group_keys=False).action_flow.apply(lambda x: [i for i in x])
-        dupl_actcts = pd.concat(
-            [dupl_actcts, pd.DataFrame(columns=subcols+actcols)], axis=1).fillna(0)
-        for col in subcols:  # duplicate total subactions
-            dupl_actcts[col] = dupl_actcts.action_flow.apply(
-                lambda x: len([i for i in x if i.endswith('_' + col)]))
-        for col in actcols:  # duplicate subactions by video/form
-            dupl_actcts[col] = dupl_actcts.action_flow.apply(
-                lambda x: len([i for i in x if i == col]))
-        for col in subcols + actcols:
-            df.loc[df.index.isin(dupl_actcts.index), col] = df[col] - dupl_actcts[col]
-            df[col] = df[col].astype(float)
-        if actpre == 'video':  # update average video columns
-            df.avg_video_watch_time = (df.video_watch_time / df.video_plays).replace(
-                np.inf, 0).fillna(0)
-
-        
-def clean_action_flows(df, deltat=0):
-    """
-    Clean action flows.
-
-    Remove duplicate actions, i.e. consecutive actions of same type occurring at
-    once, from action flows. Update action flow, timestamp, count, and average
-    duration columns for total and individual action types with duplicate actions removed.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Dataframe of website visits.
-
-    Returns
-    -------
-    pd.DataFrame
-        Dataframe of website visits with cleaned action flows.
-    deltat : int
-        Maximum time difference, in seconds, between consecutive actions for which to 
-        apply cleaning. Consecutive actions occurring within delta-t seconds of one 
-        another will be cleaned, with the latter of the two being removed from the action flow. 
-        Default of 0 cleans consecutive actions occurring at exactly the same time only.
-    """
-
-    # set visit id as index
-    df.set_index('visit_id', inplace=True)
-
-    # clean action ts columns: replace '0.0' with 'None'
-    for col in [col for col in df.columns if col.endswith('_ts')]:
-        df[col] = df[col].replace('0.0', 'None')
-
-    # clean up action path flow --> remove split entries for page-not-found pageviews
-    bad_flows = df[df.action_flow.str.split(',').str.len() !=
-                   df.action_path_flow.str.split(',').str.len()].action_path_flow
-    df.loc[df.index.isin(bad_flows.index),
-           'action_path_flow'] = bad_flows.str.rstrip(',').apply(
-        lambda x: ','.join([i for i in x.split(',') if not
-                            i.startswith('<svg') and i not in ['/)', "'"]]))
-
-    # get individual actions and timestamps per visit
-    actions = pd.concat([df.action_flow.apply(lambda x: x.split(',')).explode(),
-                         df.action_site_flow.apply(lambda x: x.split(',')).explode(),
-                         df.action_path_flow.apply(lambda x: x.split(',')).explode(),
-                         df.action_ts.apply(lambda x: x.split(',')).explode(),
-                         ], axis=1).sort_values(by=['visit_id', 'action_ts']).reset_index()
-    actions['action_ts_int'] = actions.action_ts.fillna('None').replace('None', '0').astype(int)
-
-    # find duplicate actions (consecutive same actions within time range) and update flow/ts columns
-    dupl_mask = (
-        (actions.visit_id == actions.visit_id.shift()) &  # same visit id
-        (actions.action_flow == actions.action_flow.shift()) &  # same action
-        (actions.action_ts_int - actions.action_ts_int.shift() <= deltat)  # timestamps in range
-        )
-    act_clean = actions.drop(actions.loc[dupl_mask].index)
-    act_clean['action_duration'] = act_clean.groupby(
-        'visit_id').action_ts_int.diff(1).shift(-1).abs()
-    actions['action_duration'] = act_clean['action_duration']
-    act_grp = act_clean.groupby('visit_id')
-    for col in ['action_flow', 'action_site_flow', 'action_path_flow', 'action_ts']:
-        df[col] = act_grp[col].apply(lambda x: ','.join(x))
-
-    # update action count, action duration, and average duration columns
-    df.actions = df.action_flow.apply(lambda x: 0 if x == 'None' else len(x.split(',')))
-    df.action_duration = act_grp.action_duration.sum()
-    df.action_duration = df.action_duration.fillna(0).astype(int)
-    df.avg_action_duration = (df.action_duration / df.actions).fillna(0)
-
-    # clean individual action type flows
-    for action_type in ['pageview',
-                        'download',
-                        'outlink_click',
-                        'buyetf_click',
-                        'brokerlink_click',
-                        'video_action',
-                        'form_action',
-                        ]: clean_flow(df, action_type, actions, deltat)
-
-    # reset index
-    df.reset_index(inplace=True)
-
-
-def clean_standalone_action(df, action_type, deltat=0):
-    """
-    Clean individual action type flow and update overall action flow.
-
-    Remove duplicate actions of given type, i.e. consecutive actions occurring 
-    within given time range, from overall and specific action flows. 
-    Update action flow, timestamp, count, and average duration columns with 
-    duplicate actions removed.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Dataframe of website visits.
-    action_type : str
-        Type of action for which to clean flows. Valid options are 'pageview',
-        'download', 'outlink_click', 'buyetf_click', 'brokerlink_click', 
-        'video_action', and 'form_action'. An invalid action flow will cause the
-        function to return without making any modifications to the dataframe.
-    deltat : int
-        Maximum time difference, in seconds, between consecutive actions for which to 
-        apply cleaning. Consecutive actions occurring within delta-t seconds of one 
-        another will be cleaned, with the latter of the two being removed from the action flow. 
-        Default of 0 cleans consecutive actions occurring at exactly the same time only.
-    """
-
-    # set visit id as index
-    df.set_index('visit_id', inplace=True)
-    
-    # get individual actions and timestamps per visit
-    actions = pd.concat([df.action_flow.apply(lambda x: x.split(',')).explode(),
-                         df.action_site_flow.apply(lambda x: x.split(',')).explode(),
-                         df.action_path_flow.apply(lambda x: x.split(',')).explode(),
-                         df.action_ts.apply(lambda x: x.split(',')).explode(),
-                         ], axis=1).sort_values(by=['visit_id', 'action_ts']).reset_index()
-    actions['action_ts_int'] = actions.action_ts.fillna('None').replace('None', '0').astype(int)
-    
-    # get individual actions and timestamps of given type per visit
-    acts_mask = (actions.action_flow.str.endswith('_' + action_type))
-    if action_type == 'buyetf_click':
-        acts_mask = (actions.action_flow == 'buyetf_click')
-    elif action_type.split('_')[-1] == 'action':
-        acts_mask = (actions.action_flow.str.split('_', n=1).str[-1].str.split('_').str[0] ==
-                     action_type.split('_')[0])  # *_video/form_*
-    
-    # find duplicate actions (consecutive same actions within time range) and update flow/ts columns
-    dupl_mask = (
-        (actions.visit_id == actions.visit_id.shift()) &  # same visit id
-        (actions.action_flow == actions.action_flow.shift()) &  # same action
-        (actions.action_ts_int - actions.action_ts_int.shift() <= deltat)  # timestamps in range
-        )
-    # drop duplicate actions of given type
-    act_clean = actions.drop(actions.loc[dupl_mask & acts_mask].index)
-    act_clean['action_duration'] = act_clean.groupby(
-        'visit_id').action_ts_int.diff(1).shift(-1).abs()
-    actions['action_duration'] = act_clean['action_duration']
-    act_grp = act_clean.groupby('visit_id')
-    for col in ['action_flow', 'action_site_flow', 'action_path_flow', 'action_ts']:
-        df[col] = act_grp[col].apply(lambda x: ','.join(x))
-
-    # update action count, action duration, and average duration columns
-    df.actions = df.action_flow.apply(lambda x: 0 if x == 'None' else len(x.split(',')))
-    df.action_duration = act_grp.action_duration.sum()
-    df.action_duration = df.action_duration.fillna(0).astype(int)
-    df.avg_action_duration = (df.action_duration / df.actions).fillna(0)
-    
-    # clean individual action type flow
-    clean_flow(df, action_type, actions, deltat)
-    
-    # reset index
-    df.reset_index(inplace=True)
-    
-
-
-# VISITOR-LEVEL DATA ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-def categorize_visitor_action_flow(df):
-    """
-    Categorize visitor-level action flows - map specific actions to categories.
-    
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Raw visitor-level data.
-    """
-    
-    # separate actions
-    adf = df.action_flow.str.split(',').explode()
-    
-    # map actions to categories
-    subs = {r'^(.*)_socially_responsible_pageview$' :
-            r'\1_pageview',
-            r'^articles-.*_pageview$' :
-            'articles-post_pageview',
-            r'^rankings_.*_pageview$' :
-            'rankings_pageview',
-            r'^rankings-.*_pageview$' :
-            'rankings-company_pageview',
-            r'^.*\.(jpg|png|eps)_download$' :
-            'logo_download',
-            r'^(linkedin|youtube|twitter|instagram|facebook)_outlink_click$' :
-            'social_outlink_click',
-            r'^(adviserinfo\.sec|sipc|finra|investor)_outlink_click$' :
-            'compliance_outlink_click',
-            r'^(theconversation|benefitcorporationreduced|onlinelibrary\.wiley)_outlink_click$' :
-            'articles_outlink_click',
-            r'^(.*)_video_.*$' :
-            r'\1_video_action',
-            r'^(.*)_form_.*$' :
-            r'\1_form_action',
-           }
-    for sub in subs.items():
-        adf = adf.apply(lambda x: re.sub(r'^{}$'.format(sub[0]), sub[1], x))
-        
-    # regroup actions and insert new categorical column into dataframe
-    adf = adf.groupby('visitor_id').apply(lambda x: ','.join(x))
-    df.insert(df.columns.get_loc('action_flow')+1, 'action_category_flow', adf)
-
-
-def clean_visitor_action_flow(df):
-    """
-    Clean raw visitor-level action flows - map extraneous actions.
-    
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Raw visitor-level data.
-    """
-    
-    # build dataframe of individual actions
-    adf = pd.concat([df.action_flow.str.split(',').explode(), 
-                     df.action_site_flow.str.split(',').explode(),
-                     df.action_ts.str.split(',').explode(),
-                    ], axis=1)
-
-    # map socially responsible pages to proper homepages
-    srpg = 'socially_responsible_pageview'
-    for site in ['humankind.co', 'humankindfunds.com']:
-        adf.loc[(adf.action_flow == srpg) & (adf.action_site_flow == site),
-                'action_flow'] = site.split('.')[0] + '_' + srpg
-
-    # map original rankings company pages to corresponding year
-    adf.action_flow = np.where((adf.action_flow.str.startswith('rankings-')) &
-                               (adf.action_flow.str.endswith('_pageview')),
-                               adf.action_flow.str.replace('_pageview', '-2022_pageview'),
-                               adf.action_flow)
-        
-    # map article post and rankings company pageviews with bad urls to page-not-found
-    fpats = ['^articles-', '^rankings-']
-    bpat = '_pageview$'
-    for fpat in fpats:
-        pgmask = (adf.action_flow.apply(lambda x: bool(re.match(r'{}.*{}'.format(fpat, bpat), x))))
-        if fpat[1:-1] == 'articles':
-            patmask = (~(adf.action_flow.apply(lambda x: bool(
-                re.match(r'({}(?=.*?\-)[a-z0-9\-]*{})'.format(fpat, bpat), x)))) |
-                       (adf.action_flow.apply(lambda x: bool(
-                           re.match(r'({}frame-[a-z0-9]*{})'.format(fpat, bpat), x)))))
-        elif fpat[1:-1] == 'rankings':
-            patmask = ~(adf.action_flow.apply(
-                lambda x: '-' in re.sub(r'-[\d]{4}', '', x.replace('rankings-', ''))))
-        adf.loc[pgmask & patmask, 'action_flow'] = 'page-not-found_pageview'
-        
-    # map article link downloads to outlink clicks
-    link_dls = ['benefitcorporationreduced']
-    for link_dl in link_dls:
-        adf.loc[adf.action_flow == '{}_download'.format(link_dl),
-                'action_flow'] = '{}_outlink_click'.format(link_dl)
-        
-    df.action_flow = adf.groupby('visitor_id').action_flow.apply(lambda x: ','.join(x))
-    
-    
-def build_raw_visitor_data(vdf):
-    """
-    Build raw visitor-level data set.
-
-    Raw visitor data = time-ordered list of visits and activities across customer lifetime.
-    
-    Parameters
-    ----------
-    vdf : pd.DataFrame
-        Raw visit-level data.
-
-    Returns
-    -------
-    pd.DataFrame
-        Raw visitor-level data.
-    """
-
-    # initialize dataframe
-    df = pd.DataFrame()
-
-    # copy input dataframe (avoid modifying original)
-    vdf = vdf.copy()
-
-    # add necessary columns to input dataframe
-    vdf['datetime'] = vdf.date.astype(str) + ' ' + vdf.time
-    vdf['timestamp'] = vdf.datetime.apply(lambda x: eastern.localize(
-        datetime.strptime(x, '%Y-%m-%d %H:%M:%S')).timestamp()).astype(int)
-    vdf['bounce'] = (vdf.visit_duration == 0).astype(int)
-    vdf['true_bounce'] = ((vdf.visit_duration == 0) &
-                          (vdf.actions - vdf.pages == 0) & (vdf.pages < 2)).astype(int)
-    vdf['mobile'] = (vdf.device_category == 'mobile').astype(int)
-    vdf['desktop'] = (vdf.device_category == 'desktop').astype(int)
-    dict_cols = {'location' : ['city', 'region', 'country', 'continent'],
-                 'campaign' : [col for col in vdf.columns if col.startswith('campaign')]}
-    for out_col, in_cols in dict_cols.items():
-        vdf[out_col] = vdf[in_cols].apply(lambda x: ','.join(x), axis=1)
-        vdf[out_col] = vdf[out_col].apply(
-            lambda x: {in_cols[i] : x.split(',')[i] for i in range(len(in_cols))})
-    
-    # add engagement types
-    if 'engagement_type' not in vdf.columns:
-        visit_engagement = assign_cluster(vdf).reset_index()
-        vdf = vdf.merge(visit_engagement, how='left', on='visit_id')
-    vdf['engagement_type'] = vdf.engagement_type.str.replace(',', '').str.replace(' ', '_')
-    
-    # modify flow columns in input dataframe to include session starts/ends
-    flows = ['action', 'action_site', 'page']
-    for flow in flows:
-        vdf[flow + '_flow'] = 'session-start,' + vdf[flow + '_flow'] + ',session-end'
-    for flow in [flow for flow in flows if flow != 'action_site']:
-        vdf[flow + '_ts'] = '0,' + vdf[flow + '_ts'] + ',1'
-    
-    # group by visitor id in order of visit
-    grp = vdf.sort_values(by='visit_id').groupby('visitor_id')
-
-    # visitor lifetime
-    df['datetime'] = grp.datetime.agg(list)
-    df['timestamp'] = grp.timestamp.agg(list)
-    df['day'] = grp.day.agg(list)
-    df['visit_trade_hours'] = grp.visit_trade_hours.agg(list)
-    
-    # visits
-    df['visits'] = grp.visit_count.max()
-    df['visit_count'] = grp.visit_count.agg(list)
-    df['visit_id'] = grp.visit_id.agg(list)
-    df['visit_duration'] = grp.visit_duration.agg(list)
-    
-    # bounce rates
-    df['bounce'] = grp.bounce.agg(list)
-    df['bounce_rate'] = grp.bounce.sum().div(df.visits)
-    df['true_bounce'] = grp.true_bounce.agg(list)
-    df['true_bounce_rate'] = grp.true_bounce.sum().div(df.visits)
-
-    # devices
-    df['device_category'] = grp.device_category.agg(list)
-    df['mobile_desktop_ratio'] = grp.mobile.sum().div(grp.desktop.sum()).replace(np.inf, 0)
-    
-    # locations
-    df['location'] = grp.location.agg(list)
-    
-    # referrals
-    df['referrer_type'] = grp.referrer_subtype.agg(list)
-    df['referrer_website'] = grp.referrer_website_url.agg(list)
-    df['referrer_social_network'] = grp.referrer_social_network_name.agg(list)
-    df['referrer_search_engine'] = grp.referrer_search_engine_name.agg(list)
-    df['referrer_search_engine_keyword'] = grp.referrer_search_engine_keyword.agg(list)
-    df['campaign'] = grp.campaign.agg(list)
-
-    # actions
-    df['actions'] = grp.actions.agg(list)
-    df['action_duration'] = grp.action_duration.agg(list)
-    df['page_duration'] = grp.page_duration.agg(list)
-    df['page_action_duration'] = grp.page_action_duration.agg(list)
-    df['action_flow'] = grp.action_flow.apply(lambda x: ','.join(x))
-    df['action_site_flow'] = grp.action_site_flow.apply(lambda x: ','.join(x))
-    df['action_ts'] = grp.action_ts.apply(lambda x: ','.join(x))
-        
-    # engagement types
-    df['engagement_flow'] = grp.engagement_type.apply(lambda x: ','.join(x))
-
-    # clean and categorize action flows
-    clean_visitor_action_flow(df)
-    categorize_visitor_action_flow(df)
-    
-    return df
-
-
-def get_asset_urls(url, urls):
-    """
-    Get URLs of all assets on advisor site.
-    
-    Parameters
-    ----------
-    url : str
-        Main assets page URL.
-    urls : list of str
-        List of assets urls. This list is changed in place.
-    """
-    
-    # recursively loop through assets folders to get urls
-    response = requests.request('GET', url)
-    content = response.content
-    soup = BeautifulSoup(content, 'html.parser')
-    divs = soup.find_all('div', class_=re.compile('assets_folder__[a-zA-Z0-9]*'))
-    for div in divs:
-        links = div.find_all('a')
-        for link in links:
-            new_url = os.path.join(url, link.string)
-            urls.append(new_url)
-            get_asset_urls(new_url, urls)
-
-
-def get_action_category_map():
-    """
-    Build numerical mapping for categorical action flows.
-    
-    Returns
-    -------
-    dict of {str : int}
-        Dictionary mapping categorical actions to integers.
-    """
-    
-    # replace hardcoding for some actions, i.e. downloads, brokerlinks, with site scraping (?)
-    action_dict = {
-        'pageview' : ['humankind', 'mission', 'research', 'team', 'articles',
-                      'articles-post', 'rankings', 'rankings-company', 'humankindfunds',
-                      'etf-explanation', 'topcompanies', 'shareholders', 'tax-information',
-                      'investors', 'contact', 'relationship', 'terms', 'page-not-found'],
-        'download' : ['summaryprospectus', 'prospectus', 'prospectussupplement',
-                      'sai', 'methodology', 'factsheet', 'premiumdiscountchart',
-                      'quarterlyreport', 'semiannualreport', 'annualreport', 'benefitreport',
-                      '8937', 'holdings', 'crs', 'logo'],
-        'outlink_click' : ['social', 'compliance', 'articles'],
-        'click' : ['buyetf'],
-        'brokerlink_click' : ['robinhood', 'fidelity', 'vanguard', 'schwab',
-                              'tdameritrade', 'etrade', 'interactivebrokers'],
-        'video_action' : ['humankind-short', 'humankind', 'wtf-short', 'wtf'],
-        'form_action' : ['getstarted', 'newsletter', 'contactus', 'institutionalcontact'],
-    }
-    
-    action_list = []
-    for action_type, actions in action_dict.items(): 
-        actions = [action + '_' + action_type for action in actions]
-        for action in actions: action_list.append(action)
-    action_list += ['session-start', 'session-end', 'None']
-    
-    return {action : i for i, action in enumerate(action_list)}
-
-
-def get_action_map():
-    """
-    Build numerical mapping for full action flows.
-    
-    Returns
-    -------
-    dict of {str : int}
-        Dictionary mapping granular actions to integers.
-    """
-
-    # grab individual article posts in order of appearance on site
-    url = 'https://www.humankind.co/articles'
-    response = requests.request('GET', url)
-    content = response.content
-    soup = BeautifulSoup(content, 'html.parser')
-    article_list = []
-    for link in soup.find_all('a'):
-        href = link.get('href').strip('/')
-        if href.startswith('articles/') and not link.get('class'):
-            article_list.append(href.replace('/', '-') + '_pageview')
-    
-    # grab individual company rankings in order of rank and year on site
-    url = 'https://rankings.humankind.co/{}'
-    year_list = [str(i) for i in range(2022, int(datetime.now().year)+1)]
-    year_list = [''] + year_list  # temporary --> remove empty string when rankings site migrated
-    ranking_list = []
-    for year in year_list:
-        year_url = url.format(year)
-        response = requests.request('GET', year_url)
-        content = response.content
-        soup = BeautifulSoup(content, 'html.parser')
-        data = soup.find_all('script', id='__NEXT_DATA__')[0].contents[0]
-        data = json.loads(data)
-        if 'companies' in data['props']['pageProps']:
-            # --> remove condition below after site update
-            if year != '': ranking_list.append('rankings_' + year + '_pageview')
-            for company in data['props']['pageProps']['companies']['items']:
-                ranking_list.append('rankings-' + company['slug'] + '_pageview')
-    # --> temporary until site updated...
-    ranking_list = [ranking.replace('_pageview', '-2022_pageview') for
-                    ranking in ranking_list if ranking.startswith('rankings')]
-
-    # grab individual logo downloads in order of appearance on site
-    url = 'https://www.humankind.co/assets'
-    asset_urls = []
-    get_asset_urls(url, asset_urls)
-    logo_list = []
-    for url in asset_urls:
-        response = requests.request('GET', url)
-        content = response.content
-        soup = BeautifulSoup(content, 'html.parser')
-        for link in soup.find_all('a'): 
-            href = link.get('href')
-            if not href: continue
-            href = href.strip('/')
-            if href.startswith('assets'): logo_list.append(re.sub(
-                    r'(hknd|humankind|[\d_%]+)', '', href.split('/')[-1].lower()) + '_download')
-
-    # expand individual social and compliance outlinks
-    outlink_list = ['facebook', 'twitter', 'instagram', 'linkedin', 'youtube',
-                    'investor', 'adviserinfo.sec', 'finra', 'sipc',
-                    'theconversation', 'benefitcorporationreduced', 'onlinelibrary.wiley']
-    outlink_list = [outlink + '_outlink_click' for outlink in outlink_list]
-    # --> scrape rest of outlinks from site (?)
-
-    # expand video actions to individual plays, pauses, resumes, seeks, and finishes
-    video_list = []
-    for video in ['humankind-short', 'humankind', 'wtf-short', 'wtf']:
-        for video_act in ['video_play', 'video_pause', 'video_resume', 'video_seek',
-                          'video_finish']: video_list.append(video + '_' + video_act)
-
-    # expand form actions to individual interactions and submissions
-    form_list = []
-    for form in ['getstarted', 'newsletter', 'contactus', 'institutionalcontact']:
-        for form_act in ['form_interaction', 'form_submission']:
-            form_list.append(form + '_' + form_act)
-
-    # build full action list
-    action_list = [i for i in get_action_category_map()]
-    article_index = action_list.index('articles-post_pageview')
-    action_list[article_index:article_index] = article_list
-    action_list.remove('articles-post_pageview')
-    ranking_index = action_list.index('rankings-company_pageview')
-    action_list[ranking_index:ranking_index] = ranking_list
-    action_list.remove('rankings-company_pageview')
-    logo_index = action_list.index('logo_download')
-    action_list[logo_index:logo_index] = logo_list
-    action_list.remove('logo_download')
-    outlink_index = action_list.index('social_outlink_click')
-    action_list[outlink_index:outlink_index] = outlink_list
-    for ol in ['social_outlink_click', 'articles_outlink_click', 'compliance_outlink_click']:
-        action_list.remove(ol)
-    video_index = action_list.index('humankind-short_video_action')
-    action_list[video_index:video_index] = video_list
-    for vid in ['humankind-short_video_action', 'humankind_video_action',
-                'wtf-short_video_action', 'wtf_video_action']:
-        action_list.remove(vid)
-    form_index = action_list.index('getstarted_form_action')
-    action_list[form_index:form_index] = form_list
-    for frm in ['getstarted_form_action', 'newsletter_form_action',
-                'contactus_form_action', 'institutionalcontact_form_action']:
-        action_list.remove(frm)
-    for hmpg in ['humankind', 'humankindfunds']: action_list.insert(
-            action_list.index(hmpg + '_pageview')+1, hmpg + '_socially_responsible_pageview')
-
-    # map actions to numbers
-    return {action : i for i, action in enumerate(action_list)}
-
-
-def get_site_map():
-    """
-    Build numerical mapping for site flows.
-    
-    Returns
-    -------
-    dict of {str : int}
-        Dictionary mapping sites to integers.
-    """
-    
-    site_list = ['humankind.co', 'rankings.humankind.co', 'humankindfunds.com',
-                 'session-start', 'session-end', 'None']
-    return {site : i for i, site in enumerate(site_list)}
-
-
-def get_engage_map():
-    """
-    Build numerical mapping for engagement flows.
-    
-    Returns
-    -------
-    dict of {str : int}
-        Dictionary mapping engagement types to integers.
-    """
-    
-    return {val.replace(',', '').replace(' ', '_') : key for
-            key, val in get_cluster_grades().engagement_type.to_dict().items()}
-
-
-def map_action_flow(df, colstr='', action_types=[], drop_sessions=False, drop_none=False):
-    """
-    Map action flows to numerical sequences.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Raw visitor-level data.
-    colstr : str
-        String to replace 'action' in action flow column names.
-    action_types : list of str
-        Action types to include in flows.
-    drop_sessions : bool
-        Whether to drop 'session-start' and 'session-end' from action flows.
-    drop_none : bool
-        Whether to drop 'None' from action flows.
-
-    Returns
-    -------
-    pd.DataFrame
-        Dataframe of numerical sequences of given action type flows.
-    """
-    
-    action_flow = []
-    actflow_cols = ['action_flow', 'action_category_flow', 'action_site_flow', 'action_ts']
-    for col in actflow_cols: action_flow.append(df[col].str.split(',').explode())
-    action_flow = pd.concat(action_flow, axis=1).reset_index()
-    
-    # filter action flow based on action types
-    pat_ix = pd.Index([])  # select actions of given types 
-    pat = r'.*_({})'.format('|'.join(action_types))
-    pat_ix = action_flow.loc[action_flow.action_flow.apply(
-        lambda x: bool(re.match(pat, x)))].index
-    sess_ix = pd.Index([])  # select session-starts/ends
-    if not drop_sessions: sess_ix = action_flow.loc[
-            action_flow.action_flow.isin(['session-start', 'session-end'])].index
-    none_ix = pd.Index([])  # select None's
-    if not drop_none: none_ix = action_flow.loc[
-            action_flow.action_flow == 'None'].index
-    drop_ix = action_flow.index.difference(pat_ix.union(sess_ix).union(none_ix))  # drop other ix
-    action_flow = action_flow.drop(drop_ix)
-    
-    # map actions to numbers
-    action_flow.action_flow = action_flow.action_flow.map(get_action_map())
-    action_flow.action_category_flow = action_flow.action_category_flow.map(
-        get_action_category_map())
-    action_flow.action_site_flow = action_flow.action_site_flow.map(get_site_map())
-    
-    # drop rows with missing values
-    action_flow = action_flow.drop(action_flow[action_flow.isnull().any(axis=1)].index)
-    action_flow[actflow_cols[:-1]] = action_flow[actflow_cols[:-1]].astype(int).astype(str)
-    
-    # group actions by visitor id to build numerical sequence columns
-    vdf = pd.DataFrame()
-    for col in actflow_cols:
-        outcol = col.replace('action', colstr) if colstr else col
-        vdf[outcol] = action_flow.groupby('visitor_id')[col].apply(lambda x: ','.join(x))
-    
-    return vdf
-
-
-def map_engage_flow(df):
-    """
-    Map engagement flows to numerical sequences.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Raw visitor-level data.
-
-    Returns
-    -------
-    pd.DataFrame
-       Numerical sequences of engagement types across visits.
-    """
-    
-    engage_flow = df.engagement_flow.str.split(',').explode()
-    engage_flow = engage_flow.map(get_engage_map()).astype(str)
-    engage_flow = pd.DataFrame(engage_flow.groupby('visitor_id').apply(lambda x: ','.join(x)))
-    
-    return engage_flow
-
-
-def build_processed_visitor_data(visits=None, visitors=None, drop_sessions=False, drop_none=False):
-    """
-    Build processed visitor-level data set.
-
-    Processed visitor data = summary data and numerical sequences representing customer journeys.
-    
-    Parameters
-    ----------
-    visits : pd.DataFrame
-        Raw visit-level data. If none passed in, must pass in raw visitor-level data instead.
-    visitors : pd.DataFrame
-        Raw visitor-level data. If none passed in, will build on the fly.
-    drop_sessions : bool
-        Whether to drop 'session-start' and 'session-end' from action flows.
-    drop_none : bool
-        Whether to drop 'None' from action flows.
-
-    Returns
-    -------
-    pd.DataFrame
-        Processed visitor-level data.
-    """
-
-    # get raw visitor-level data
-    if visitors is None:
-        if visits is None: raise Exception('Must pass in either raw visit- or visitor-level data.')
-        visitors = build_raw_visitor_data(visits)
-
-    df = visitors.copy()
-
-    # get summary data
-    df.actions = df.action_category_flow.apply(
-        lambda x: len([i for i in x.split(',') if not i.startswith('session-') and i != 'None']))
-    for action in ['pageview', 'download', 'outlink_click', 'buyetf_click',
-                   'brokerlink_click', 'video_action', 'form_action']:
-        df[action + 's'] = df.action_category_flow.apply(
-            lambda x: len([i for i in x.split(',') if i.endswith('_' + action)]))
-    for duration in ['visit_duration', 'action_duration',
-                     'page_duration', 'page_action_duration']:
-        df[duration] = df[duration].apply(lambda x: sum(x))
-
-    df.timestamp = df.timestamp.explode().astype(str).groupby('visitor_id').apply(
-        lambda x: ','.join(x))  # transform from list to comma separated string
-
-    # map visit flows to numerical sequences
-    maps = [
-        dict(zip(calendar.day_name, [str(i) for i in range(7)])),
-        {hr : str(i) for i, hr in enumerate(['preopening', 'early', 'core', 'late', 'None'])},
-        {dc : str(i) for i, dc in enumerate(np.sort(df.device_category.explode().unique()))},
-        {rt : str(i) for i, rt in enumerate(sorted(
-            sorted(df.referrer_type.explode().unique()), key=lambda s: s.split('_')[-1]))},
-        ]
-    cols = ['day', 'visit_trade_hours', 'device_category', 'referrer_type']
-    for i, col in enumerate(cols):
-        df[col] = df[col].apply(lambda x: ','.join(list(map(maps[i].get, x))))
-        
-    # map action and engagement flows to numerical sequences
-    action_flow = map_action_flow(df, drop_sessions=drop_sessions, drop_none=drop_none)
-    page_flow = map_action_flow(df, colstr='page', action_types=['pageview'],
-                                drop_sessions=drop_sessions, drop_none=drop_none)
-    engage_flow = map_engage_flow(df)
-
-    # drop original columns and replace with transformations
-    df = df.drop(columns=[col for col in df.columns if col in
-                          list(action_flow.columns) +
-                          list(page_flow.columns) +
-                          list(engage_flow.columns)])
-    df = pd.concat([df, action_flow, page_flow, engage_flow], axis=1)    
-
-    return df
-
-    
-# MODEL FOR ENGAGEMENT TYPES ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-def load_default_model():
-    """
-    Load visit-level engagement types model and corresponding scaler.
-
-    Returns
-    -------
-    sklearn.estimator
-        Fitted Gaussian mixture model.
-    sklearn.preprocessor
-        Fitted StandardScaler that includes feature names.
-    """
-    
-    data_path = os.path.join(pathlib.Path(__file__).parent.resolve(), "data")
-    d = '2023-04-02'
-    scaler = load(os.path.join(data_path,'gmm_scaler_{}.joblib'.format(d)))
-    clf = load(os.path.join(data_path,'gmm_{}.joblib'.format(d)))
-
-    return clf, scaler
-
-
-def get_engagement_features(scaler=None):
-    """
-    Get feature names of required for classifying visit engagement types.
-
-    Parameters
-    ----------
-    scaler : sklearn.preprocessor
-        Fitted StandardScaler with feature names.
-    
-    Returns
-    -------
-    list of str
-        List of feature names.
-    """
-
-    if scaler is None: _, scaler = load_default_model()
-
-    scaler_features = scaler.feature_names_in_.tolist()
-    bounce_features = ['visit_count',
-                       'visit_duration',
-                       'action_duration',
-                       'pages',
-                       'downloads',
-                       'brokerlinks',
-                       'video_pauses',
-                       'video_resumes',
-                       ]
-    visit_features = ['visit_id', 'date']
-    calc_features = ['articles_page_action_duration',
-                     'article-post_page_action_duration',
-                     'seconds_since_first_visit',
-                     'seconds_since_last_visit',
-                     'page_action_duration',
-                     'humankind_page_action_duration',
-                     'humankindfunds_page_action_duration',
-                     ]
-
-    return list(set(scaler_features + bounce_features + visit_features + calc_features))
-
-    
-def get_bounce_mask(df):
-    """
-    Create mask for 'new, bounce' cluster
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Visit-level data.
-
-    Returns
-    -------
-    bounce_mask : pd.Series
-        Mask for selecting the bounce visits out of the df.
-    """
-    
-    # check that the required columns are present in the dataframe
-    col = ['visit_duration',
-           'action_duration',
-           'downloads',
-           'video_resumes',
-           'brokerlinks',
-           'visit_count',
-           'pages',
-           ]
-    assert all(c in list(df) for c in col), "One or more columns are missing from df"
-    bounce_mask= (((df['visit_duration']==0) | (df['action_duration']==0)) &
-                  (df['downloads']==0) & (df['brokerlinks']==0) &
-                  (df['visit_count']==1) & (df['pages']<=1) & (df['video_resumes']==0))
-    return bounce_mask
-
-
-def get_cluster_names(date=''):
-    """
-    Provide a map between cluster ids and the names assigned to those clusters.
-
-    Parameters
-    ----------
-    date : str
-        The final date for the data set used to derive the names.
-    
-    Returns
-    -------
-    names : pd.Series
-        Series mapping engagement type numbers to names. Internal name allows
-        use as column upon merging with dataframe.
-    """
-    
-    if date== '2022-10-23':
-        names = pd.Series({
-            0: 'new, low engagement', 
-            5: 'return, 1pg, no action',
-            12: 'scrolling pgs with vids',
-            7: 'browsing home pgs',
-            19: 'ETF, brokerlinks',  # small chance brokerlink?
-            11: 'ETF, just looking',  # no vids, brokerlinks, downloads. Similar chance of seeing either home pg. 
-            17: 'return, low engagement', 
-            9: 'article reading', 
-            3: 'new, downloads',
-            8: 'browsing home pgs',
-            16: 'brokerlinks, articles',
-            1: 'video watching',
-            6: 'downloads, brokerlink',
-            13: 'new, visiting many pgs',
-            18: 'broad engagement except downloads',
-            2: 'get started form',
-            10: 'downloads, brokerlink', 
-            14: 'research and articles',
-            15: 'downloads, videos, team pg, get started',
-            4: 'downloads, videos, team pg, get started'
-            },name='engagement_type')
-    else:
-        names= pd.Series({
-            1: 'new, auto video', 
-            9: 'return, 1pg, no action',
-            0: 'browsing home pgs',
-            4: 'new, low chance of download',
-            6: 'return to advisor home and explore pages', 
-            5: 'scrolling advisor home',
-            8: 'brief return, low chance of download',
-            7: 'new, exploratory',
-            3: 'likely to click brokerlink',
-            11: 'article reading, other exploration',
-            2: 'exploratory, high chance of download',
-            10: 'broad, long engagement', 
-            },name='engagement_type')
-        
-    return names
-    
-    
-def assign_cluster(visit, scaler=None, clf=None, cluster_names=None):
-    """
-    Assign each visit to a cluster based on the trained clustering model.
-
-    Parameters
-    ----------
-    visit : pd.DataFrame
-        Visit-level data. Some features will be normalized to be used as inputs
-        for the classifier. If the dataset is too different from the original 
-        data set (from 2021-04-01 to 2022-09-20) the scaling may lead to 
-        inconsistent results from the classifier
-    scaler : sklearn.preprocessor, optional
-        Fitted StandardScaler that includes feature names. The default is the
-        most recent fitted StandardScaler.
-    clf : sklearn.estimator, optional
-        Fitted Gaussian mixture model. The default is the most recent fitted 
-        model.
-    cluster_names : pd.Series, optional.
-        A map from cluster id to name. The default is the most recent map.
-
-    Returns
-    -------
-    engagement : pd.DataFrame
-        The index is visit_id and the only column is engagement_type.
-    
-    Example
-    -------
-    assign engagement type and merge with the rest of the data:
-        engagement= analy_utils.assign_cluster(visit)
-        visit.set_index('visit_id', inplace=True)
-        visit= visit.join(engagement, how='inner')
-    """
-
-    if clf is None or scaler is None: clf, scaler = load_default_model()
-    if cluster_names is None: cluster_names = get_cluster_names('')
-        
-    #check for required features
-    if 'articles_duration' not in visit.columns:
-        #combine all article time
-        visit['articles_duration']= visit.loc[:, [
-            'articles_page_action_duration', 'article-post_page_action_duration']].sum(axis=1)
-    if 'minutes_since_last_visit' not in visit.columns:
-        #convert seconds to minutes
-        for col in ['seconds_since_first_visit', 'seconds_since_last_visit']:
-            visit['minutes_'+ col.split('_', 1)[1]]= visit[col]/60
-            
-    visit['other_page_duration']= visit['page_action_duration']- visit[
-        ['humankind_page_action_duration',
-         'humankindfunds_page_action_duration',
-         'articles_duration']].sum(axis=1)
-    #change negative values to 0
-    visit['other_page_duration']= np.where(visit['other_page_duration']<0, 0, visit['other_page_duration'])
-    
-    #check that all features are present in the input data
-    missing_features= [c for c in scaler.feature_names_in_ if c not in visit.columns]
-    assert len(missing_features)==0, f"The following features are missing from visit: {missing_features}"
-    
-    #fill null values if they exist in these columns
-    visit[scaler.feature_names_in_] = visit[scaler.feature_names_in_].fillna(0)
-    
-    #let the first cluster be the bounce cluster for non-returning visits
-    bounce_mask= get_bounce_mask(visit)
-    df_bounce= visit.loc[bounce_mask, ['visit_id','date']]
-    df_bounce['engagement_type']= "new, bounce"
-    df= visit.loc[~bounce_mask, ['visit_id'] + list(scaler.feature_names_in_)]
-    
-    #apply the preprocessor and the model
-    X= scaler.transform(df[scaler.feature_names_in_])
-    df['cluster_id']= clf.predict(X)
-    
-    #assign the names based on cluster id to the corresponding visits
-    df= df.merge(cluster_names, how='left', 
-                 left_on='cluster_id', right_index=True)
-    
-    engagement= pd.concat([df[['visit_id','engagement_type']], 
-                    df_bounce[['visit_id','engagement_type']]], 
-                   ignore_index=True, axis=0)
-    engagement.set_index('visit_id', inplace=True)
-    return engagement
-
-
-def get_cluster_grades():
-    """
-    Get the look up table for the grade and engagement score of each engagement
-    type
-
-    Returns
-    -------
-    grade : pd.DataFrame
-        1 row for each engagement type, 3 columns.
-
-    """
-    grade= pd.DataFrame([
-        ['new, low chance of download', 'A'],
-        ['likely to click brokerlink', 'A'],
-        ['return, 1pg, no action','A'],
-        ['new, exploratory', 'A'],
-        
-        ['exploratory, high chance of download', 'B+'],
-        
-        ['article reading, other exploration', 'B'], 
-        ['browsing home pgs', 'B'],
-        ['new, auto video', 'B'],
-        
-        ['brief return, low chance of download', 'C'],
-        
-        ['scrolling advisor home', 'D'],
-        ['return to advisor home and explore pages','D'], 
-        ['broad, long engagement', 'D'],
-        
-        ['new, bounce', 'F']], 
-        columns=['engagement_type','grade'])
-    
-    value= pd.DataFrame([
-        [4, 'A'],
-        [3, 'B'],
-        [3.2, 'B+'],
-        [2, 'C'],
-        [1, 'D'],
-        [0, 'F']], 
-        columns=['engagement_score','grade'])
-    grade= grade.merge(value, how='left', on='grade')
-    
-    return grade
+"""
+Analysis utility functions.
+Copyright (C) 2022 Humankind Investments.
+"""
+
+import os, sys
+from joblib import load
+import pathlib
+import re
+
+from datetime import datetime
+import calendar
+import pytz
+eastern = pytz.timezone('US/Eastern')
+
+import requests
+from bs4 import BeautifulSoup
+import json
+
+import pandas as pd
+import numpy as np
+
+from .db_utils import database_connect
+
+
+# CLEANING DUPLICATE AND SPLIT VISITS +++++++++++++++++++++++++++++++++++++++++++++++++++++++
+def drop_false_splits(df):
+    """
+    Drop false splits.
+    
+    Drop extraneous false splits, i.e. visits with duplicate visit counts per visitor
+    occurring more than thirty minutes from each other. For each set of false splits, 
+    the visit with the most activity is kept.
+    
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Dataframe of false splits.
+        
+    Returns
+    -------
+    pd.DataFrame
+        Dataframe of remaining splits after drops.
+    """
+    
+    # keep visit among false splits with longest visit duration or most actions
+    cdf = df.sort_values(by=['visit_duration', 'actions'],
+                         ascending=[False, False]).drop_duplicates(
+                             subset=['visitor_id', 'visit_count']).reset_index(drop=True)
+    
+    return cdf
+
+
+def combine_true_splits(df, dt0=True):
+    """
+    Combine true splits.
+    
+    Combine and return true split visits, i.e. visits with duplicate visit counts 
+    per visitor occurring within thirty minutes of one another.
+    
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Dataframe of true splits.
+    dt0 : bool
+        Whether delta-dt between visits is 0, indicating split visits occur at same time.
+        
+    Returns
+    -------
+    pd.DataFrame
+        Dataframe of combined splits.
+    """
+    
+    # separate columns by how data to be aggregated
+    mean_cols = [col for col in df.columns if col.split('_')[0] == 'avg']
+    sum_cols = [col for col in df.columns if col.split('_')[-1] in [
+        'actions', 'pages', 'downloads', 'outlinks', 'buyetfs', 'brokerlinks', 
+        'plays', 'pauses', 'resumes', 'seeks', 'finishes', 
+        'time', 'submissions', 'duration'] and col != 'time' and col not in mean_cols]
+    first_cols = [col for col in df.columns if col not in
+                  mean_cols + sum_cols and col.split('_')[0] not in [
+                      'first', 'last', 'entry', 'exit'] and col.split('_')[-1] not in [
+                          'flow', 'ts', 'list'] and not col.endswith('video_resolution')]
+    manual_cols = [col for col in df.columns if col not in sum_cols + mean_cols + first_cols]
+
+    # convert numeric columns to proper type
+    df[mean_cols] = df[mean_cols].astype(float)
+    
+    # combine split visits with same visitor id and visit count
+    # --> sort by visit id for split visits occurring at same time; split by datetime otherwise
+    sort_col = 'visit_id' if dt0 else 'datetime'
+    grp_cols = ['visitor_id', 'visit_count']
+    # --> also group by datetime for split visits occurring at same time
+    if dt0: grp_cols.append('datetime')
+    grp = df.sort_values(by=sort_col).groupby(grp_cols)
+    
+    # apply basic aggregates for appropriate columns (first/last, sum, mean)
+    first_grp = grp[[col for col in first_cols if col not in grp.keys]]
+    # --> pull basic visit info from last visit info in half hour window if delta-t != 0
+    first_df = first_grp.first() if dt0 else first_grp.last()
+    sum_df = grp[[col for col in sum_cols if col not in grp.keys]].sum()
+    mean_df = grp[[col for col in mean_cols if col not in grp.keys]].mean()
+    cdf = pd.concat([first_df, sum_df, mean_df], axis=1)
+
+    # combine remaining columns manually ...
+    
+    # select first and last non-empty action, and combine non-empty action flows in order
+    actgrp = df[df['first_action'] != 'None'].sort_values(by=sort_col).groupby(
+        grp_cols, group_keys=False)
+    acts_df = pd.concat([actgrp['first_action'].first(), 
+                         actgrp['last_action'].last(),
+                         actgrp['action_flow'].apply(lambda x: ','.join(x)),
+                         actgrp['action_ts'].apply(lambda x: ','.join(x)),
+                         actgrp['action_site_flow'].apply(lambda x: ','.join(x)), 
+                         actgrp['action_path_flow'].apply(lambda x: ','.join(x))], axis=1)
+    
+    # select first/last entry/exit pages, and fill in missing values based on first/last actions
+    pgs_df = pd.concat([actgrp['entry_page'].first(), actgrp['exit_page'].last()], axis=1)
+    pgs_df.loc[(pgs_df['entry_page'] == 'None') &
+               (acts_df['first_action'].str.rsplit('_', n=1).str[0].isin(
+                   ['humankind_video', 'humankind-short_video', 'getstarted_form'])),
+               'entry_page'] = 'humankind'
+    pgs_df.loc[(pgs_df['entry_page'] == 'None') &
+               ((acts_df['first_action'].str.rsplit('_', n=1).str[0].isin(
+                   ['wtf_video', 'wtf-short_video', 'buyetf'])) |
+                (acts_df['first_action'].str.split('_', n=1).str[-1].isin(
+                    ['brokerlink_click', 'download']))), 'entry_page'] = 'humankindfunds'
+    pgs_df.loc[(pgs_df['exit_page'] == 'None') &
+               (acts_df['last_action'].str.rsplit('_', n=1).str[0].isin(
+                   ['humankind_video', 'humankind-short_video', 'getstarted_form'])),
+               'exit_page'] = 'humankind'
+    pgs_df.loc[(pgs_df['exit_page'] == 'None') &
+               ((acts_df['last_action'].str.rsplit('_', n=1).str[0].isin(
+                   ['wtf_video', 'wtf-short_video', 'buyetf'])) |
+                (acts_df['last_action'].str.split('_', n=1).str[-1].isin(
+                    ['brokerlink_click', 'download']))), 'exit_page'] = 'humankindfunds'
+
+    # combine non-empty page flows
+    pggrp = df[df['page_flow'] != 'None'].sort_values(by=sort_col).groupby(
+        grp_cols, group_keys=False)
+    pgs_df = pd.concat([
+        pgs_df, pggrp['page_flow'].apply(lambda x: ','.join(x)), 
+        pggrp['page_ts'].apply(lambda x: ','.join(x))], axis=1).fillna('None')
+    
+    # combine non-empty article post and ranked company page lists
+    for pg in ['article-post', 'ranked-company']:
+        pg += '_page_list'
+        pgs_df = pd.concat([pgs_df, df[df[pg].fillna('None').replace(
+            'NaN', 'None') != 'None'].sort_values(by=sort_col).groupby(
+                grp_cols, group_keys=False)[pg].apply(
+                    lambda x: ','.join(x))], axis=1).fillna('None')
+        
+    # combine non-empty download flows
+    dlgrp = df[df['download_flow'] != 'None'].sort_values(by=sort_col).groupby(
+        grp_cols, group_keys=False)
+    dls_df = pd.concat([
+        dlgrp['download_flow'].apply(lambda x: ','.join(x)), 
+        dlgrp['download_ts'].apply(lambda x: ','.join(x))], axis=1).fillna('None')
+    
+    # combine non-empty outlink flows
+    olgrp = df[df['outlink_flow'] != 'None'].sort_values(by=sort_col).groupby(
+        grp_cols, group_keys=False)
+    ols_df = pd.concat([
+        olgrp['outlink_flow'].apply(lambda x: ','.join(x)), 
+        olgrp['outlink_ts'].apply(lambda x: ','.join(x))], axis=1).fillna('None')
+
+    # combine non-empty outlink lists
+    for ol in ['social', 'crs', 'disclosures', 'articles']:
+        ol += '_outlink_list'
+        ols_df = pd.concat([ols_df, df[df[ol].fillna('None').replace(
+            'NaN', 'None') != 'None'].sort_values(by=sort_col).groupby(
+                grp_cols, group_keys=False)[ol].apply(
+                    lambda x: ','.join(x))], axis=1).fillna('None')
+           
+    # combine non-empty buy-etf timestamps
+    etfs_df = df[df['buyetf_ts'].fillna('None').replace(
+        'NaN', 'None') != 'None'].sort_values(by=sort_col).groupby(
+            grp_cols, group_keys=False)['buyetf_ts'].apply(lambda x: ','.join(x))
+    
+    # combine non-empty broker link flows
+    brkgrp = df[df['brokerlink_flow'] != 'None'].sort_values(by=sort_col).groupby(
+        grp_cols, group_keys=False)
+    brks_df = pd.concat([
+        brkgrp['brokerlink_flow'].apply(lambda x: ','.join(x)), 
+        brkgrp['brokerlink_ts'].apply(lambda x: ','.join(x))], axis=1).fillna('None')
+    
+    # combine non-empty video flows and non-empty video resolutions
+    vidgrp = df[df['video_action_flow'] != 'None'].sort_values(by=sort_col).groupby(
+        grp_cols, group_keys=False)
+    vids_df = pd.concat([
+        vidgrp['video_action_flow'].apply(lambda x: ','.join(x)), 
+        vidgrp['video_action_ts'].apply(lambda x: ','.join(x))], axis=1).fillna('None')
+
+    # combine non-empty form flows
+    frmgrp = df[df['form_action_flow'] != 'None'].sort_values(by=sort_col).groupby(
+        grp_cols, group_keys=False)
+    frms_df = pd.concat([
+        frmgrp['form_action_flow'].apply(lambda x: ','.join(x)), 
+        frmgrp['form_action_ts'].apply(lambda x: ','.join(x))], axis=1).fillna('None')
+    
+    # combine all split visit columns
+    cdf = pd.concat([cdf, acts_df, pgs_df, dls_df, ols_df, etfs_df,
+                     brks_df, vids_df, frms_df], axis=1).fillna('None')
+    
+    # reset missing values in appropriate columns
+    cdt = cdf.index.get_level_values(2) if dt0 else cdf['datetime']
+    for pg in [col[:-1] for col in df.isnull().sum()[df.isnull().sum() > 0].index
+               if col.endswith('_pages')]:
+        cdf.loc[cdt <= df[df[pg + 's'].isnull()].sort_values(
+            by='datetime', ascending=False)['datetime'].iloc[0],
+                [col for col in cdf.columns if pg in col]] = np.nan
+    for dl in [col[:-1] for col in df.isnull().sum()[df.isnull().sum() > 0].index
+               if col.endswith('_downloads')]:
+        cdf.loc[cdt <= df[df[dl + 's'].isnull()].sort_values(
+            by='datetime', ascending=False)['datetime'].iloc[0],
+                [col for col in cdf.columns if col == dl + 's'
+                 or col == dl + '_duration']] = np.nan
+    for ol in [col[:-1] for col in df.isnull().sum()[df.isnull().sum() > 0].index
+               if col.endswith('_outlinks')]:
+        cdf.loc[cdt <= df[df[ol + 's'].isnull()].sort_values(
+            by='datetime', ascending=False)['datetime'].iloc[0],
+                [col for col in cdf.columns if ol in col]] = np.nan
+    if any(df['buyetfs'].isnull()):
+        cdf.loc[cdt <= df[df['buyetfs'].isnull()].sort_values(
+            by='datetime', ascending=False)['datetime'].iloc[0],
+                [col for col in cdf.columns if 'buyetf' in col]] = np.nan
+    for vid in [col.rsplit('_', 1)[0] for col in df.isnull().sum()[df.isnull().sum() > 0].index
+                if col.endswith('_video_plays')]:
+        cdf.loc[cdt <= df[df[vid + '_plays'].isnull()].sort_values(
+            by='datetime', ascending=False)['datetime'].iloc[0],
+                [col for col in cdf.columns if vid in col]] = np.nan
+    for frm in [col.rsplit('_', 1)[0] for col in df.isnull().sum()[df.isnull().sum() > 0].index
+                if col.endswith('_form_actions')]:
+        cdf.loc[cdt <= df[df[frm + '_actions'].isnull()].sort_values(
+            by='datetime', ascending=False)['datetime'].iloc[0],
+                [col for col in cdf.columns if frm in col]] = np.nan
+    
+    return cdf
+    
+    
+def clean_split_visits(df, true_split=True, same_time=True):
+    """
+    Clean split visits, combining true splits and dropping false splits.
+    
+    Combine true split visits, i.e. visits with duplicate visit counts per visitor 
+    occurring within thirty minutes of one another, and drop extraneous false splits,
+    i.e. visits with duplicate visit counts per visitor occurring more than thirty 
+    minutes from each other.
+    
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Dataframe of split visits.
+    true_split : bool
+        Whether split visits are true splits or false splits.
+    same_time : bool
+        Whether true splits occur at same time or different times.
+        
+    Returns
+    -------
+    pd.DataFrame
+        Cleaned dataframe of split visits.
+    """
+
+    # calculate differences in time between split visits
+    grp = df.sort_values(by='datetime').groupby(['visitor_id', 'visit_count'])
+    # --> deltadt = time between each split visit for given visitor ID and visit count
+    deltadt = grp['datetime'].apply(list).apply(
+        lambda x: [(x[i+1] - x[i]).total_seconds() for i in range(len(x)-1)]).rename('deltadt')
+    # --> visit_id_pairs = split visit pairs for which delta-dt calculated
+    visit_id_pairs = grp['visit_id'].unique().apply(
+        lambda x: [(x[i], x[i+1]) for i in range(len(x)-1)] if len(x) > 1 else
+        [(x[0], x[0])]).rename('visit_id_pairs')
+    split_dt = pd.concat([deltadt, visit_id_pairs], axis=1)
+    
+    # filter out split visits already cleaned (no duplicates)
+    split_mask = split_dt['deltadt'].str.len() > 0
+    split_dt = pd.concat([split_dt[split_mask]['deltadt'].explode(),
+                          split_dt[split_mask]['visit_id_pairs'].explode()], axis=1)
+    
+    # sum up total delta-dt for true splits occurring at different times or false splits
+    if not true_split or not same_time:
+        split_dt = pd.concat([
+            split_dt.reset_index().groupby(['visitor_id', 'visit_count'])['deltadt'].sum(),
+            split_dt['visit_id_pairs'].apply(
+                lambda x: list(x)).explode().drop_duplicates().reset_index().groupby([
+                    'visitor_id', 'visit_count'])['visit_id_pairs'].unique()], axis=1)
+    # set delta-dt thresholds for selecting split visits of given type
+    if true_split:
+        deltadt_mask = split_dt['deltadt'] == 0 if same_time else split_dt['deltadt'] < 1800
+    else:
+        deltadt_mask = split_dt['deltadt'] >= 1800
+    # isolate split visits of given type
+    split_ids = split_dt[deltadt_mask]['visit_id_pairs'].apply(
+        lambda x: list(x)).explode().drop_duplicates()
+    split_visits = df[df['visit_id'].isin(split_ids)].reset_index(drop=True)
+    
+    # combine true splits or drop false splits
+    if true_split: clean_splits = combine_true_splits(split_visits, same_time).reset_index()
+    else: clean_splits = drop_false_splits(split_visits)
+
+    # drop split visits of given type, and add newly cleaned split visits
+    df = df.drop(df.loc[df['visit_id'].isin(split_visits['visit_id'])].index)
+    df = pd.concat([df, clean_splits]).sort_values(by='visit_id').reset_index(drop=True)
+    
+    return df
+
+
+def get_split_visits(df):
+    """
+    Get split visits from visit-level data.
+    
+    Identify and return all split visits from visit-level data set, where split visits
+    are those with duplicate visit counts per visitor.
+    
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Dataframe of visits.
+    
+    Returns
+    -------
+    pd.DataFrame
+        Dataframe of split visits.
+    """
+
+    # count number of visit IDs associated with each visitor ID - visit count pair
+    visit_count = df.groupby(['visitor_id', 'visit_count'])['visit_id'].count()
+    
+    # isolate visitor ID - visit count pairs with multiple visit IDs
+    dupl_visit_count = visit_count[visit_count > 1]
+    
+    # pull out split visits from visit-level data set
+    split_visits = df.loc[df[['visitor_id', 'visit_count']].apply(
+        tuple, axis=1).isin(dupl_visit_count.index)].reset_index(drop=True)
+    
+    return split_visits
+
+
+def clean_duplicate_visits(df):
+    """
+    Clean duplicate visits from visit-level data.
+    
+    The real-time visits logged in the visit-level data set are sometimes prone to 
+    tracking errors by Matomo that result in duplicate visits. Such duplicate visits 
+    can take the form of true duplicates, where multiple rows contain identical entries 
+    but for the visit IDs attached to them. Alternatively, duplicate visits can appear 
+    in the form of split visits, where a single visit is split into multiple entries with 
+    different visit IDs and visit metrics for the same visit count and visitor ID. 
+    When such split visits occur within a small window of time, i.e. within thirty minutes 
+    of one another, such split visits represent true splits that should be recombined into 
+    the original visits from which they were split. On the other hand, when split visits 
+    are spread across large amounts of time, i.e. hours or days, they represent false splits, 
+    or truly unique visits that Matomo erroneously attributed the same visit count to, which 
+    are cleaned by dropping all but those with the longest visit durations or most activity.
+    
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Dataframe of visits.
+    
+    Returns
+    -------
+    pd.DataFrame
+        Dataframe of visits with cleaned duplicates.
+    """
+
+    # clean action ts columns: replace '0.0' with 'None'
+    for col in [col for col in df.columns if col.endswith('_ts')]:
+        df[col] = df[col].astype(str).replace('0.0', 'None')
+
+    # DROP DUPLICATE VISITS +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+    # duplicate visits = entries with identical metrics except for visit IDs
+    df = df.drop_duplicates(subset=[col for col in df.columns if
+                                    col != 'visit_id']).reset_index(drop=True)
+
+    
+    # IDENTIFY SPLIT VISITS +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+    # split visits = visits with duplicate visit counts per visitor
+    
+    # isolate split visits to be combined or cleaned
+    split_df = get_split_visits(df)
+
+    # keep track of initial split visit IDs (for dropping later)
+    split_visit_ids = split_df['visit_id']
+
+    # drop split visits with no actions (no use in combining these if nothing to combine)
+    split_df = split_df.drop(split_df[split_df['actions'] == 0].index).reset_index(drop=True)
+
+    # add datetime column
+    split_df['datetime'] = pd.to_datetime(split_df['date'].astype(str) + ' ' + split_df['time'])
+    
+    # COMBINE SAME-TIME TRUE SPLITS +++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+    # same-time true splits = split visits occurring at exact same time
+    if not split_df.empty:
+        split_df = clean_split_visits(split_df, true_split=True, same_time=True)
+    
+    # COMBINE DIFFERENT-TIME TRUE SPLITS ++++++++++++++++++++++++++++++++++++++++++++++++++++
+    # different-time true splits = split visits occurring within 30 minutes of one another
+    if not split_df.empty:
+        split_df = clean_split_visits(split_df, true_split=True, same_time=False)
+    
+    # CLEAN FALSE SPLITS ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+    # false splits = split visits occurring more than 30 minutes from each other
+    if not split_df.empty:
+        split_df = clean_split_visits(split_df, true_split=False)
+    
+    # DROP SPLIT VISITS AND REPLACE WITH CLEANED SPLITS +++++++++++++++++++++++++++++++++++++
+    df = df.drop(df[df['visit_id'].isin(split_visit_ids)].index)
+    df = pd.concat([df, split_df.drop(columns='datetime')],
+                   ignore_index=True).sort_values(by='visit_id').reset_index(drop=True)
+
+    # drop remaining duplicate visits, if any
+    df = df.drop(df[df.duplicated(subset='visit_id')].index).reset_index(drop=True)
+    
+    return df
+
+
+# CLEANING ATYPICAL VISITS ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+def drop_hki(df, db_dict):
+    """
+    Drop visits from Humankind employees and third-party vendors.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Visit-level data.
+    db_dict : dict
+        Dictionary of database credentials.
+    """
+
+    # DROP HUMANKIND EMPLOYEE VISITS ++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+
+    # read in ip addresses and locations of humankind employees
+    cursor, conn = database_connect('hkisocial', db_dict)
+    query = """SELECT * FROM ips ORDER BY name, description, start_date"""
+    ips = pd.read_sql(query, conn)
+    ips.ip = ips.ip.str.rsplit('.', n=2).str[0] + '.0.0'  # anonymize ips
+    cursor.close()
+    conn.close()
+
+    # merge with visits of same ips and locations
+    ip_grp = ips.groupby(['name', 'description', 'ip', 'city', 'region', 'country'])
+    vis_grp = df.groupby(['ip', 'city', 'region', 'country', 'date'])
+    ipvis = pd.merge(pd.concat([ip_grp.start_date.first(),
+                                ip_grp.end_date.last().fillna('9999-99-99')],
+                               axis=1).droplevel(['name', 'description']).reset_index(),
+                     vis_grp.visit_id.unique().reset_index(), how='left',
+                     on=['ip', 'city', 'region', 'country'])
+
+    # isolate visits with select ip-locations within relevant date ranges
+    ipvis = ipvis.drop(ipvis[(ipvis.date.astype(str) < ipvis.start_date) |
+                             (ipvis.date.astype(str) > ipvis.end_date)].index)
+    hki_visits = ipvis.visit_id.explode().tolist()
+
+    # isolate visitors with offending visits
+    hki_visitors = df[(df.referrer_type != 'campaign') &  # exclude campaign referrals
+                      (df.visit_id.isin(hki_visits))].visitor_id.tolist()
+
+    # drop non-campaign referral entries from humankind employees
+    df.drop(df[(df.visitor_id.isin(hki_visitors))].index, inplace=True)
+
+    # DROP VENDORS ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+
+    # drop yellow.system visitors
+    ys_visits = df[df.country.isin(['Belarus', 'Armenia', 'Georgia'])].visit_id.tolist()
+    ys_visitors = df[df.visit_id.isin(ys_visits)].visitor_id.tolist()
+    df.drop(df[(df.visitor_id.isin(ys_visitors))].index, inplace=True)
+    df.reset_index(drop=True, inplace=True)
+
+
+def drop_dev(df, db_dict):
+    """
+    Drop visitors with any visits to the dev sites.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Visit-level data.
+    db_dict : dict
+        Dictionary of database credentials.
+    """
+
+    # get list of unique visitors to dev sites from action log
+    cursor, conn = database_connect('hkiweb', db_dict)
+    query = """SELECT distinct visitor_id
+                 FROM action_log
+                WHERE split_part(regexp_replace(url, '(https?://)?(www.)?', ''), '/', 1)
+               NOT IN ('humankind.co', 'humankindfunds.com', 'rankings.humankind.co')
+            """
+    dev = pd.read_sql(query, conn)
+    cursor.close()
+    conn.close()
+
+    # drop dev-site visitors
+    df.drop(df[df.visitor_id.isin(dev.visitor_id)].index, inplace=True)
+    df.reset_index(drop=True, inplace=True)
+
+
+def drop_foreign(df):
+    """
+    Drop foreign visitors.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Visit-level data.
+    """
+
+    # count number of domestic and foreign visits per visitor
+    domestic = df.groupby('visitor_id').country.apply(
+        lambda x: [i for i in x if i == 'United States']).rename('domestic')
+    foreign = df.groupby('visitor_id').country.apply(
+        lambda x: [i for i in x if i != 'United States']).rename('foreign')
+
+    # count visitors with more foreign than domestic visits as foreign
+    foreign_visitors = foreign[foreign.str.len() > domestic.str.len()].index
+
+    # drop foreign visitors
+    df.drop(df[df.visitor_id.isin(foreign_visitors)].index, inplace=True)
+    df.reset_index(drop=True, inplace=True)
+
+
+# CLEANING ACTION FLOWS +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+def clean_flow(df, action_type, actions, deltat=0):
+    """
+    Clean action flows for individual action type.
+
+    Remove duplicate actions, i.e. consecutive actions of same type occurring
+    within given time range, from action flows. Update action flow, timestamp, 
+    count, and average duration columns with duplicate actions removed.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Dataframe of website visits.
+    action_type : str
+        Type of action for which to clean flows. Valid options are 'pageview',
+        'download', 'outlink_click', 'buyetf_click', 'brokerlink_click', 'video_action',
+        and 'form_action'. An invalid action flow will cause the
+        function to return without making any modifications to the dataframe.
+    actions : pd.DataFrame
+        Dataframe of individual actions of all type over all visits.
+    deltat : int
+        Maximum time difference, in seconds, between consecutive actions for which to 
+        apply cleaning. Consecutive actions occurring within delta-t seconds of one 
+        another will be cleaned, with the latter of the two being removed from the action flow. 
+        Default of 0 cleans consecutive actions occurring at exactly the same time only.
+    """
+
+    # exit if action type not valid option
+    if action_type not in ['pageview',
+                           'download',
+                           'outlink_click',
+                           'buyetf_click',
+                           'brokerlink_click',
+                           'video_action',
+                           'form_action',
+                          ]: return df
+
+    # get action string
+    action_str = action_type
+    if action_type == 'pageview': action_str = 'page'
+    elif action_type.split('_')[-1] == 'click': action_str = action_type.split('_')[0]
+
+    # get individual actions and timestamps of given type per visit
+    acts_mask = (actions.action_flow.str.endswith('_' + action_type))
+    if action_type == 'buyetf_click':
+        acts_mask = (actions.action_flow == 'buyetf_click')
+    elif action_type.split('_')[-1] == 'action':
+        acts_mask = (actions.action_flow.str.split('_', n=1).str[-1].str.split('_').str[0] ==
+                     action_type.split('_')[0])  # *_video/form_*
+    acts = actions[acts_mask].rename(
+        columns={col : col.replace('action', action_str) for col in actions.columns})
+    acts[action_str + '_flow'] = acts[action_str + '_flow'].replace(
+        '_' + action_type, '', regex=True)
+
+    # find duplicate actions of given type and update action type flow/ts columns
+    dupl_mask = ((actions.visit_id == actions.visit_id.shift()) &  # same visit id
+                 (actions.action_flow == actions.action_flow.shift()) &  # same action 
+                 (actions.action_ts_int - actions.action_ts_int.shift() <= deltat)  # time in range
+                )        
+    dupl_acts = actions.loc[dupl_mask & acts_mask]
+    act_grp = acts.drop(dupl_acts.index).groupby('visit_id', group_keys=False)
+    flow_cols = [action_str + '_ts']
+    if action_type != 'buyetf_click': flow_cols = [action_str + '_flow'] + flow_cols
+    for col in flow_cols:
+        df[col] = act_grp[col].apply(lambda x: ','.join(x))
+        df[col] = df[col].fillna('None')
+
+    # update action type counts and average durations
+    df[action_str + 's'] = df[action_str + '_ts'].apply(
+        lambda x: 0 if x == 'None' else len(x.split(',')))
+    if action_type != 'form_action':
+        if action_type != 'pageview':  # modify page action duration instead
+            df[action_str + '_duration'] = act_grp[action_str + '_duration'].sum()
+            df[action_str + '_duration'] = df[action_str + '_duration'].fillna(0).astype(int)
+        df['avg_' + action_str + '_duration'] = (df[action_str + '_duration'] /
+                                                 df[action_str + 's']).fillna(0)
+    if action_type == 'pageview':
+        df.page_action_duration = act_grp[action_str + '_duration'].sum()
+        df.page_action_duration = df.page_action_duration.fillna(0).astype(int)
+        df.avg_page_action_duration = (df.page_action_duration / df.pages).fillna(0)
+    elif action_type == 'form_action':
+        df.avg_form_interaction_time = (df.form_interaction_time / df.form_actions).fillna(0)
+
+    # update individual action type counts: subtract duplicate actions from corresponding columns
+    dupl_acts = dupl_acts.drop(columns=['action_path_flow', 'action_ts'])
+    if action_type == 'buyetf_click': return  # no further columns to update
+    elif action_type.split('_')[-1] != 'action':
+        dupl_acts.action_flow = dupl_acts.action_flow.str.replace(action_type, action_str + 's')
+        if action_type == 'pageview':  # combine individual article post / company ranking pages
+            dupl_acts.action_flow = dupl_acts.action_flow.apply(
+                lambda x: re.sub('articles-.*_pages', 'article-post_pages', x)).apply(
+                lambda x: re.sub('rankings-.*_pages', 'ranked-company_pages', x))
+            dupl_acts.action_flow = np.select(  # map socially responsible pages to site homepages
+                [(dupl_acts.action_flow == 'socially_responsible_pages') &
+                 (dupl_acts.action_site_flow == 'humankind.co'),
+                 (dupl_acts.action_flow == 'socially_responsible_pages') &
+                 (dupl_acts.action_site_flow == 'humankindfunds.com')],
+                ['humankind_pages', 'humankindfunds_pages'], default=dupl_acts.action_flow)
+            dupl_acts = dupl_acts.loc[dupl_acts.action_flow != 'page-not-found_pages']
+        elif action_type == 'outlink_click':  # combine categories of outlinks
+            dupl_acts.action_flow = dupl_acts.action_flow.apply(
+                lambda x: re.sub('(linkedin|instagram|youtube|facebook|twitter)_outlinks',
+                                 'social_outlinks', x)).apply(
+                lambda x: re.sub('(investor|adviserinfo.sec)_outlinks', 'crs_outlinks', x)).apply(
+                lambda x: re.sub('(finra|sipc)_outlinks', 'disclosures_outlinks', x))
+            # drop article outlinks: no good way to track this category
+            df.drop(columns = [col for col in df.columns if
+                               col.startswith('articles_outlink')], inplace=True)
+        actcols = [col for col in df.columns if col.endswith('_' + action_str + 's')]
+        dupl_actcts = dupl_acts.groupby('visit_id').action_flow.apply(lambda x: [i for i in x])
+        dupl_actcts = pd.concat([dupl_actcts, pd.DataFrame(columns=actcols)], axis=1).fillna(0)
+        for col in actcols:
+            dupl_actcts[col] = dupl_actcts.action_flow.apply(
+                lambda x: len([i for i in x if i == col]))
+            df.loc[df.index.isin(dupl_actcts.index), col] = df[col] - dupl_actcts[col]
+            df[col] = df[col].astype(float)
+    else:  # handle video and form actions separately
+        actpre = action_type.split('_')[0]
+        if actpre == 'video': subs = ['play', 'pause', 'resume', 'seek', 'finish']
+        elif actpre == 'form': subs = ['submission']
+        subs = [actpre + '_' + i for i in subs]
+        subcols = [col for col in df.columns for i in subs if
+                   col == (i + 'es' if i.endswith('sh') else i + 's')]
+        actcols = [col for col in df.columns for i in subcols if col.endswith('_' + i)]
+        for icol, col in enumerate(subcols):
+            dupl_acts.action_flow = dupl_acts.action_flow.str.replace(subs[icol], col)
+        dupl_actcts = dupl_acts.groupby(
+            'visit_id', group_keys=False).action_flow.apply(lambda x: [i for i in x])
+        dupl_actcts = pd.concat(
+            [dupl_actcts, pd.DataFrame(columns=subcols+actcols)], axis=1).fillna(0)
+        for col in subcols:  # duplicate total subactions
+            dupl_actcts[col] = dupl_actcts.action_flow.apply(
+                lambda x: len([i for i in x if i.endswith('_' + col)]))
+        for col in actcols:  # duplicate subactions by video/form
+            dupl_actcts[col] = dupl_actcts.action_flow.apply(
+                lambda x: len([i for i in x if i == col]))
+        for col in subcols + actcols:
+            df.loc[df.index.isin(dupl_actcts.index), col] = df[col] - dupl_actcts[col]
+            df[col] = df[col].astype(float)
+        if actpre == 'video':  # update average video columns
+            df.avg_video_watch_time = (df.video_watch_time / df.video_plays).replace(
+                np.inf, 0).fillna(0)
+
+        
+def clean_action_flows(df, deltat=0):
+    """
+    Clean action flows.
+
+    Remove duplicate actions, i.e. consecutive actions of same type occurring at
+    once, from action flows. Update action flow, timestamp, count, and average
+    duration columns for total and individual action types with duplicate actions removed.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Dataframe of website visits.
+
+    Returns
+    -------
+    pd.DataFrame
+        Dataframe of website visits with cleaned action flows.
+    deltat : int
+        Maximum time difference, in seconds, between consecutive actions for which to 
+        apply cleaning. Consecutive actions occurring within delta-t seconds of one 
+        another will be cleaned, with the latter of the two being removed from the action flow. 
+        Default of 0 cleans consecutive actions occurring at exactly the same time only.
+    """
+
+    # set visit id as index
+    df.set_index('visit_id', inplace=True)
+
+    # clean action ts columns: replace '0.0' with 'None'
+    for col in [col for col in df.columns if col.endswith('_ts')]:
+        df[col] = df[col].replace('0.0', 'None')
+
+    # clean up action path flow --> remove split entries for page-not-found pageviews
+    bad_flows = df[df.action_flow.str.split(',').str.len() !=
+                   df.action_path_flow.str.split(',').str.len()].action_path_flow
+    df.loc[df.index.isin(bad_flows.index),
+           'action_path_flow'] = bad_flows.str.rstrip(',').apply(
+        lambda x: ','.join([i for i in x.split(',') if not
+                            i.startswith('<svg') and i not in ['/)', "'"]]))
+
+    # get individual actions and timestamps per visit
+    actions = pd.concat([df.action_flow.apply(lambda x: x.split(',')).explode(),
+                         df.action_site_flow.apply(lambda x: x.split(',')).explode(),
+                         df.action_path_flow.apply(lambda x: x.split(',')).explode(),
+                         df.action_ts.apply(lambda x: x.split(',')).explode(),
+                         ], axis=1).sort_values(by=['visit_id', 'action_ts']).reset_index()
+    actions['action_ts_int'] = actions.action_ts.fillna('None').replace('None', '0').astype(int)
+
+    # find duplicate actions (consecutive same actions within time range) and update flow/ts columns
+    dupl_mask = (
+        (actions.visit_id == actions.visit_id.shift()) &  # same visit id
+        (actions.action_flow == actions.action_flow.shift()) &  # same action
+        (actions.action_ts_int - actions.action_ts_int.shift() <= deltat)  # timestamps in range
+        )
+    act_clean = actions.drop(actions.loc[dupl_mask].index)
+    act_clean['action_duration'] = act_clean.groupby(
+        'visit_id').action_ts_int.diff(1).shift(-1).abs()
+    actions['action_duration'] = act_clean['action_duration']
+    act_grp = act_clean.groupby('visit_id')
+    for col in ['action_flow', 'action_site_flow', 'action_path_flow', 'action_ts']:
+        df[col] = act_grp[col].apply(lambda x: ','.join(x))
+
+    # update action count, action duration, and average duration columns
+    df.actions = df.action_flow.apply(lambda x: 0 if x == 'None' else len(x.split(',')))
+    df.action_duration = act_grp.action_duration.sum()
+    df.action_duration = df.action_duration.fillna(0).astype(int)
+    df.avg_action_duration = (df.action_duration / df.actions).fillna(0)
+
+    # clean individual action type flows
+    for action_type in ['pageview',
+                        'download',
+                        'outlink_click',
+                        'buyetf_click',
+                        'brokerlink_click',
+                        'video_action',
+                        'form_action',
+                        ]: clean_flow(df, action_type, actions, deltat)
+
+    # reset index
+    df.reset_index(inplace=True)
+
+
+def clean_standalone_action(df, action_type, deltat=0):
+    """
+    Clean individual action type flow and update overall action flow.
+
+    Remove duplicate actions of given type, i.e. consecutive actions occurring 
+    within given time range, from overall and specific action flows. 
+    Update action flow, timestamp, count, and average duration columns with 
+    duplicate actions removed.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Dataframe of website visits.
+    action_type : str
+        Type of action for which to clean flows. Valid options are 'pageview',
+        'download', 'outlink_click', 'buyetf_click', 'brokerlink_click', 
+        'video_action', and 'form_action'. An invalid action flow will cause the
+        function to return without making any modifications to the dataframe.
+    deltat : int
+        Maximum time difference, in seconds, between consecutive actions for which to 
+        apply cleaning. Consecutive actions occurring within delta-t seconds of one 
+        another will be cleaned, with the latter of the two being removed from the action flow. 
+        Default of 0 cleans consecutive actions occurring at exactly the same time only.
+    """
+
+    # set visit id as index
+    df.set_index('visit_id', inplace=True)
+    
+    # get individual actions and timestamps per visit
+    actions = pd.concat([df.action_flow.apply(lambda x: x.split(',')).explode(),
+                         df.action_site_flow.apply(lambda x: x.split(',')).explode(),
+                         df.action_path_flow.apply(lambda x: x.split(',')).explode(),
+                         df.action_ts.apply(lambda x: x.split(',')).explode(),
+                         ], axis=1).sort_values(by=['visit_id', 'action_ts']).reset_index()
+    actions['action_ts_int'] = actions.action_ts.fillna('None').replace('None', '0').astype(int)
+    
+    # get individual actions and timestamps of given type per visit
+    acts_mask = (actions.action_flow.str.endswith('_' + action_type))
+    if action_type == 'buyetf_click':
+        acts_mask = (actions.action_flow == 'buyetf_click')
+    elif action_type.split('_')[-1] == 'action':
+        acts_mask = (actions.action_flow.str.split('_', n=1).str[-1].str.split('_').str[0] ==
+                     action_type.split('_')[0])  # *_video/form_*
+    
+    # find duplicate actions (consecutive same actions within time range) and update flow/ts columns
+    dupl_mask = (
+        (actions.visit_id == actions.visit_id.shift()) &  # same visit id
+        (actions.action_flow == actions.action_flow.shift()) &  # same action
+        (actions.action_ts_int - actions.action_ts_int.shift() <= deltat)  # timestamps in range
+        )
+    # drop duplicate actions of given type
+    act_clean = actions.drop(actions.loc[dupl_mask & acts_mask].index)
+    act_clean['action_duration'] = act_clean.groupby(
+        'visit_id').action_ts_int.diff(1).shift(-1).abs()
+    actions['action_duration'] = act_clean['action_duration']
+    act_grp = act_clean.groupby('visit_id')
+    for col in ['action_flow', 'action_site_flow', 'action_path_flow', 'action_ts']:
+        df[col] = act_grp[col].apply(lambda x: ','.join(x))
+
+    # update action count, action duration, and average duration columns
+    df.actions = df.action_flow.apply(lambda x: 0 if x == 'None' else len(x.split(',')))
+    df.action_duration = act_grp.action_duration.sum()
+    df.action_duration = df.action_duration.fillna(0).astype(int)
+    df.avg_action_duration = (df.action_duration / df.actions).fillna(0)
+    
+    # clean individual action type flow
+    clean_flow(df, action_type, actions, deltat)
+    
+    # reset index
+    df.reset_index(inplace=True)
+    
+
+
+# VISITOR-LEVEL DATA ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+def categorize_visitor_action_flow(df):
+    """
+    Categorize visitor-level action flows - map specific actions to categories.
+    
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Raw visitor-level data.
+    """
+    
+    # separate actions
+    adf = df.action_flow.str.split(',').explode()
+    
+    # map actions to categories
+    subs = {r'^(.*)_socially_responsible_pageview$' :
+            r'\1_pageview',
+            r'^articles-.*_pageview$' :
+            'articles-post_pageview',
+            r'^rankings_.*_pageview$' :
+            'rankings_pageview',
+            r'^rankings-.*_pageview$' :
+            'rankings-company_pageview',
+            r'^.*\.(jpg|png|eps)_download$' :
+            'logo_download',
+            r'^(linkedin|youtube|twitter|instagram|facebook)_outlink_click$' :
+            'social_outlink_click',
+            r'^(adviserinfo\.sec|sipc|finra|investor)_outlink_click$' :
+            'compliance_outlink_click',
+            r'^(theconversation|benefitcorporationreduced|onlinelibrary\.wiley)_outlink_click$' :
+            'articles_outlink_click',
+            r'^(.*)_video_.*$' :
+            r'\1_video_action',
+            r'^(.*)_form_.*$' :
+            r'\1_form_action',
+           }
+    for sub in subs.items():
+        adf = adf.apply(lambda x: re.sub(r'^{}$'.format(sub[0]), sub[1], x))
+        
+    # regroup actions and insert new categorical column into dataframe
+    adf = adf.groupby('visitor_id').apply(lambda x: ','.join(x))
+    df.insert(df.columns.get_loc('action_flow')+1, 'action_category_flow', adf)
+
+
+def clean_visitor_action_flow(df):
+    """
+    Clean raw visitor-level action flows - map extraneous actions.
+    
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Raw visitor-level data.
+    """
+    
+    # build dataframe of individual actions
+    adf = pd.concat([df.action_flow.str.split(',').explode(), 
+                     df.action_site_flow.str.split(',').explode(),
+                     df.action_ts.str.split(',').explode(),
+                    ], axis=1)
+
+    # map socially responsible pages to proper homepages
+    srpg = 'socially_responsible_pageview'
+    for site in ['humankind.co', 'humankindfunds.com']:
+        adf.loc[(adf.action_flow == srpg) & (adf.action_site_flow == site),
+                'action_flow'] = site.split('.')[0] + '_' + srpg
+
+    # map original rankings company pages to corresponding year
+    adf.action_flow = np.where((adf.action_flow.str.startswith('rankings-')) &
+                               (adf.action_flow.str.endswith('_pageview')),
+                               adf.action_flow.str.replace('_pageview', '-2022_pageview'),
+                               adf.action_flow)
+        
+    # map article post and rankings company pageviews with bad urls to page-not-found
+    fpats = ['^articles-', '^rankings-']
+    bpat = '_pageview$'
+    for fpat in fpats:
+        pgmask = (adf.action_flow.apply(lambda x: bool(re.match(r'{}.*{}'.format(fpat, bpat), x))))
+        if fpat[1:-1] == 'articles':
+            patmask = (~(adf.action_flow.apply(lambda x: bool(
+                re.match(r'({}(?=.*?\-)[a-z0-9\-]*{})'.format(fpat, bpat), x)))) |
+                       (adf.action_flow.apply(lambda x: bool(
+                           re.match(r'({}frame-[a-z0-9]*{})'.format(fpat, bpat), x)))))
+        elif fpat[1:-1] == 'rankings':
+            patmask = ~(adf.action_flow.apply(
+                lambda x: '-' in re.sub(r'-[\d]{4}', '', x.replace('rankings-', ''))))
+        adf.loc[pgmask & patmask, 'action_flow'] = 'page-not-found_pageview'
+        
+    # map article link downloads to outlink clicks
+    link_dls = ['benefitcorporationreduced']
+    for link_dl in link_dls:
+        adf.loc[adf.action_flow == '{}_download'.format(link_dl),
+                'action_flow'] = '{}_outlink_click'.format(link_dl)
+        
+    df.action_flow = adf.groupby('visitor_id').action_flow.apply(lambda x: ','.join(x))
+    
+    
+def build_raw_visitor_data(vdf):
+    """
+    Build raw visitor-level data set.
+
+    Raw visitor data = time-ordered list of visits and activities across customer lifetime.
+    
+    Parameters
+    ----------
+    vdf : pd.DataFrame
+        Raw visit-level data.
+
+    Returns
+    -------
+    pd.DataFrame
+        Raw visitor-level data.
+    """
+
+    # initialize dataframe
+    df = pd.DataFrame()
+
+    # copy input dataframe (avoid modifying original)
+    vdf = vdf.copy()
+
+    # add necessary columns to input dataframe
+    vdf['datetime'] = vdf.date.astype(str) + ' ' + vdf.time
+    vdf['timestamp'] = vdf.datetime.apply(lambda x: eastern.localize(
+        datetime.strptime(x, '%Y-%m-%d %H:%M:%S')).timestamp()).astype(int)
+    vdf['bounce'] = (vdf.visit_duration == 0).astype(int)
+    vdf['true_bounce'] = ((vdf.visit_duration == 0) &
+                          (vdf.actions - vdf.pages == 0) & (vdf.pages < 2)).astype(int)
+    vdf['mobile'] = (vdf.device_category == 'mobile').astype(int)
+    vdf['desktop'] = (vdf.device_category == 'desktop').astype(int)
+    dict_cols = {'location' : ['city', 'region', 'country', 'continent'],
+                 'campaign' : [col for col in vdf.columns if col.startswith('campaign')]}
+    for out_col, in_cols in dict_cols.items():
+        vdf[out_col] = vdf[in_cols].apply(lambda x: ','.join(x), axis=1)
+        vdf[out_col] = vdf[out_col].apply(
+            lambda x: {in_cols[i] : x.split(',')[i] for i in range(len(in_cols))})
+    
+    # add engagement types
+    if 'engagement_type' not in vdf.columns:
+        visit_engagement = assign_cluster(vdf).reset_index()
+        vdf = vdf.merge(visit_engagement, how='left', on='visit_id')
+    vdf['engagement_type'] = vdf.engagement_type.str.replace(',', '').str.replace(' ', '_')
+    
+    # modify flow columns in input dataframe to include session starts/ends
+    flows = ['action', 'action_site', 'page']
+    for flow in flows:
+        vdf[flow + '_flow'] = 'session-start,' + vdf[flow + '_flow'] + ',session-end'
+    for flow in [flow for flow in flows if flow != 'action_site']:
+        vdf[flow + '_ts'] = '0,' + vdf[flow + '_ts'] + ',1'
+    
+    # group by visitor id in order of visit
+    grp = vdf.sort_values(by='visit_id').groupby('visitor_id')
+
+    # visitor lifetime
+    df['datetime'] = grp.datetime.agg(list)
+    df['timestamp'] = grp.timestamp.agg(list)
+    df['day'] = grp.day.agg(list)
+    df['visit_trade_hours'] = grp.visit_trade_hours.agg(list)
+    
+    # visits
+    df['visits'] = grp.visit_count.max()
+    df['visit_count'] = grp.visit_count.agg(list)
+    df['visit_id'] = grp.visit_id.agg(list)
+    df['visit_duration'] = grp.visit_duration.agg(list)
+    
+    # bounce rates
+    df['bounce'] = grp.bounce.agg(list)
+    df['bounce_rate'] = grp.bounce.sum().div(df.visits)
+    df['true_bounce'] = grp.true_bounce.agg(list)
+    df['true_bounce_rate'] = grp.true_bounce.sum().div(df.visits)
+
+    # devices
+    df['device_category'] = grp.device_category.agg(list)
+    df['mobile_desktop_ratio'] = grp.mobile.sum().div(grp.desktop.sum()).replace(np.inf, 0)
+    
+    # locations
+    df['location'] = grp.location.agg(list)
+    
+    # referrals
+    df['referrer_type'] = grp.referrer_subtype.agg(list)
+    df['referrer_website'] = grp.referrer_website_url.agg(list)
+    df['referrer_social_network'] = grp.referrer_social_network_name.agg(list)
+    df['referrer_search_engine'] = grp.referrer_search_engine_name.agg(list)
+    df['referrer_search_engine_keyword'] = grp.referrer_search_engine_keyword.agg(list)
+    df['campaign'] = grp.campaign.agg(list)
+
+    # actions
+    df['actions'] = grp.actions.agg(list)
+    df['action_duration'] = grp.action_duration.agg(list)
+    df['page_duration'] = grp.page_duration.agg(list)
+    df['page_action_duration'] = grp.page_action_duration.agg(list)
+    df['action_flow'] = grp.action_flow.apply(lambda x: ','.join(x))
+    df['action_site_flow'] = grp.action_site_flow.apply(lambda x: ','.join(x))
+    df['action_ts'] = grp.action_ts.apply(lambda x: ','.join(x))
+        
+    # engagement types
+    df['engagement_flow'] = grp.engagement_type.apply(lambda x: ','.join(x))
+
+    # clean and categorize action flows
+    clean_visitor_action_flow(df)
+    categorize_visitor_action_flow(df)
+    
+    return df
+
+
+def get_asset_urls(url, urls):
+    """
+    Get URLs of all assets on advisor site.
+    
+    Parameters
+    ----------
+    url : str
+        Main assets page URL.
+    urls : list of str
+        List of assets urls. This list is changed in place.
+    """
+    
+    # recursively loop through assets folders to get urls
+    response = requests.request('GET', url)
+    content = response.content
+    soup = BeautifulSoup(content, 'html.parser')
+    divs = soup.find_all('div', class_=re.compile('assets_folder__[a-zA-Z0-9]*'))
+    for div in divs:
+        links = div.find_all('a')
+        for link in links:
+            new_url = os.path.join(url, link.string)
+            urls.append(new_url)
+            get_asset_urls(new_url, urls)
+
+
+def get_action_category_map():
+    """
+    Build numerical mapping for categorical action flows.
+    
+    Returns
+    -------
+    dict of {str : int}
+        Dictionary mapping categorical actions to integers.
+    """
+    
+    # replace hardcoding for some actions, i.e. downloads, brokerlinks, with site scraping (?)
+    action_dict = {
+        'pageview' : ['humankind', 'mission', 'research', 'team', 'articles',
+                      'articles-post', 'rankings', 'rankings-company', 'humankindfunds',
+                      'etf-explanation', 'topcompanies', 'shareholders', 'tax-information',
+                      'investors', 'contact', 'relationship', 'terms', 'page-not-found'],
+        'download' : ['summaryprospectus', 'prospectus', 'prospectussupplement',
+                      'sai', 'methodology', 'factsheet', 'premiumdiscountchart',
+                      'quarterlyreport', 'semiannualreport', 'annualreport', 'benefitreport',
+                      '8937', 'holdings', 'crs', 'logo'],
+        'outlink_click' : ['social', 'compliance', 'articles'],
+        'click' : ['buyetf'],
+        'brokerlink_click' : ['robinhood', 'fidelity', 'vanguard', 'schwab',
+                              'tdameritrade', 'etrade', 'interactivebrokers'],
+        'video_action' : ['humankind-short', 'humankind', 'wtf-short', 'wtf'],
+        'form_action' : ['getstarted', 'newsletter', 'contactus', 'institutionalcontact'],
+    }
+    
+    action_list = []
+    for action_type, actions in action_dict.items(): 
+        actions = [action + '_' + action_type for action in actions]
+        for action in actions: action_list.append(action)
+    action_list += ['session-start', 'session-end', 'None']
+    
+    return {action : i for i, action in enumerate(action_list)}
+
+
+def get_action_map():
+    """
+    Build numerical mapping for full action flows.
+    
+    Returns
+    -------
+    dict of {str : int}
+        Dictionary mapping granular actions to integers.
+    """
+
+    # grab individual article posts in order of appearance on site
+    url = 'https://www.humankind.co/articles'
+    response = requests.request('GET', url)
+    content = response.content
+    soup = BeautifulSoup(content, 'html.parser')
+    article_list = []
+    for link in soup.find_all('a'):
+        href = link.get('href').strip('/')
+        if href.startswith('articles/') and not link.get('class'):
+            article_list.append(href.replace('/', '-') + '_pageview')
+    
+    # grab individual company rankings in order of rank and year on site
+    url = 'https://rankings.humankind.co/{}'
+    year_list = [str(i) for i in range(2022, int(datetime.now().year)+1)]
+    year_list = [''] + year_list  # temporary --> remove empty string when rankings site migrated
+    ranking_list = []
+    for year in year_list:
+        year_url = url.format(year)
+        response = requests.request('GET', year_url)
+        content = response.content
+        soup = BeautifulSoup(content, 'html.parser')
+        data = soup.find_all('script', id='__NEXT_DATA__')[0].contents[0]
+        data = json.loads(data)
+        if 'companies' in data['props']['pageProps']:
+            # --> remove condition below after site update
+            if year != '': ranking_list.append('rankings_' + year + '_pageview')
+            for company in data['props']['pageProps']['companies']['items']:
+                ranking_list.append('rankings-' + company['slug'] + '_pageview')
+    # --> temporary until site updated...
+    ranking_list = [ranking.replace('_pageview', '-2022_pageview') for
+                    ranking in ranking_list if ranking.startswith('rankings')]
+
+    # grab individual logo downloads in order of appearance on site
+    url = 'https://www.humankind.co/assets'
+    asset_urls = []
+    get_asset_urls(url, asset_urls)
+    logo_list = []
+    for url in asset_urls:
+        response = requests.request('GET', url)
+        content = response.content
+        soup = BeautifulSoup(content, 'html.parser')
+        for link in soup.find_all('a'): 
+            href = link.get('href')
+            if not href: continue
+            href = href.strip('/')
+            if href.startswith('assets'): logo_list.append(re.sub(
+                    r'(hknd|humankind|[\d_%]+)', '', href.split('/')[-1].lower()) + '_download')
+
+    # expand individual social and compliance outlinks
+    outlink_list = ['facebook', 'twitter', 'instagram', 'linkedin', 'youtube',
+                    'investor', 'adviserinfo.sec', 'finra', 'sipc',
+                    'theconversation', 'benefitcorporationreduced', 'onlinelibrary.wiley']
+    outlink_list = [outlink + '_outlink_click' for outlink in outlink_list]
+    # --> scrape rest of outlinks from site (?)
+
+    # expand video actions to individual plays, pauses, resumes, seeks, and finishes
+    video_list = []
+    for video in ['humankind-short', 'humankind', 'wtf-short', 'wtf']:
+        for video_act in ['video_play', 'video_pause', 'video_resume', 'video_seek',
+                          'video_finish']: video_list.append(video + '_' + video_act)
+
+    # expand form actions to individual interactions and submissions
+    form_list = []
+    for form in ['getstarted', 'newsletter', 'contactus', 'institutionalcontact']:
+        for form_act in ['form_interaction', 'form_submission']:
+            form_list.append(form + '_' + form_act)
+
+    # build full action list
+    action_list = [i for i in get_action_category_map()]
+    article_index = action_list.index('articles-post_pageview')
+    action_list[article_index:article_index] = article_list
+    action_list.remove('articles-post_pageview')
+    ranking_index = action_list.index('rankings-company_pageview')
+    action_list[ranking_index:ranking_index] = ranking_list
+    action_list.remove('rankings-company_pageview')
+    logo_index = action_list.index('logo_download')
+    action_list[logo_index:logo_index] = logo_list
+    action_list.remove('logo_download')
+    outlink_index = action_list.index('social_outlink_click')
+    action_list[outlink_index:outlink_index] = outlink_list
+    for ol in ['social_outlink_click', 'articles_outlink_click', 'compliance_outlink_click']:
+        action_list.remove(ol)
+    video_index = action_list.index('humankind-short_video_action')
+    action_list[video_index:video_index] = video_list
+    for vid in ['humankind-short_video_action', 'humankind_video_action',
+                'wtf-short_video_action', 'wtf_video_action']:
+        action_list.remove(vid)
+    form_index = action_list.index('getstarted_form_action')
+    action_list[form_index:form_index] = form_list
+    for frm in ['getstarted_form_action', 'newsletter_form_action',
+                'contactus_form_action', 'institutionalcontact_form_action']:
+        action_list.remove(frm)
+    for hmpg in ['humankind', 'humankindfunds']: action_list.insert(
+            action_list.index(hmpg + '_pageview')+1, hmpg + '_socially_responsible_pageview')
+
+    # map actions to numbers
+    return {action : i for i, action in enumerate(action_list)}
+
+
+def get_site_map():
+    """
+    Build numerical mapping for site flows.
+    
+    Returns
+    -------
+    dict of {str : int}
+        Dictionary mapping sites to integers.
+    """
+    
+    site_list = ['humankind.co', 'rankings.humankind.co', 'humankindfunds.com',
+                 'session-start', 'session-end', 'None']
+    return {site : i for i, site in enumerate(site_list)}
+
+
+def get_engage_map():
+    """
+    Build numerical mapping for engagement flows.
+    
+    Returns
+    -------
+    dict of {str : int}
+        Dictionary mapping engagement types to integers.
+    """
+    
+    return {val.replace(',', '').replace(' ', '_') : key for
+            key, val in get_cluster_grades().engagement_type.to_dict().items()}
+
+
+def map_action_flow(df, colstr='', action_types=[], drop_sessions=False, drop_none=False):
+    """
+    Map action flows to numerical sequences.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Raw visitor-level data.
+    colstr : str
+        String to replace 'action' in action flow column names.
+    action_types : list of str
+        Action types to include in flows.
+    drop_sessions : bool
+        Whether to drop 'session-start' and 'session-end' from action flows.
+    drop_none : bool
+        Whether to drop 'None' from action flows.
+
+    Returns
+    -------
+    pd.DataFrame
+        Dataframe of numerical sequences of given action type flows.
+    """
+    
+    action_flow = []
+    actflow_cols = ['action_flow', 'action_category_flow', 'action_site_flow', 'action_ts']
+    for col in actflow_cols: action_flow.append(df[col].str.split(',').explode())
+    action_flow = pd.concat(action_flow, axis=1).reset_index()
+    
+    # filter action flow based on action types
+    pat_ix = pd.Index([])  # select actions of given types 
+    pat = r'.*_({})'.format('|'.join(action_types))
+    pat_ix = action_flow.loc[action_flow.action_flow.apply(
+        lambda x: bool(re.match(pat, x)))].index
+    sess_ix = pd.Index([])  # select session-starts/ends
+    if not drop_sessions: sess_ix = action_flow.loc[
+            action_flow.action_flow.isin(['session-start', 'session-end'])].index
+    none_ix = pd.Index([])  # select None's
+    if not drop_none: none_ix = action_flow.loc[
+            action_flow.action_flow == 'None'].index
+    drop_ix = action_flow.index.difference(pat_ix.union(sess_ix).union(none_ix))  # drop other ix
+    action_flow = action_flow.drop(drop_ix)
+    
+    # map actions to numbers
+    action_flow.action_flow = action_flow.action_flow.map(get_action_map())
+    action_flow.action_category_flow = action_flow.action_category_flow.map(
+        get_action_category_map())
+    action_flow.action_site_flow = action_flow.action_site_flow.map(get_site_map())
+    
+    # drop rows with missing values
+    action_flow = action_flow.drop(action_flow[action_flow.isnull().any(axis=1)].index)
+    action_flow[actflow_cols[:-1]] = action_flow[actflow_cols[:-1]].astype(int).astype(str)
+    
+    # group actions by visitor id to build numerical sequence columns
+    vdf = pd.DataFrame()
+    for col in actflow_cols:
+        outcol = col.replace('action', colstr) if colstr else col
+        vdf[outcol] = action_flow.groupby('visitor_id')[col].apply(lambda x: ','.join(x))
+    
+    return vdf
+
+
+def map_engage_flow(df):
+    """
+    Map engagement flows to numerical sequences.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Raw visitor-level data.
+
+    Returns
+    -------
+    pd.DataFrame
+       Numerical sequences of engagement types across visits.
+    """
+    
+    engage_flow = df.engagement_flow.str.split(',').explode()
+    engage_flow = engage_flow.map(get_engage_map()).astype(str)
+    engage_flow = pd.DataFrame(engage_flow.groupby('visitor_id').apply(lambda x: ','.join(x)))
+    
+    return engage_flow
+
+
+def build_processed_visitor_data(visits=None, visitors=None, drop_sessions=False, drop_none=False):
+    """
+    Build processed visitor-level data set.
+
+    Processed visitor data = summary data and numerical sequences representing customer journeys.
+    
+    Parameters
+    ----------
+    visits : pd.DataFrame
+        Raw visit-level data. If none passed in, must pass in raw visitor-level data instead.
+    visitors : pd.DataFrame
+        Raw visitor-level data. If none passed in, will build on the fly.
+    drop_sessions : bool
+        Whether to drop 'session-start' and 'session-end' from action flows.
+    drop_none : bool
+        Whether to drop 'None' from action flows.
+
+    Returns
+    -------
+    pd.DataFrame
+        Processed visitor-level data.
+    """
+
+    # get raw visitor-level data
+    if visitors is None:
+        if visits is None: raise Exception('Must pass in either raw visit- or visitor-level data.')
+        visitors = build_raw_visitor_data(visits)
+
+    df = visitors.copy()
+
+    # get summary data
+    df.actions = df.action_category_flow.apply(
+        lambda x: len([i for i in x.split(',') if not i.startswith('session-') and i != 'None']))
+    for action in ['pageview', 'download', 'outlink_click', 'buyetf_click',
+                   'brokerlink_click', 'video_action', 'form_action']:
+        df[action + 's'] = df.action_category_flow.apply(
+            lambda x: len([i for i in x.split(',') if i.endswith('_' + action)]))
+    for duration in ['visit_duration', 'action_duration',
+                     'page_duration', 'page_action_duration']:
+        df[duration] = df[duration].apply(lambda x: sum(x))
+
+    df.timestamp = df.timestamp.explode().astype(str).groupby('visitor_id').apply(
+        lambda x: ','.join(x))  # transform from list to comma separated string
+
+    # map visit flows to numerical sequences
+    maps = [
+        dict(zip(calendar.day_name, [str(i) for i in range(7)])),
+        {hr : str(i) for i, hr in enumerate(['preopening', 'early', 'core', 'late', 'None'])},
+        {dc : str(i) for i, dc in enumerate(np.sort(df.device_category.explode().unique()))},
+        {rt : str(i) for i, rt in enumerate(sorted(
+            sorted(df.referrer_type.explode().unique()), key=lambda s: s.split('_')[-1]))},
+        ]
+    cols = ['day', 'visit_trade_hours', 'device_category', 'referrer_type']
+    for i, col in enumerate(cols):
+        df[col] = df[col].apply(lambda x: ','.join(list(map(maps[i].get, x))))
+        
+    # map action and engagement flows to numerical sequences
+    action_flow = map_action_flow(df, drop_sessions=drop_sessions, drop_none=drop_none)
+    page_flow = map_action_flow(df, colstr='page', action_types=['pageview'],
+                                drop_sessions=drop_sessions, drop_none=drop_none)
+    engage_flow = map_engage_flow(df)
+
+    # drop original columns and replace with transformations
+    df = df.drop(columns=[col for col in df.columns if col in
+                          list(action_flow.columns) +
+                          list(page_flow.columns) +
+                          list(engage_flow.columns)])
+    df = pd.concat([df, action_flow, page_flow, engage_flow], axis=1)    
+
+    return df
+
+    
+# MODEL FOR ENGAGEMENT TYPES ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+def load_default_model():
+    """
+    Load visit-level engagement types model and corresponding scaler.
+
+    Returns
+    -------
+    sklearn.estimator
+        Fitted Gaussian mixture model.
+    sklearn.preprocessor
+        Fitted StandardScaler that includes feature names.
+    """
+    
+    data_path = os.path.join(pathlib.Path(__file__).parent.resolve(), "data")
+    d = '2023-04-02'
+    scaler = load(os.path.join(data_path,'gmm_scaler_{}.joblib'.format(d)))
+    clf = load(os.path.join(data_path,'gmm_{}.joblib'.format(d)))
+
+    return clf, scaler
+
+
+def get_engagement_features(scaler=None):
+    """
+    Get feature names of required for classifying visit engagement types.
+
+    Parameters
+    ----------
+    scaler : sklearn.preprocessor
+        Fitted StandardScaler with feature names.
+    
+    Returns
+    -------
+    list of str
+        List of feature names.
+    """
+
+    if scaler is None: _, scaler = load_default_model()
+
+    scaler_features = scaler.feature_names_in_.tolist()
+    bounce_features = ['visit_count',
+                       'visit_duration',
+                       'action_duration',
+                       'pages',
+                       'downloads',
+                       'brokerlinks',
+                       'video_pauses',
+                       'video_resumes',
+                       ]
+    visit_features = ['visit_id', 'date']
+    calc_features = ['articles_page_action_duration',
+                     'article-post_page_action_duration',
+                     'seconds_since_first_visit',
+                     'seconds_since_last_visit',
+                     'page_action_duration',
+                     'humankind_page_action_duration',
+                     'humankindfunds_page_action_duration',
+                     ]
+
+    return list(set(scaler_features + bounce_features + visit_features + calc_features))
+
+    
+def get_bounce_mask(df):
+    """
+    Create mask for 'new, bounce' cluster
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Visit-level data.
+
+    Returns
+    -------
+    bounce_mask : pd.Series
+        Mask for selecting the bounce visits out of the df.
+    """
+    
+    # check that the required columns are present in the dataframe
+    col = ['visit_duration',
+           'action_duration',
+           'downloads',
+           'video_resumes',
+           'brokerlinks',
+           'visit_count',
+           'pages',
+           ]
+    assert all(c in list(df) for c in col), "One or more columns are missing from df"
+    bounce_mask= (((df['visit_duration']==0) | (df['action_duration']==0)) &
+                  (df['downloads']==0) & (df['brokerlinks']==0) &
+                  (df['visit_count']==1) & (df['pages']<=1) & (df['video_resumes']==0))
+    return bounce_mask
+
+
+def get_cluster_names(date=''):
+    """
+    Provide a map between cluster ids and the names assigned to those clusters.
+
+    Parameters
+    ----------
+    date : str
+        The final date for the data set used to derive the names.
+    
+    Returns
+    -------
+    names : pd.Series
+        Series mapping engagement type numbers to names. Internal name allows
+        use as column upon merging with dataframe.
+    """
+    
+    if date== '2022-10-23':
+        names = pd.Series({
+            0: 'new, low engagement', 
+            5: 'return, 1pg, no action',
+            12: 'scrolling pgs with vids',
+            7: 'browsing home pgs',
+            19: 'ETF, brokerlinks',  # small chance brokerlink?
+            11: 'ETF, just looking',  # no vids, brokerlinks, downloads. Similar chance of seeing either home pg. 
+            17: 'return, low engagement', 
+            9: 'article reading', 
+            3: 'new, downloads',
+            8: 'browsing home pgs',
+            16: 'brokerlinks, articles',
+            1: 'video watching',
+            6: 'downloads, brokerlink',
+            13: 'new, visiting many pgs',
+            18: 'broad engagement except downloads',
+            2: 'get started form',
+            10: 'downloads, brokerlink', 
+            14: 'research and articles',
+            15: 'downloads, videos, team pg, get started',
+            4: 'downloads, videos, team pg, get started'
+            },name='engagement_type')
+    else:
+        names= pd.Series({
+            1: 'new, auto video', 
+            9: 'return, 1pg, no action',
+            0: 'browsing home pgs',
+            4: 'new, low chance of download',
+            6: 'return to advisor home and explore pages', 
+            5: 'scrolling advisor home',
+            8: 'brief return, low chance of download',
+            7: 'new, exploratory',
+            3: 'likely to click brokerlink',
+            11: 'article reading, other exploration',
+            2: 'exploratory, high chance of download',
+            10: 'broad, long engagement', 
+            },name='engagement_type')
+        
+    return names
+    
+    
+def assign_cluster(visit, scaler=None, clf=None, cluster_names=None):
+    """
+    Assign each visit to a cluster based on the trained clustering model.
+
+    Parameters
+    ----------
+    visit : pd.DataFrame
+        Visit-level data. Some features will be normalized to be used as inputs
+        for the classifier. If the dataset is too different from the original 
+        data set (from 2021-04-01 to 2022-09-20) the scaling may lead to 
+        inconsistent results from the classifier
+    scaler : sklearn.preprocessor, optional
+        Fitted StandardScaler that includes feature names. The default is the
+        most recent fitted StandardScaler.
+    clf : sklearn.estimator, optional
+        Fitted Gaussian mixture model. The default is the most recent fitted 
+        model.
+    cluster_names : pd.Series, optional.
+        A map from cluster id to name. The default is the most recent map.
+
+    Returns
+    -------
+    engagement : pd.DataFrame
+        The index is visit_id and the only column is engagement_type.
+    
+    Example
+    -------
+    assign engagement type and merge with the rest of the data:
+        engagement= analy_utils.assign_cluster(visit)
+        visit.set_index('visit_id', inplace=True)
+        visit= visit.join(engagement, how='inner')
+    """
+
+    if clf is None or scaler is None: clf, scaler = load_default_model()
+    if cluster_names is None: cluster_names = get_cluster_names('')
+        
+    #check for required features
+    if 'articles_duration' not in visit.columns:
+        #combine all article time
+        visit['articles_duration']= visit.loc[:, [
+            'articles_page_action_duration', 'article-post_page_action_duration']].sum(axis=1)
+    if 'minutes_since_last_visit' not in visit.columns:
+        #convert seconds to minutes
+        for col in ['seconds_since_first_visit', 'seconds_since_last_visit']:
+            visit['minutes_'+ col.split('_', 1)[1]]= visit[col]/60
+            
+    visit['other_page_duration']= visit['page_action_duration']- visit[
+        ['humankind_page_action_duration',
+         'humankindfunds_page_action_duration',
+         'articles_duration']].sum(axis=1)
+    #change negative values to 0
+    visit['other_page_duration']= np.where(visit['other_page_duration']<0, 0, visit['other_page_duration'])
+    
+    #check that all features are present in the input data
+    missing_features= [c for c in scaler.feature_names_in_ if c not in visit.columns]
+    assert len(missing_features)==0, f"The following features are missing from visit: {missing_features}"
+    
+    #fill null values if they exist in these columns
+    visit[scaler.feature_names_in_] = visit[scaler.feature_names_in_].fillna(0)
+    
+    #let the first cluster be the bounce cluster for non-returning visits
+    bounce_mask= get_bounce_mask(visit)
+    df_bounce= visit.loc[bounce_mask, ['visit_id','date']]
+    df_bounce['engagement_type']= "new, bounce"
+    df= visit.loc[~bounce_mask, ['visit_id'] + list(scaler.feature_names_in_)]
+    
+    #apply the preprocessor and the model
+    X= scaler.transform(df[scaler.feature_names_in_])
+    df['cluster_id']= clf.predict(X)
+    
+    #assign the names based on cluster id to the corresponding visits
+    df= df.merge(cluster_names, how='left', 
+                 left_on='cluster_id', right_index=True)
+    
+    engagement= pd.concat([df[['visit_id','engagement_type']], 
+                    df_bounce[['visit_id','engagement_type']]], 
+                   ignore_index=True, axis=0)
+    engagement.set_index('visit_id', inplace=True)
+    return engagement
+
+
+def get_cluster_grades():
+    """
+    Get the look up table for the grade and engagement score of each engagement
+    type
+
+    Returns
+    -------
+    grade : pd.DataFrame
+        1 row for each engagement type, 3 columns.
+
+    """
+    grade= pd.DataFrame([
+        ['new, low chance of download', 'A'],
+        ['likely to click brokerlink', 'A'],
+        ['return, 1pg, no action','A'],
+        ['new, exploratory', 'A'],
+        
+        ['exploratory, high chance of download', 'B+'],
+        
+        ['article reading, other exploration', 'B'], 
+        ['browsing home pgs', 'B'],
+        ['new, auto video', 'B'],
+        
+        ['brief return, low chance of download', 'C'],
+        
+        ['scrolling advisor home', 'D'],
+        ['return to advisor home and explore pages','D'], 
+        ['broad, long engagement', 'D'],
+        
+        ['new, bounce', 'F']], 
+        columns=['engagement_type','grade'])
+    
+    value= pd.DataFrame([
+        [4, 'A'],
+        [3, 'B'],
+        [3.2, 'B+'],
+        [2, 'C'],
+        [1, 'D'],
+        [0, 'F']], 
+        columns=['engagement_score','grade'])
+    grade= grade.merge(value, how='left', on='grade')
+    
+    return grade
```

### Comparing `utilities_hki-0.1.7/src/utilities_hki/db_utils.py` & `utilities_hki-0.1.8/src/utilities_hki/db_utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-"""
-Database utility functions.
-Copyright (C) 2022 Humankind Investments
-"""
-
-import boto3
-import psycopg2
-from psycopg2.extras import execute_batch
-from psycopg2 import sql
-
-
-def database_connect(dbname, db_dict):
-    """
-    Connect to database with given name.
-
-    Parameters
-    ----------
-    dbname : str
-        Name of database to query.
-    db_dict : dict
-        Dictionary of credentials for all databases. For example:
-        db_dict = {'hkisocial' : cred.hkisocial,
-                    'hkiweb' : cred.hkiweb,
-                    'hkimarket' : cred.hkimarket,
-                    'hkiads' : cred.hkiads,
-                    }
-
-    Returns
-    -------
-    psycopg2.connection.cursor
-        Database connection cursor object.
-    psycopg2.connection
-        Database connection object.
-    """
-
-    session = boto3.Session(profile_name = 'default')
-    client = boto3.client('rds')
-
-    conn = psycopg2.connect(host = db_dict[dbname]['endpoint'],
-                            port = db_dict[dbname]['port'],
-                            database = dbname,
-                            user = db_dict[dbname]['username'],
-                            password = db_dict[dbname]['pw'],
-                            )
-
-    return conn.cursor(), conn
-
-
-def database_write(dbname, db_dict, table_query, df, table_name):
-    """
-    Write data to table in database.
-
-    Parameters
-    ----------
-    dbname : str
-        Name of database to which to write the data.
-    db_dict : dict
-        Dictionary of credentials for database(s).
-    table_query : str
-        Initial table creation query.
-    df : pd.DataFrame
-        Dataframe to insert into table in database.
-    table_name : str
-        Name of table in which to insert data.
-    """
-
-    # connect to database
-    cursor, conn = database_connect(dbname, db_dict)
-
-    # create initial table
-    cursor.execute(table_query)
-    conn.commit()
-
-    # write data to table in DB
-    tdict = df.to_dict(orient='records')
-    tname = '%s' % table_name
-    tcolumns = list(df)
-    query = insert_data(tname, tcolumns)
-    execute_batch(cursor, query, tdict)
-    conn.commit()
-
-    cursor.close()
-    conn.close()
-
-    
-def insert_data(table, columns):
-    """
-    Create insert query.
-
-    Parameters
-    ----------
-    table : str
-        Name of table in which to insert data.
-    columns : list of str
-        List of column names in table.
-    
-    Returns
-    -------
-    insert : sql query
-        SQL insert query.
-    """
-
-    insert = sql.SQL('INSERT INTO {} ({}) VALUES({});').format(
-        sql.Identifier(table),
-        sql.SQL(',').join(map(sql.Identifier, columns)),
-        sql.SQL(',').join(map(sql.Placeholder, columns))
-        )
-
-    return insert
-
+"""
+Database utility functions.
+Copyright (C) 2022 Humankind Investments
+"""
+
+import boto3
+import psycopg2
+from psycopg2.extras import execute_batch
+from psycopg2 import sql
+
+
+def database_connect(dbname, db_dict):
+    """
+    Connect to database with given name.
+
+    Parameters
+    ----------
+    dbname : str
+        Name of database to query.
+    db_dict : dict
+        Dictionary of credentials for all databases. For example:
+        db_dict = {'hkisocial' : cred.hkisocial,
+                    'hkiweb' : cred.hkiweb,
+                    'hkimarket' : cred.hkimarket,
+                    'hkiads' : cred.hkiads,
+                    }
+
+    Returns
+    -------
+    psycopg2.connection.cursor
+        Database connection cursor object.
+    psycopg2.connection
+        Database connection object.
+    """
+
+    session = boto3.Session(profile_name = 'default')
+    client = boto3.client('rds')
+
+    conn = psycopg2.connect(host = db_dict[dbname]['endpoint'],
+                            port = db_dict[dbname]['port'],
+                            database = dbname,
+                            user = db_dict[dbname]['username'],
+                            password = db_dict[dbname]['pw'],
+                            )
+
+    return conn.cursor(), conn
+
+
+def database_write(dbname, db_dict, table_query, df, table_name):
+    """
+    Write data to table in database.
+
+    Parameters
+    ----------
+    dbname : str
+        Name of database to which to write the data.
+    db_dict : dict
+        Dictionary of credentials for database(s).
+    table_query : str
+        Initial table creation query.
+    df : pd.DataFrame
+        Dataframe to insert into table in database.
+    table_name : str
+        Name of table in which to insert data.
+    """
+
+    # connect to database
+    cursor, conn = database_connect(dbname, db_dict)
+
+    # create initial table
+    cursor.execute(table_query)
+    conn.commit()
+
+    # write data to table in DB
+    tdict = df.to_dict(orient='records')
+    tname = '%s' % table_name
+    tcolumns = list(df)
+    query = insert_data(tname, tcolumns)
+    execute_batch(cursor, query, tdict)
+    conn.commit()
+
+    cursor.close()
+    conn.close()
+
+    
+def insert_data(table, columns):
+    """
+    Create insert query.
+
+    Parameters
+    ----------
+    table : str
+        Name of table in which to insert data.
+    columns : list of str
+        List of column names in table.
+    
+    Returns
+    -------
+    insert : sql query
+        SQL insert query.
+    """
+
+    insert = sql.SQL('INSERT INTO {} ({}) VALUES({});').format(
+        sql.Identifier(table),
+        sql.SQL(',').join(map(sql.Identifier, columns)),
+        sql.SQL(',').join(map(sql.Placeholder, columns))
+        )
+
+    return insert
+
```

### Comparing `utilities_hki-0.1.7/src/utilities_hki/fb_utils.py` & `utilities_hki-0.1.8/src/utilities_hki/fb_utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-"""
-Facebook Ads utility functions.
-Copyright (C) 2022 Humankind Investments
-"""
-
-import re
-import os, sys
-
-
-def get_columns(df_columns):
-    """
-    Get lists of columns by type for aggregating statistics.
-
-    Parameters
-    ----------
-    df_columns : list of str
-        List of column names in dataframe.
-
-    Returns
-    -------
-    list of str
-        List of column names representing metadata.
-    list of str
-        List of column names representing additive values.
-    list of str
-        List of column names representing scores.
-    list of str
-        List of column names representing ranks.
-    list of str
-        List of column names representing fractional values.
-    """
-
-    meta_cols = [col for col in ['account_id',
-                                 'campaign_id',
-                                 'campaign_name',
-                                 'adset_id',
-                                 'adset_name',
-                                 'ad_id',
-                                 'ad_name',
-                                 'objective',
-                                 'optimization_goal',
-                                 ] if col in df_columns]
-
-    sum_cols = [col for col in ['spend',
-                                'impressions',
-                                'reach',
-                                'clicks',
-                                'unique_clicks',
-                                'link_clicks',
-                                'landing_page_views',
-                                'post_engagements',
-                                'page_engagements',
-                                'unique_link_clicks',
-                                'unique_post_engagements',
-                                'unique_page_engagements',
-                                'outbound_clicks',
-                                'unique_outbound_clicks',
-                                'video_30_sec_watched_actions',
-                                'video_avg_time_watched_actions',
-                                'video_p100_watched_actions',
-                                'video_p75_watched_actions',
-                                'video_p50_watched_actions',
-                                'video_p25_watched_actions',
-                                'video_play_actions',
-                                'visits',
-                                'not_bounced',
-                                'etf_clicks',
-                                ] if col in df_columns]
-
-    score_cols = [col for col in df_columns if re.search("^quality_score.*$", col)]
-
-    rank_cols = [col for col in df_columns if re.search("^.*ranking$", col)]
-
-    div_cols = [col for col in ['frequency',
-                                'ctr',
-                                'unique_ctr',
-                                'cpc',
-                                'cost_per_unique_click',
-                                'cpm',
-                                'cpp',
-                                'cost_per_link_click',
-                                'cost_per_landing_page_view',
-                                'cost_per_post_engagement',
-                                'cost_per_page_engagement',
-                                'cost_per_unique_link_click',
-                                'cost_per_unique_post_engagement',
-                                'cost_per_unique_page_engagement',
-                                'outbound_clicks_ctr',
-                                'unique_outbound_clicks_ctr',
-                                'cost_per_outbound_click',
-                                'cost_per_unique_outbound_click',
-                                ] if col in df_columns]
-
-    return meta_cols, sum_cols, score_cols, rank_cols, div_cols
-
-
-def calculate_fractions(df, columns):
-    """
-    Return fractional values for given columns of dataframe.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Facebook Ads dataframe.
-    columns : list of str
-        List of columns to calculate and return.
-
-    Returns
-    -------
-    pd.DataFrame
-        Dataframe containing columns with recalculated values.
-    """
-    
-    ctr_cols = [col for col in columns if re.search(r"^.*ctr.*$", col)]
-    cost_cols = [col for col in columns if re.search(r"^(cost.*|cp.)$", col)]
-
-    try:
-        df['frequency'] = df['impressions'] / df['reach']
-    except:
-        pass
-
-    for icol in ctr_cols:
-        numer = icol.split('ctr')[0]
-        if 'click' not in numer: numer += 'clicks'
-        numer = numer.strip('_')
-        denom = 'reach' if numer.startswith('unique') else 'impressions'
-        try:
-            df[icol] = df[numer] / df[denom] * 100
-        except:
-            pass
-        
-    for icol in cost_cols:
-        mult = 1
-        numer = 'spend'
-        col_split = icol.split('cost_per_')
-        try:
-            denom = col_split[1] + 's'
-        except IndexError:
-            denom = col_split[0]
-            if denom == 'cpm' or denom == 'cpp':
-                denom = 'impressions' if denom == 'cpm' else 'reach'
-                mult = 1000
-            else:
-                denom = 'clicks'
-        try:
-            df[icol] = df[numer] / df[denom] * mult
-        except:
-            pass
-
-    return df[columns]
-
-
+"""
+Facebook Ads utility functions.
+Copyright (C) 2022 Humankind Investments
+"""
+
+import re
+import os, sys
+
+
+def get_columns(df_columns):
+    """
+    Get lists of columns by type for aggregating statistics.
+
+    Parameters
+    ----------
+    df_columns : list of str
+        List of column names in dataframe.
+
+    Returns
+    -------
+    list of str
+        List of column names representing metadata.
+    list of str
+        List of column names representing additive values.
+    list of str
+        List of column names representing scores.
+    list of str
+        List of column names representing ranks.
+    list of str
+        List of column names representing fractional values.
+    """
+
+    meta_cols = [col for col in ['account_id',
+                                 'campaign_id',
+                                 'campaign_name',
+                                 'adset_id',
+                                 'adset_name',
+                                 'ad_id',
+                                 'ad_name',
+                                 'objective',
+                                 'optimization_goal',
+                                 ] if col in df_columns]
+
+    sum_cols = [col for col in ['spend',
+                                'impressions',
+                                'reach',
+                                'clicks',
+                                'unique_clicks',
+                                'link_clicks',
+                                'landing_page_views',
+                                'post_engagements',
+                                'page_engagements',
+                                'unique_link_clicks',
+                                'unique_post_engagements',
+                                'unique_page_engagements',
+                                'outbound_clicks',
+                                'unique_outbound_clicks',
+                                'video_30_sec_watched_actions',
+                                'video_avg_time_watched_actions',
+                                'video_p100_watched_actions',
+                                'video_p75_watched_actions',
+                                'video_p50_watched_actions',
+                                'video_p25_watched_actions',
+                                'video_play_actions',
+                                'visits',
+                                'not_bounced',
+                                'etf_clicks',
+                                ] if col in df_columns]
+
+    score_cols = [col for col in df_columns if re.search("^quality_score.*$", col)]
+
+    rank_cols = [col for col in df_columns if re.search("^.*ranking$", col)]
+
+    div_cols = [col for col in ['frequency',
+                                'ctr',
+                                'unique_ctr',
+                                'cpc',
+                                'cost_per_unique_click',
+                                'cpm',
+                                'cpp',
+                                'cost_per_link_click',
+                                'cost_per_landing_page_view',
+                                'cost_per_post_engagement',
+                                'cost_per_page_engagement',
+                                'cost_per_unique_link_click',
+                                'cost_per_unique_post_engagement',
+                                'cost_per_unique_page_engagement',
+                                'outbound_clicks_ctr',
+                                'unique_outbound_clicks_ctr',
+                                'cost_per_outbound_click',
+                                'cost_per_unique_outbound_click',
+                                ] if col in df_columns]
+
+    return meta_cols, sum_cols, score_cols, rank_cols, div_cols
+
+
+def calculate_fractions(df, columns):
+    """
+    Return fractional values for given columns of dataframe.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Facebook Ads dataframe.
+    columns : list of str
+        List of columns to calculate and return.
+
+    Returns
+    -------
+    pd.DataFrame
+        Dataframe containing columns with recalculated values.
+    """
+    
+    ctr_cols = [col for col in columns if re.search(r"^.*ctr.*$", col)]
+    cost_cols = [col for col in columns if re.search(r"^(cost.*|cp.)$", col)]
+
+    try:
+        df['frequency'] = df['impressions'] / df['reach']
+    except:
+        pass
+
+    for icol in ctr_cols:
+        numer = icol.split('ctr')[0]
+        if 'click' not in numer: numer += 'clicks'
+        numer = numer.strip('_')
+        denom = 'reach' if numer.startswith('unique') else 'impressions'
+        try:
+            df[icol] = df[numer] / df[denom] * 100
+        except:
+            pass
+        
+    for icol in cost_cols:
+        mult = 1
+        numer = 'spend'
+        col_split = icol.split('cost_per_')
+        try:
+            denom = col_split[1] + 's'
+        except IndexError:
+            denom = col_split[0]
+            if denom == 'cpm' or denom == 'cpp':
+                denom = 'impressions' if denom == 'cpm' else 'reach'
+                mult = 1000
+            else:
+                denom = 'clicks'
+        try:
+            df[icol] = df[numer] / df[denom] * mult
+        except:
+            pass
+
+    return df[columns]
+
+
```

### Comparing `utilities_hki-0.1.7/src/utilities_hki/data/gmm_2022-10-23.joblib` & `utilities_hki-0.1.8/src/utilities_hki/data/gmm_2022-10-23.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.7/src/utilities_hki/data/gmm_2023-04-02.joblib` & `utilities_hki-0.1.8/src/utilities_hki/data/gmm_2023-04-02.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.7/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib` & `utilities_hki-0.1.8/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.7/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib` & `utilities_hki-0.1.8/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.7/LICENSE.txt` & `utilities_hki-0.1.8/LICENSE.txt`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,661 +1,661 @@
-                    GNU AFFERO GENERAL PUBLIC LICENSE
-                       Version 3, 19 November 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU Affero General Public License is a free, copyleft license for
-software and other kinds of works, specifically designed to ensure
-cooperation with the community in the case of network server software.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-our General Public Licenses are intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  Developers that use our General Public Licenses protect your rights
-with two steps: (1) assert copyright on the software, and (2) offer
-you this License which gives you legal permission to copy, distribute
-and/or modify the software.
-
-  A secondary benefit of defending all users' freedom is that
-improvements made in alternate versions of the program, if they
-receive widespread use, become available for other developers to
-incorporate.  Many developers of free software are heartened and
-encouraged by the resulting cooperation.  However, in the case of
-software used on network servers, this result may fail to come about.
-The GNU General Public License permits making a modified version and
-letting the public access it on a server without ever releasing its
-source code to the public.
-
-  The GNU Affero General Public License is designed specifically to
-ensure that, in such cases, the modified source code becomes available
-to the community.  It requires the operator of a network server to
-provide the source code of the modified version running there to the
-users of that server.  Therefore, public use of a modified version, on
-a publicly accessible server, gives the public access to the source
-code of the modified version.
-
-  An older license, called the Affero General Public License and
-published by Affero, was designed to accomplish similar goals.  This is
-a different license, not a version of the Affero GPL, but Affero has
-released a new version of the Affero GPL which permits relicensing under
-this license.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU Affero General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Remote Network Interaction; Use with the GNU General Public License.
-
-  Notwithstanding any other provision of this License, if you modify the
-Program, your modified version must prominently offer all users
-interacting with it remotely through a computer network (if your version
-supports such interaction) an opportunity to receive the Corresponding
-Source of your version by providing access to the Corresponding Source
-from a network server at no charge, through some standard or customary
-means of facilitating copying of software.  This Corresponding Source
-shall include the Corresponding Source for any work covered by version 3
-of the GNU General Public License that is incorporated pursuant to the
-following paragraph.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the work with which it is combined will remain governed by version
-3 of the GNU General Public License.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU Affero General Public License from time to time.  Such new versions
-will be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU Affero General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU Affero General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU Affero General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU Affero General Public License as published
-    by the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU Affero General Public License for more details.
-
-    You should have received a copy of the GNU Affero General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If your software can interact with users remotely through a computer
-network, you should also make sure that it provides a way for users to
-get its source.  For example, if your program is a web application, its
-interface could display a "Source" link that leads users to an archive
-of the code.  There are many ways you could offer source, and different
-solutions will be better for different programs; see section 13 for the
-specific requirements.
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU AGPL, see
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+our General Public Licenses are intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU Affero General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU Affero General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU Affero General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU Affero General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published
+    by the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU AGPL, see
 <https://www.gnu.org/licenses/>.
```

### Comparing `utilities_hki-0.1.7/README.md` & `utilities_hki-0.1.8/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-# Global Utilities
-
-> last modified 8 March 2023 by Colleen Treado
-
-The `utilities-hki` repository contains the common utilities required by multiple other `humankind-datascience` repositories. Unlike the old `utilities` repo, this package contains no encrypted files, and credentials are now passed into the utility functions as input arguments.
-
-## Current status
-This repository is the code repository for the `utilities-hki` pip package, which, together with the new `credentials` repository, replaces the current `utilities` submodule in the other repositories used for data science at Humankind. The package was created by following [this guide](https://packaging.python.org/en/latest/tutorials/packaging-projects/) and the package can be found on [PyPI](https://pypi.org/project/utilities-hki/). Most of our repositories have been updated to import the new `utilities-hki` pip package and call the updated utility functions, passing in the credentials from the new `credentials` repo, instead. The repositories that still need to be updated are
-- daily_volume_predict
-- volume_predict (but this is not in use)
-- facebook_ads
-
-
-## Installation and setup
-
-For first-time setup, clone the repository into a fresh work area:
-
-```bash
-# cloning via ssh is preferred but requires an ssh key connection in your account
-git clone git@github.com:humankind-datascience/utilities-hki.git
-```
-
-The code requires a number of Python packages to run, which should be installed inside of a dedicated virtual environment. The preferred virtual environment tool is [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/).
-
-To install the required packages in a new virtual environment, run the following command from the top-level directory of the git repository:
-```bash
-pip install -r requirements.txt
-```
-
-If additional packages need to be installed upon changes to the code, add them to the `requirements-top-level.txt` file. Then run the below commands to install (and upgrade) the top-level dependencies and update the `requirements.txt` file for future use.
-```bash
-pip install -r requirements-top-level.txt --upgrade
-pip freeze -r requirements-top-level.txt > requirements.txt
-```
-
-Additionally, the AWS Command Line Interface (AWS CLI) is required for use of the botocore library, which is used in database utilitify functions to read from and write to the AWS RDS databases. See the [https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-welcome.html](AWS CLI documentation) for installation instructions.
-
-Now you can run the top-level scripts:
-
-```bash
-python <utilities-script.py>
-```
-
-The `utilities-hki` repository contains only testing top-level scripts, designed to test the utility functions during package development.
-
-
-## Code updates
-
-When making changes to the code, follow [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow), i.e. create a new branch, make changes on that branch, frequently committing and pushing those changes to that branch, and then create a pull request to merge those changes into master upon review and approval.
-
-
-## Utility code overview
-
-The `utilities-hki` repository contains common utility functions used across repositories in the Humankind Data Science code base. The utility functions are grouped by type into separate modules, as outlined below.
-
-- **analy_utils**: analysis utility functions, including cleaning procedures for and assignment of engagement types to the visit-level data;
-- **db_utils**: database utility functions;
-- **email_utils**: email utility functions;
-- **fb_utils**: Facebook Ads utility functions.
-
-Standard cleaning of the visit-level data should be implemented at the start of any analysis and can be achieved by calling the `analy_utils.clean_visits` function (see the docstrings for more details.
-
-Sample code for applying the trained clustering model and assigning the letter/numeric grades to the engagement types for each visit is provided below, where `visit` is a DataFrame. Read the docstrings for assign_cluster() and get_cluster_grades() for more details.
-
-```
-from utilities-hki import analy_utils
-# assumes visit data has already been pulled or loaded into visit
-
-engagement = analy_utils.assign_cluster(visit)
-engagement = engagement.reset_index().merge(
-    analy_utils.get_cluster_grades(), how='left', on='engagement_type')
-visit = visit.merge(engagement, how='inner', on='visit_id')
+# Global Utilities
+
+> last modified 8 March 2023 by Colleen Treado
+
+The `utilities-hki` repository contains the common utilities required by multiple other `humankind-datascience` repositories. Unlike the old `utilities` repo, this package contains no encrypted files, and credentials are now passed into the utility functions as input arguments.
+
+## Current status
+This repository is the code repository for the `utilities-hki` pip package, which, together with the new `credentials` repository, replaces the current `utilities` submodule in the other repositories used for data science at Humankind. The package was created by following [this guide](https://packaging.python.org/en/latest/tutorials/packaging-projects/) and the package can be found on [PyPI](https://pypi.org/project/utilities-hki/). Most of our repositories have been updated to import the new `utilities-hki` pip package and call the updated utility functions, passing in the credentials from the new `credentials` repo, instead. The repositories that still need to be updated are
+- daily_volume_predict
+- volume_predict (but this is not in use)
+- facebook_ads
+
+
+## Installation and setup
+
+For first-time setup, clone the repository into a fresh work area:
+
+```bash
+# cloning via ssh is preferred but requires an ssh key connection in your account
+git clone git@github.com:humankind-datascience/utilities-hki.git
+```
+
+The code requires a number of Python packages to run, which should be installed inside of a dedicated virtual environment. The preferred virtual environment tool is [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/).
+
+To install the required packages in a new virtual environment, run the following command from the top-level directory of the git repository:
+```bash
+pip install -r requirements.txt
+```
+
+If additional packages need to be installed upon changes to the code, add them to the `requirements-top-level.txt` file. Then run the below commands to install (and upgrade) the top-level dependencies and update the `requirements.txt` file for future use.
+```bash
+pip install -r requirements-top-level.txt --upgrade
+pip freeze -r requirements-top-level.txt > requirements.txt
+```
+
+Additionally, the AWS Command Line Interface (AWS CLI) is required for use of the botocore library, which is used in database utilitify functions to read from and write to the AWS RDS databases. See the [https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-welcome.html](AWS CLI documentation) for installation instructions.
+
+Now you can run the top-level scripts:
+
+```bash
+python <utilities-script.py>
+```
+
+The `utilities-hki` repository contains only testing top-level scripts, designed to test the utility functions during package development.
+
+
+## Code updates
+
+When making changes to the code, follow [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow), i.e. create a new branch, make changes on that branch, frequently committing and pushing those changes to that branch, and then create a pull request to merge those changes into master upon review and approval.
+
+
+## Utility code overview
+
+The `utilities-hki` repository contains common utility functions used across repositories in the Humankind Data Science code base. The utility functions are grouped by type into separate modules, as outlined below.
+
+- **analy_utils**: analysis utility functions, including cleaning procedures for and assignment of engagement types to the visit-level data;
+- **db_utils**: database utility functions;
+- **email_utils**: email utility functions;
+- **fb_utils**: Facebook Ads utility functions.
+
+Standard cleaning of the visit-level data should be implemented at the start of any analysis and can be achieved by calling the `analy_utils.clean_visits` function (see the docstrings for more details.
+
+Sample code for applying the trained clustering model and assigning the letter/numeric grades to the engagement types for each visit is provided below, where `visit` is a DataFrame. Read the docstrings for assign_cluster() and get_cluster_grades() for more details.
+
+```
+from utilities-hki import analy_utils
+# assumes visit data has already been pulled or loaded into visit
+
+engagement = analy_utils.assign_cluster(visit)
+engagement = engagement.reset_index().merge(
+    analy_utils.get_cluster_grades(), how='left', on='engagement_type')
+visit = visit.merge(engagement, how='inner', on='visit_id')
 ```
```

### Comparing `utilities_hki-0.1.7/pyproject.toml` & `utilities_hki-0.1.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "utilities_hki"
-version = "0.1.7"
-authors = [
-  { name="Francisco Pena" },
-  { name="Colleen Treado" },
-]
-description = "Global utilities for Humankind data science"
-readme = "README.md"
-requires-python = ">=3.7"
-dependencies = [
-  "boto3>=1.21",
-  "psycopg2-binary>2.8",
-  "joblib==1.2.0",
-]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU Affero General Public License v3",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "utilities_hki"
+version = "0.1.8"
+authors = [
+  { name="Francisco Pena" },
+  { name="Colleen Treado" },
+]
+description = "Global utilities for Humankind data science"
+readme = "README.md"
+requires-python = ">=3.7"
+dependencies = [
+  "boto3>=1.21",
+  "psycopg2-binary>2.8",
+  "joblib==1.2.0",
+]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: GNU Affero General Public License v3",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
 "Homepage" = "https://github.com/humankind-datascience/utilities-hki"
```

### Comparing `utilities_hki-0.1.7/PKG-INFO` & `utilities_hki-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
-Name: utilities_hki
-Version: 0.1.7
+Name: utilities-hki
+Version: 0.1.8
 Summary: Global utilities for Humankind data science
 Project-URL: Homepage, https://github.com/humankind-datascience/utilities-hki
 Author: Francisco Pena, Colleen Treado
-License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: boto3>=1.21
 Requires-Dist: joblib==1.2.0
 Requires-Dist: psycopg2-binary>2.8
```

