# Comparing `tmp/accompanist-1.1.7-py3-none-any.whl.zip` & `tmp/accompanist-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,25 @@
-Zip file size: 45293 bytes, number of entries: 22
+Zip file size: 49464 bytes, number of entries: 23
 -rw-r--r--  2.0 unx        0 b- defN 23-May-18 15:07 accompanist/__init__.py
--rw-r--r--  2.0 unx     1511 b- defN 23-May-20 14:35 accompanist/cmd_init.py
--rw-r--r--  2.0 unx     6498 b- defN 23-May-24 14:49 accompanist/cmd_listen.py
--rw-r--r--  2.0 unx     3338 b- defN 23-May-22 09:12 accompanist/cmd_play.py
--rw-r--r--  2.0 unx      741 b- defN 23-May-18 15:08 accompanist/main.py
--rw-r--r--  2.0 unx      310 b- defN 23-May-18 14:54 accompanist/utility.py
--rw-r--r--  2.0 unx       18 b- defN 23-May-31 04:13 accompanist/version.py
+-rw-r--r--  2.0 unx     8566 b- defN 23-Jul-14 13:26 accompanist/cmd_hear.py
+-rw-r--r--  2.0 unx     1970 b- defN 23-Jul-14 12:07 accompanist/cmd_init.py
+-rw-r--r--  2.0 unx     8281 b- defN 23-Jul-14 13:31 accompanist/cmd_listen.py
+-rw-r--r--  2.0 unx     3637 b- defN 23-Jun-13 14:46 accompanist/cmd_play.py
+-rw-r--r--  2.0 unx      918 b- defN 23-Jun-08 14:26 accompanist/main.py
+-rw-r--r--  2.0 unx     1630 b- defN 23-Jul-14 12:05 accompanist/utility.py
+-rw-r--r--  2.0 unx       18 b- defN 23-Jul-14 14:18 accompanist/version.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-18 15:10 accompanist/report/__init__.py
 -rw-r--r--  2.0 unx     4302 b- defN 23-May-20 15:45 accompanist/report/draw_histgram.py
--rw-r--r--  2.0 unx     4578 b- defN 23-May-31 04:17 accompanist/report/draw_pie_chart.py
+-rw-r--r--  2.0 unx     5259 b- defN 23-Jun-15 13:41 accompanist/report/draw_pie_chart.py
 -rw-r--r--  2.0 unx     3562 b- defN 23-May-20 14:16 accompanist/report/draw_table.py
 -rw-r--r--  2.0 unx     1602 b- defN 23-May-18 16:04 accompanist/report/write_comment.py
 -rw-r--r--  2.0 unx     1503 b- defN 23-May-21 16:45 accompanist/report/write_front_cover.py
--rw-r--r--  2.0 unx     3645 b- defN 23-May-22 09:43 accompanist/report/write_header_footer.py
+-rw-r--r--  2.0 unx     3905 b- defN 23-Jun-09 15:09 accompanist/report/write_header_footer.py
 -rw-r--r--  2.0 unx    19193 b- defN 23-Mar-26 08:39 accompanist/resource/logo_trans.png
 -rw-r--r--  2.0 unx     6761 b- defN 23-Mar-26 08:25 accompanist/resource/logo_trans_small.png
--rw-r--r--  2.0 unx     1063 b- defN 23-May-31 04:20 accompanist-1.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     6225 b- defN 23-May-31 04:20 accompanist-1.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-31 04:20 accompanist-1.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-May-31 04:20 accompanist-1.1.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       31 b- defN 23-May-31 04:20 accompanist-1.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1889 b- defN 23-May-31 04:20 accompanist-1.1.7.dist-info/RECORD
-22 files, 66915 bytes uncompressed, 42191 bytes compressed:  36.9%
+-rw-r--r--  2.0 unx     1063 b- defN 23-Jul-14 14:33 accompanist-1.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7983 b- defN 23-Jul-14 14:33 accompanist-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 14:33 accompanist-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jul-14 14:33 accompanist-1.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       31 b- defN 23-Jul-14 14:33 accompanist-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1970 b- defN 23-Jul-14 14:33 accompanist-1.2.0.dist-info/RECORD
+23 files, 82299 bytes uncompressed, 46240 bytes compressed:  43.8%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: accompanist/__init__.py
 Comment: 
 
+Filename: accompanist/cmd_hear.py
+Comment: 
+
 Filename: accompanist/cmd_init.py
 Comment: 
 
 Filename: accompanist/cmd_listen.py
 Comment: 
 
 Filename: accompanist/cmd_play.py
@@ -42,26 +45,26 @@
 
 Filename: accompanist/resource/logo_trans.png
 Comment: 
 
 Filename: accompanist/resource/logo_trans_small.png
 Comment: 
 
