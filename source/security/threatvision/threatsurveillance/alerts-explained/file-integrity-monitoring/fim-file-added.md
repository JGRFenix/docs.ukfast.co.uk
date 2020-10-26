# File Added

When a file is added to the system in a monitored directory or File Integrity Monitoring is configured for a file then an alert will be triggered. These will be level 7 alerts which won't be sent as an email but will appear in MyUKFast. Once this alert is generated we can then monitor that file for any particular changes. 

**Rule(s) details**

```eval_rst
+---------+------------+----------------------------------------------------------------------+
| Rule ID | Rule Level | Rule Description                                                     |
+=========+============+======================================================================+
| 554     | 7          | FIM: File added to the system.                                       |
+---------+------------+----------------------------------------------------------------------+
| 598     | 7          | FIM: Registry Entry Added to the System                              |
+---------+------------+----------------------------------------------------------------------+

```

```eval_rst
   .. title:: File Monitoring - File Added | UKFast Documentation
   .. meta::
      :title: File Monitoring | UKFast Documentation
      :description: Our Threat Surveillance ruleset explained
      :keywords: threat surveillance, alerts, security, compliance, rules, rulesets, ukfast, hosting, file integrity monitoring, rootkit, detection, vulnerability scan, scans, hids, intrusion detection, 554, 598
```