-Filename: accompanist-1.1.7.dist-info/LICENSE
+Filename: accompanist-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: accompanist-1.1.7.dist-info/METADATA
+Filename: accompanist-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: accompanist-1.1.7.dist-info/WHEEL
+Filename: accompanist-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: accompanist-1.1.7.dist-info/entry_points.txt
+Filename: accompanist-1.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: accompanist-1.1.7.dist-info/top_level.txt
+Filename: accompanist-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: accompanist-1.1.7.dist-info/RECORD
+Filename: accompanist-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## accompanist/cmd_init.py

```diff
@@ -4,29 +4,34 @@
 
 import accompanist.utility as ut
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
 @click.command(name="init", context_settings=CONTEXT_SETTINGS,
-               help="Configure CWL log group setting.")
-@click.option("-l", "--log-group", required=True, default="aws-waf-logs-xxxxxxx", type=str,
-              prompt="Please input a log group name",
-              help="Set a CloudWatch Logs Log group name.")
+               help="Configure the accompanist's initial settings.")
+@click.option("-l", "--log-destination", required=True, default="CWL",
+              type=click.Choice(["CWL", "S3"]),
+              prompt="Please select a log destination type",
+              help="Select a log destination type of AWS WAF.")
+@click.option("-d", "--destination-name", required=True, default="aws-waf-logs-xxxxxxx", type=str,
+              prompt="Please input a log destination name, CloudWatch Logs log group name or S3 bucket name.",
+              help="Set a log destination name of AWS WAF, CloudWatch Logs log group name or S3 bucket name.")
 @click.option("-p", "--path", required=True, default="/.env", type=str,
               prompt="Please input a analysis target URI path",
               help="Set a URI path for counts that is blocked/counted.")
 @click.option("-c", "--comment", required=True,
               default="This is a sample comment.", type=str,
               prompt="Please input a comment on the report",
               help="Set a comment for report.")
-def init(log_group: str, path: str, comment: str) -> None:
+def init(log_destination: str, destination_name: str, path: str, comment: str) -> None:
 
     configure_items = {
-        "log_group": log_group,
+        "log_destination": log_destination,
+        "destination_name": destination_name,
         "target_uri": [path],
         "comment": [comment]
     }
 
     with open("config.json", mode="w", encoding="utf-8") as f:
         json.dump(configure_items, f, indent=2)
```

## accompanist/cmd_listen.py

```diff
@@ -15,15 +15,15 @@
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
 @click.command(name="listen", context_settings=CONTEXT_SETTINGS,
                help="Get a WAF log file in CSV format.")
 @click.option("-a", "--action", required=True, default="BLOCK",
               prompt="Please input the action of AWS WAF",
-              type=click.Choice(["BLOCK", "COUNT"]),
+              type=click.Choice(["BLOCK", "COUNT", "EXCLUDED_AS_COUNT"]),
               help="Chose an action type of AWS WAF. The default is \"BLOCK\".")
 @click.option("-d", "--days", required=False, type=int, default="1",
               prompt="Please input the number of analysis target days",
               help="Set a number of the past days until today for analysis target period.")
 @click.option("-s", "--start_time", required=False, type=int,
               help="Set a UNIX time of the oldest time for analysis target period (instead of \"--days\").")
 @click.option("-e", "--end_time", required=False, type=int,
@@ -38,33 +38,37 @@
     else:
         error_file = "[Error] " + CONFIG_FILE + " is not found in the ccurrent directory."
         info_before = "[Info] You may have to run \"accompanist init\" at first."
         ut.colorize_print(error_file, "red")
         ut.colorize_print(info_before, "cyan")
         sys.exit()
 
-    log_group = config_dict["log_group"]
+    log_group = config_dict["destination_name"]
     client = boto3.client("logs")
 
     if action == "BLOCK":
         query = 'fields @timestamp, @message | filter @message like "BLOCK" | sort @timestamp desc'
     elif action == "COUNT":
         query = 'fields @timestamp, @message | filter @message like /"action":"COUNT"/ | sort @timestamp desc'
+    elif action == "EXCLUDED_AS_COUNT":
+        query = 'fields @timestamp, @message | filter @message like "EXCLUDED_AS_COUNT" | sort @timestamp desc'
     else:
         error_action = "[Error] The action is empty or invalid. You should set BLOCK or COUNT"
         ut.colorize_print(error_action, "red")
         sys.exit()
 
     if days is not None and (start_time is None or end_time is None):
         end_time = int(time.time())
         start_time = end_time - days * 24 * 3600
     else:
         days_warning = "[Warning] The inputted number of days is ignored as the start & end times had been set."
         ut.colorize_print(days_warning, "yellow")
 
+    ut.is_valid_days(start_time, end_time)
+
     try:
         start_query_response = client.start_query(
             logGroupName=log_group,
             startTime=start_time,
             endTime=end_time,
             queryString=query,
             limit=10000
@@ -100,36 +104,55 @@
         with open("waf-log.json", mode="w", encoding="utf-8") as f:
             log_str = "[" + str(', '.join(log_json)) + "]"
             json.dump(json.loads(log_str), f, indent=2)
 
         debug_message = "[Debug] A raw log file and the excerpted log file were outputted."
         ut.colorize_print(debug_message, "purple")
 
-    with open("waf-log.csv", mode="w", encoding="utf-8") as f:
+    with open("waf-log.csv", mode="w", encoding="utf-8", newline="") as f:
         writer = csv.writer(f, quoting=csv.QUOTE_NONE, lineterminator="\n", delimiter="\t")
 
         if action == "BLOCK":
             for i in range(len(response["results"])):
                 message = json.loads(response["results"][i][1]["value"])
-                row = str(message["timestamp"]) + "," + \
-                    message["terminatingRuleId"] + "," + \
-                    message["httpRequest"]["uri"] + "," + \
-                    message["httpRequest"]["clientIp"] + "," + \
-                    message["httpRequest"]["country"]
-                writer.writerow([row])
+                if message["action"] == "BLOCK": # to distinguish in logs. it's only for CWL
+                    row = str(message["timestamp"]) + "," + \
+                        message["terminatingRuleId"] + "," + \
+                        message["httpRequest"]["uri"] + "," + \
+                        message["httpRequest"]["clientIp"] + "," + \
+                        message["httpRequest"]["country"] + "," + \
+                        ut.extract_user_agent(message["httpRequest"]["headers"]) + "," + \
+                        ut.extract_rule_id(message["ruleGroupList"])
+                    writer.writerow([row])
         elif action == "COUNT":
             for i in range(len(response["results"])):
                 message = json.loads(response["results"][i][1]["value"])
                 for j in range(len(message["nonTerminatingMatchingRules"])):
                     row = str(message["timestamp"]) + "," + \
                         message["nonTerminatingMatchingRules"][j]["ruleId"] + "," + \
                         message["httpRequest"]["uri"] + "," + \
                         message["httpRequest"]["clientIp"] + "," + \
-                        message["httpRequest"]["country"]
+                        message["httpRequest"]["country"] + "," + \
+                        ut.extract_user_agent(message["httpRequest"]["headers"]) + "," + \
+                        ut.extract_rule_id(message["ruleGroupList"])
                     writer.writerow([row])
+        elif action == "EXCLUDED_AS_COUNT":
+            for i in range(len(response["results"])):
+                message = json.loads(response["results"][i][1]["value"])
+                for j in range(len(message["ruleGroupList"])):
+                    if message["ruleGroupList"][j]["excludedRules"] is not None:
+                        for k in range(len(message["ruleGroupList"][j]["excludedRules"])):
+                            row = str(message["timestamp"]) + "," + \
+                                ut.extract_rule_group(message["ruleGroupList"][j]["ruleGroupId"]) + "," + \
+                                message["httpRequest"]["uri"] + "," + \
+                                message["httpRequest"]["clientIp"] + "," + \
+                                message["httpRequest"]["country"] + "," + \
+                                ut.extract_user_agent(message["httpRequest"]["headers"]) + "," + \
+                                message["ruleGroupList"][j]["excludedRules"][k]["ruleId"]
+                            writer.writerow([row])
         else:
             error_action = "Error: action is invalid"
             ut.colorize_print(error_action, "red")
             sys.exit()
     info_csv = "[Info] A WAF log file in CSV format was outputted."
     ut.colorize_print(info_csv, "cyan")
 
@@ -140,14 +163,15 @@
 
     # Dump data for creating report
 
     sheet_music = {
         "start_time": start_time,
         "end_time": end_time,
         "days": days,
-        "log_group": log_group,
         "action": action,
+        "log_destination": "CWL",
+        "destination_name": log_group,
     }
     with open(SHEET_MUSIC_FILE, mode="w", encoding="utf-8") as f:
         json.dump(sheet_music, f, indent=2)
     info_sheet = "[Info] A " + SHEET_MUSIC_FILE + " file was created for analysis."
     ut.colorize_print(info_sheet, "cyan")
```

## accompanist/cmd_play.py

```diff
@@ -33,33 +33,38 @@
 @click.option("-u", "--utc-offset", required=False, type=int, default=9,
               help="Set a number of UTC offest. The defaut offset is UTC+9 (Asia/Tokyo).")
 @click.option("-y", "--y-limit", required=False, default="50",
               type=click.Choice(["50", "100", "500", "1000"]),
               help="Adjust a Y-axis max limitation for histograms due to many requests.")
 def play(color: str, colorful: str, mask_ip: bool, utc_offset: int, y_limit: str) -> None:
     # Pre-Process
-    if os.path.isfile(INPUT_CSV_FILE):
-        waf_log = pd.read_csv(INPUT_CSV_FILE, header=None)
+    if os.stat(INPUT_CSV_FILE).st_size != 0:
+        if os.path.isfile(INPUT_CSV_FILE):
+            waf_log = pd.read_csv(INPUT_CSV_FILE, header=None)
+        else:
+            error_log = "[Error] A WAF log file, " + INPUT_CSV_FILE + " is not found in the current directory."
+            ut.colorize_print(error_log, "red")
+            sys.exit()
     else:
-        error_log = "[Error] A WAF log file, " + INPUT_CSV_FILE + " is not found in the current directory."
-        ut.colorize_print(error_log, "red")
-        sys.exit()
+        info_color = "[Error] The CSV file, \"waf-log.csv\" is empty. You should confirm a rule action."
+        ut.colorize_print(info_color, "red")
 
-    waf_log.columns = ["time", "rule", "uri", "ip", "country"]
+    waf_log.columns = ["time", "rule", "uri", "ip", "country", "ua", "ruleid"]
 
     plt.rcParams["font.family"] = "Arial"
 
     fig_1 = plt.figure(figsize=A4_SIZE)
     fig_2 = plt.figure(figsize=A4_SIZE)
     fig_3 = plt.figure(figsize=A4_SIZE)
     fig_4 = plt.figure(figsize=A4_SIZE)
     fig_5 = plt.figure(figsize=A4_SIZE)
     fig_6 = plt.figure(figsize=A4_SIZE)
+    fig_7 = plt.figure(figsize=A4_SIZE)
 
-    figs = [fig_1, fig_2, fig_3, fig_4, fig_5, fig_6]
+    figs = [fig_1, fig_2, fig_3, fig_4, fig_5, fig_6, fig_7]
 
     color_list = ["#154f74", "#1397ab", "#9a540f",
                   "#ffa50d", "#74bd97", "#2fcdfa", "#f595ff", "#9a5bc0", "#000000"]
 
     if color is None:
         if colorful:
             index = random.randint(0, len(color_list) - 1)
@@ -70,17 +75,17 @@
             color = "#154f74"  # Default color
 
     # Add front cover
     wf.write_front_cover(fig_1, color)
 
     # Calculation & Draw
     dh.draw_histgram(waf_log, fig_2, utc_offset, y_limit)
-    dp.draw_pie_chart(waf_log, fig_3, fig_4, mask_ip)
-    dt.draw_table(waf_log, fig_5)
-    wc.write_comment(fig_6)
+    dp.draw_pie_chart(waf_log, fig_3, fig_4, fig_5, mask_ip)
+    dt.draw_table(waf_log, fig_6)
+    wc.write_comment(fig_7)
 
     # Post-Process
     wh.write_header_and_footer(waf_log["time"], figs[1:], utc_offset, color)
 
     pdf = pp(OUTPUT_PDF_FILE)
 
     for i in figs:
```

## accompanist/main.py

```diff
@@ -1,21 +1,26 @@
 import click
 
+from accompanist.cmd_hear import hear as hear_cmd
 from accompanist.cmd_init import init as init_cmd
 from accompanist.cmd_listen import listen as listen_cmd
 from accompanist.cmd_play import play as play_cmd
 
 
 @click.group(help="\
         \"Accompanist\" is your accompanist on AWS WAF log analyses.               \
         You can get an AWS WAF log analysis report by the following three commands.\
         (1) $ accompanist init    # Configure CWL log group setting              \
         (2) $ accompanist listen  # Get a WAF log file for analysis              \
-        (3) $ accompanist play    # Analysis WAF logs and generate a report")
+        (3) $ accompanist play    # Analysis WAF logs and generate a report \
+         \
+        (Experimental) $ accompanist hear  # an alternative of listen for S3 \
+        ")
 @click.version_option()
 def cmd() -> None:
     pass
 
 
 cmd.add_command(init_cmd)
 cmd.add_command(listen_cmd)
+cmd.add_command(hear_cmd)
 cmd.add_command(play_cmd)
```

## accompanist/utility.py

```diff
@@ -1,8 +1,50 @@
+import re
+import sys
+
+
 def colorize_print(message: str, color: str) -> None:
     color_dic = {"red": "31m",
                  "green": "32m",
                  "yellow": "33m",
                  "blue": "34m",
                  "purple": "35m",
                  "cyan": "36m"}
     print("\033[" + color_dic[color] + message + "\033[0m")
+
+def extract_user_agent(target_ua: list) -> str:
+    user_agent = "NaN"
+    for i in range(len(target_ua)):
+        if target_ua[i]["name"] == "user-agent" or target_ua[i]["name"] == "User-agent" or target_ua[i]["name"] == "User-Agent":
+            user_agent = str(target_ua[i]["value"])
+
+    extracted_user_agent = re.split('[ ,]', user_agent)
+    if len(extracted_user_agent) > 0:
+        return extracted_user_agent[0]
+    else:
+        return user_agent
+
+def extract_rule_id(rule_group_list: list) -> str:
+    rule_id = "NaN"
+    for i in range(len(rule_group_list)):
+        if rule_group_list[i]["terminatingRule"] is not None:
+            rule_id = rule_group_list[i]["terminatingRule"]["ruleId"]
+    return rule_id
+
+
+def extract_rule_group(rule_group_all_string: str) -> str:
+    if rule_group_all_string.startswith("AWS") is False:
+        match = re.search(r'rulegroup/(.*)/', rule_group_all_string)
+        if match:
+            result = match.group(1)
+        return result
+    else:
+        return rule_group_all_string
+
+def is_valid_days(start: int, end: int) -> None:
+    _days = int(end) - int(start)
+    if _days <= (40 * 24 * 3600):
+        pass
+    else:
+        error_days = "Error: The number of days exceeds 40."
+        colorize_print(error_days, "red")
+        sys.exit()
```

## accompanist/version.py

```diff
@@ -1 +1 @@
-VERSION = "1.1.7"
+VERSION = "1.2.0"
```

## accompanist/report/draw_pie_chart.py

```diff
@@ -13,15 +13,18 @@
     def count_top5(self, target_row: Series) -> Series:
         """
         Calculate top 5 data
         """
         self._data: Series = target_row.value_counts(sort=True) / target_row.value_counts().sum() * 100
         self._top5: Series = self._data[:5]
         self._dropped: Series = self._data.drop(self._top5.index)
-        self._top5["[Others]"] = pd.Series(self._dropped[0:].sum(), dtype="float64").to_string(index=False)
+
+        # Display "Others" if the remain is not 0
+        if self._dropped.shape[0] > 0:
+            self._top5["[Others]"] = pd.Series(self._dropped[0:].sum(), dtype="float64").to_string(index=False)
 
         return self._top5
 
 
 class DrawpieChartClass:
     def __init__(self) -> None:
         self._colors: list = ["#2466a9", "#3f86bf", "#609fc6", "#88b5ce", "#bcd4e5", "#B2B2B2"]  # Blue palette
@@ -37,19 +40,19 @@
                autopct=lambda p: "{: .0f}%".format(p) if p >= 3 else "",
                wedgeprops=self._wedgeprops, textprops=self._textprops, labeldistance=None)
         ax.legend(loc="upper left", bbox_to_anchor=(1.3, 0.94),
                   prop={"size": "16", "weight": "bold"}, frameon=False, ncol=1)
         ax.set_title(title, loc="left", pad=10, fontsize="20", fontweight="bold", color="black")
 
 
-def draw_pie_chart(waf_log_df: DataFrame, fig_a: Figure, fig_b: Figure, mask_ip: bool) -> None:
+def draw_pie_chart(waf_log_df: DataFrame, fig_a: Figure, fig_b: Figure, fig_c: Figure, mask_ip: bool) -> None:
     """
     Draw pie chart for top 5
     """
-    top5: list = [0] * 4
+    top5: list = [0] * 6
 
     calc = CalcTop5Class()
 
     for i in range(len(top5)):
         top5[i] = calc.count_top5(waf_log_df.iloc[:, i + 1])
 
     # Masking IPs
@@ -57,34 +60,41 @@
         top5[2] = (mask_ip_addresses(top5[2]))
     else:
         # Add country code
         top5[2].index = add_cc_to_ip(waf_log_df, top5)
 
     fig_a.subplots_adjust(top=0.8, left=-0.5, hspace=0.2)
     fig_b.subplots_adjust(top=0.8, left=-0.5, hspace=0.2)
+    fig_c.subplots_adjust(top=0.8, left=-0.5, hspace=0.2)
 
     # Add note for country code
-    add_cc_notation(fig_b)
+    add_cc_notation(fig_c)
 
-    ax_a_1: Axes = fig_a.add_subplot(2, 1, 1)
-    ax_a_2: Axes = fig_a.add_subplot(2, 1, 2)
-    ax_b_1: Axes = fig_b.add_subplot(2, 1, 1)
-    ax_b_2: Axes = fig_b.add_subplot(2, 1, 2)
-
-    ax_a_1.set_position([0.004, 0.42, 0.4, 0.3])
-    ax_a_2.set_position([0.004, 0.06, 0.4, 0.3])
-    ax_b_1.set_position([0.004, 0.42, 0.4, 0.3])
-    ax_b_2.set_position([0.004, 0.06, 0.4, 0.3])
+    ax_a_upper: Axes = fig_a.add_subplot(2, 1, 1)
+    ax_a_lower: Axes = fig_a.add_subplot(2, 1, 2)
+    ax_b_upper: Axes = fig_b.add_subplot(2, 1, 1)
+    ax_b_lower: Axes = fig_b.add_subplot(2, 1, 2)
+    ax_c_upper: Axes = fig_c.add_subplot(2, 1, 1)
+    ax_c_lower: Axes = fig_c.add_subplot(2, 1, 2)
+
+    ax_a_upper.set_position([0.004, 0.42, 0.4, 0.3])
+    ax_a_lower.set_position([0.004, 0.06, 0.4, 0.3])
+    ax_b_upper.set_position([0.004, 0.42, 0.4, 0.3])
+    ax_b_lower.set_position([0.004, 0.06, 0.4, 0.3])
+    ax_c_upper.set_position([0.004, 0.42, 0.4, 0.3])
+    ax_c_lower.set_position([0.004, 0.06, 0.4, 0.3])
 
     draw = DrawpieChartClass()
 
-    draw.pie_chart(ax_a_1, top5[0], "Terminating Rule Group")
-    draw.pie_chart(ax_a_2, top5[1], "Path Name")
-    draw.pie_chart(ax_b_1, top5[2], "IP Address")
-    draw.pie_chart(ax_b_2, top5[3], "Country")
+    draw.pie_chart(ax_a_upper, top5[0], "Rule Group")
+    draw.pie_chart(ax_a_lower, top5[5], "Rule")
+    draw.pie_chart(ax_b_upper, top5[1], "Path Name")
+    draw.pie_chart(ax_b_lower, top5[4], "User Agent")
+    draw.pie_chart(ax_c_upper, top5[2], "IP Address")
+    draw.pie_chart(ax_c_lower, top5[3], "Country")
 
 
 def mask_ip_addresses(ip_dataframe: Series) -> Series:
     """
     Mask IP adress if the option was set
     """
     masked_ips: list = []
@@ -110,16 +120,20 @@
     fig_b.text(0.64, 0.13, CC_LINK, fontsize=12, ha="left", color="blue",
                url="https://en.wikipedia.org/wiki/ISO_3166-2")
 
 def add_cc_to_ip(waf_log_df: DataFrame, top5: Series) -> list:
     country: str = ""
     old_index: list = top5[2].index.tolist()
     new_index: list = []
-    for i in range(5):
-        for index, row in waf_log_df.iterrows():
-            if top5[2].index[i] in row["ip"]:
-                country = row["country"]
-                break
-        new_index.append(old_index[i] + "  (" + country + ")")
-    new_index.append(old_index[5])
+    for i in range(len(top5[2].index)):
+        if top5[2].index[i] != "[Others]":
+            for index, row in waf_log_df.iterrows():
+                if top5[2].index[i] in row["ip"]:
+                    country = row["country"]
+                    break
+            new_index.append(old_index[i] + "  (" + country + ")")
+
+    if len(top5[2].index) >= 5:
+        last_index = len(top5[2].index) - 1
+        new_index.append(old_index[last_index])
     return new_index
```

## accompanist/report/write_header_footer.py

```diff
@@ -1,10 +1,11 @@
 import datetime
 import json
 import site
+import sys
 
 import matplotlib.lines as lines
 from matplotlib.figure import Figure
 from matplotlib.offsetbox import AnnotationBbox, OffsetImage
 from pandas.core.series import Series
 from PIL import Image
 
@@ -30,21 +31,30 @@
 
     def header_footer(self, fig: Figure, page_number: str, term: str, main_color: str) -> None:
         with open(SHEET_MUSIC_FILE, mode="r") as f:
             settings_dict: dict = json.load(f)
 
         # Header
         page_title: str = "AWS WAF Log  (Action: " + settings_dict["action"] + ")"
-        log_group = settings_dict["log_group"].replace("aws-waf-logs-", "")
-        if len(log_group) > 15:
-            log_group = log_group[:15] + "*****"
+
+        if settings_dict["log_destination"] == "CWL":
+            log_dest = "Log Group"
+        elif settings_dict["log_destination"] == "S3":
+            log_dest = "Log Bucket"
+        else:
+            sys.exit()
+
+        log_dest_name = settings_dict["destination_name"].replace("aws-waf-logs-", "")
+
+        if len(log_dest_name) > 15:
+            log_dest_name = log_dest_name[:15] + "*****"
         fig.add_artist(lines.Line2D([0, 1], [0.94, 0.94], color=main_color, linewidth=80, zorder=0))
 
         fig.text(0.05, 0.91, page_title, color="#ffffff", fontsize=26, fontweight="bold")
-        fig.text(0.71, 0.82, "Log Group: " + log_group, color="#ffffff", fontsize=14, fontweight="bold", bbox=self._dic_box)
+        fig.text(0.71, 0.82, log_dest + ": " + log_dest_name, color="#ffffff", fontsize=14, fontweight="bold", bbox=self._dic_box)
         fig.text(0.71, 0.76, term, color="#757575", fontsize=14)
 
         # Footer
         fig.add_artist(lines.Line2D([0, 1], [0.0004, 0.0004], color=main_color, linewidth=80, zorder=0))
         fig.text(0.92, 0.02, page_number, color="#949494", fontsize=20, fontweight="bold")
 
         # Show logo file
```

## Comparing `accompanist-1.1.7.dist-info/LICENSE` & `accompanist-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `accompanist-1.1.7.dist-info/METADATA` & `accompanist-1.2.0.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 Metadata-Version: 2.1
 Name: accompanist
-Version: 1.1.7
+Version: 1.2.0
 Summary: Analysis AWS WAF logs and generate a report
 Author: itsuki
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click (>=8.1.3)
 Requires-Dist: boto3 (>=1.26.126)
 Requires-Dist: datetime (>=5.1)
 Requires-Dist: pandas (>=2.0.1)
 Requires-Dist: matplotlib (>=3.7.1)
 Requires-Dist: PdfPages (>=0.1.0)
 
+![](https://user-images.githubusercontent.com/49217613/242336282-bd8df1ff-3a2d-4967-8f0e-de7e9ed7abce.jpg)
 
 [![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-green?style=for-the-badge&logo=appveyor)  ](https://pypi.org/project/accompanist/)  
 
 # Introduction
 ---
 
 ## What is Accomapnist?
 Accompanist is an AWS WAF log analysis tool.  
 It enables you to analyze AWS WAF logs and automatically generate comprehensive analysis reports in just three simple steps. If you're using AWS WAF and CloudWatch Logs, this tool can be helpful for instant log analysis and help you understand the trends of blocked or counted accesses.
 
 - Reporting Items
     - Histgram of requests
         - Total number
-        - Number by each provider
+        - Number by each WAF rule provider
     - Top 5 for the following categories:
         - Rule group
-        - URI Paths
+        - Rule
+        - Paths name
+        - User agent
         - IP addressws
         - Country codes
     - Hit count on specific paths
     - Comment
         - An optional field where you can write additional notes
 
 ## Prerequisite
 
-- Target WAF
-    - AWS WAFv2
-        - Logging: CloudWatch Logs
-        - Action: BLOCK or COUNT
-    - Third Party WAF (using WebACL)
-        - Logging: CloudWatch Logs
-        - Action: BLOCK or COUNT
+- Conditions
+    - WAF: AWS WAFv2 and Third Party WAF (using WebACL)
+    - Logging: CloudWatch Logs or S3
+    - Support Action: BLOCK, COUNT or EXCLUDED_AS_COUNT
 
 - Requirement of Client Environment
     - IAM Role/User: including permissions to execute as follows
         - (1) `start_query` of Logs Insights
         - (2) `get_query_result` of Logs Insights
         - The example policy is noted the last
 
@@ -86,14 +86,24 @@
 ```
 
 ## Uninstall
 
 ```bash
 $ pip uninstall accompanist
 ```
+
+
+# Precaution
+
+- This tool works with AWS WAFv2 and does not support v1.
+- For AWS Managed Rules, you need to append "AWS" to the prefix, or the histogram works wrong.
+- Using the "COUNT" action, the results in double counting.
+- The logs may not be correctly calculated if you use the Label function in WAF.
+
+
 # Subcommnads
 ---
 
 ## init
 
 - Configure a CWL log group setting and more.
 
@@ -132,14 +142,40 @@
   -e, --end_time INTEGER      Set a UNIX time of the latest time for analysis
                               target period (instead of "--days").
   -r, --raw-log               Output raw log file and the excerpted log file
                               for debugging.
   -h, --help                  Show this message and exit.
 ```
 
+## hear
+
+<font color="orange">
+Note: This is experimental feature.
+</font>
+
+- Get a WAF log file in CSV format from S3.
+
+### Usage:
+```bash
+accompanist hear [OPTIONS]
+```
+### Options:
+
+```bash
+  -a, --action [BLOCK|COUNT]  Chose an action type of AWS WAF. The default is
+                              "BLOCK".  [required]
+  -d, --days INTEGER          Set a number of the past days until today for
+                              analysis target period.
+  -s, --start_time INTEGER    Set a UNIX time of the oldest time for analysis
+                              target period (instead of "--days").
+  -e, --end_time INTEGER      Set a UNIX time of the latest time for analysis
+                              target period (instead of "--days").
+  -h, --help                  Show this message and exit.
+```
+
 ## play
 
 - Analysis WAF logs and generate a report.
 
 ### Usage:
 ```bash
 accompanist play [OPTIONS]
@@ -159,17 +195,17 @@
                                   histograms due to many requests.
   -h, --help                      Show this message and exit.
 ```
 
 # Appendix
 ---
 
-## IAM Policy
+## IAM Policy for CWL
 
-Here is a sample of IAM policy with minimum permissions.
+Here is an example of IAM policy with minimum permissions.
 
 ```json
 {
     "Version": "2012-10-17",
     "Statement": [
         {
             "Effect": "Allow",
@@ -185,14 +221,38 @@
         }
     ]
 }
 ```
 
 Note: The `<region>`, `<aws-acount>` and `<log-group-name>` in this sample policy should be replaced.
 
+## IAM Policy for S3
+
+Here is an example of IAM policy with minimum permissions.
+
+```json
+{
+    "Version": "2012-10-17",
+    "Statement": [
+        {
+            "Effect": "Allow",
+            "Action": "s3:ListBucket",
+            "Resource": "arn:aws:s3:::<waf-log-bucket>"
+        },
+        {
+            "Effect": "Allow",
+            "Action": "s3:GetObject",
+            "Resource": "arn:aws:s3:::<waf-log-bucket>/*"
+        }
+    ]
+}
+```
+
+Note: The `<waf-log-bucket>`in this sample policy should be replaced.
+
 ## License
 
 ### The MIT License
 
 Copyright 2023 Itsuki Yutaka
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

## Comparing `accompanist-1.1.7.dist-info/RECORD` & `accompanist-1.2.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 accompanist/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-accompanist/cmd_init.py,sha256=zil_aW0B6trmh_TYZ777_7hc_3LpIHujqC3c1cfNACU,1511
-accompanist/cmd_listen.py,sha256=LEenowGLgxJpwMkUa95xacCKO5BAylDQkerumTEw5aA,6498
-accompanist/cmd_play.py,sha256=fX_fJZY0wPvpKNL1RXOOW3JIMR37Awjy66d1NhxIFlc,3338
-accompanist/main.py,sha256=g3QBePVSozsf-dpiyjXkUui9gUQHXd0g0znMZQL9TQ4,741
-accompanist/utility.py,sha256=FRzk5G0akYlODVy6RJtbLt6xJRZtdonH2UTh5JLY33I,310
-accompanist/version.py,sha256=swSC7Ji8JQdPbrE-3ZFHR4ljb0HO2UsntsDKA7a1Ruc,18
+accompanist/cmd_hear.py,sha256=WuDlI_MYwvDRd6CX1Rvcd-YE3nboJ5UVXR5PUqf71wM,8566
+accompanist/cmd_init.py,sha256=Ca1bNzvhOkcQNcX91JSh3myt2INCVzECcHfFE6wxPys,1970
+accompanist/cmd_listen.py,sha256=Cl4yAm_30cmVg9tw_Kgs7NG6kwRZF0nwAdkPTP-NboM,8281
+accompanist/cmd_play.py,sha256=FEyWOz-GBnC5kwA2aComfiDXsybBpf5q8aicV8RYdg8,3637
+accompanist/main.py,sha256=hr96zLDmADCXCafuwYjNWKUocBio5_vCeyrkhUO89CM,918
+accompanist/utility.py,sha256=KbYEsuL4s9sXpvpBFhTh3hDs2DaxNZO2WaNyf0UMuUM,1630
+accompanist/version.py,sha256=viNrPDalxthAcGDGV3QUhm0tvEB8vd-Uh-27v9_MV7c,18
 accompanist/report/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 accompanist/report/draw_histgram.py,sha256=cYxzjROtITo98QL6M8O98EXKlvM78E-WfE9thsPbzEE,4302
-accompanist/report/draw_pie_chart.py,sha256=74Tml51TqX6A1OMTiUDV5vB0p0gD3ML3ZWTY68GISeU,4578
+accompanist/report/draw_pie_chart.py,sha256=xxDRhpxwKWKukWwNPbM8HBkr3_EygquJ9mmw0M9_RKM,5259
 accompanist/report/draw_table.py,sha256=YZ9PpGS6sLaEgYsqL2Jj5yR7_ng1ywrLEozSlyfnNGQ,3562
 accompanist/report/write_comment.py,sha256=FqGVuAGRlOQry4ThvoB_I_1NtL1A5MFZMRWTI48nq98,1602
 accompanist/report/write_front_cover.py,sha256=lwRs7u17v7NbuoDVS-9TsH0PX0a1WQk-NEzbK3-ez10,1503
-accompanist/report/write_header_footer.py,sha256=siFZ3JRFwJj3oW7TZEOQJfHI6uSuwLPJfqX5kqjPKGA,3645
+accompanist/report/write_header_footer.py,sha256=uUt-bnbp7T4ktYXVu68WupBOVDsQFXtqPQOx2mq0P30,3905
 accompanist/resource/logo_trans.png,sha256=IbkfTLMa9qzSifN32YocbOdpDRecelHA7k8cLrBVK_4,19193
 accompanist/resource/logo_trans_small.png,sha256=SS9AlZGL3Ce-6BbD4EW5rbn7zuDcje7HkEXW_lHE2zs,6761
-accompanist-1.1.7.dist-info/LICENSE,sha256=EHImwl3uAjnXzz33MkVgnfcyDByFp0t6O-H4QaGLs4M,1063
-accompanist-1.1.7.dist-info/METADATA,sha256=4IZLPUWUmvzdLCqHL8bjnwWZx-h7dxvncCG1nR0ehlw,6225
-accompanist-1.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-accompanist-1.1.7.dist-info/entry_points.txt,sha256=gLZwXDl7kf85kYQ1HNQZSxCe81vLub8Eb8wWqrThDeM,53
-accompanist-1.1.7.dist-info/top_level.txt,sha256=vUeFtOUVsBOaqJK8b1z7iVPvaRhz3jGN4Uw79o1o9Ck,31
-accompanist-1.1.7.dist-info/RECORD,,
+accompanist-1.2.0.dist-info/LICENSE,sha256=EHImwl3uAjnXzz33MkVgnfcyDByFp0t6O-H4QaGLs4M,1063
+accompanist-1.2.0.dist-info/METADATA,sha256=RQI5lCdaYkUhE_h2jxBCI3n7g_u9gskGf65Hk82HY-M,7983
+accompanist-1.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+accompanist-1.2.0.dist-info/entry_points.txt,sha256=gLZwXDl7kf85kYQ1HNQZSxCe81vLub8Eb8wWqrThDeM,53
+accompanist-1.2.0.dist-info/top_level.txt,sha256=vUeFtOUVsBOaqJK8b1z7iVPvaRhz3jGN4Uw79o1o9Ck,31
+accompanist-1.2.0.dist-info/RECORD,,
```

