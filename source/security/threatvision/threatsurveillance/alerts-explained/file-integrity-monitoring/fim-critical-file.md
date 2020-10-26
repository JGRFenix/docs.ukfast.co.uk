# Critical File Changes

Critical File Changes are files that are considered to be extremely important. Due to this for these alerts you will receive an email as well as in the alerts page in MyUKFast. We can also set custom files as critical so that you will receive emails if these files are updated. Like all FIM alerts if you have Threat SOC these will get passed to our Threat SOC team to investigate and will have all the same information as a normal File Changed alert. 

**Rule(s) details**

```eval_rst
+---------+------------+----------------------------------------------------------------------+
| Rule ID | Rule Level | Rule Description                                                     |
+=========+============+======================================================================+
| 100345  | 12         | Changes to /etc/passwd - Critical file!                              |
+---------+------------+----------------------------------------------------------------------+
| 100346  | 12         | Changes to /etc/shadow - Critical file!                              |
+---------+------------+----------------------------------------------------------------------+
| 100347  | 12         | Changes to /root/.ssh/authorized_keys - Critical file!               |
+---------+------------+----------------------------------------------------------------------+
| 100348  | 12         | Changes to /etc/ssh/sshd_config - Critical file!                     |
+---------+------------+----------------------------------------------------------------------+
| 100349  | 12         | Changes to /etc/sudoers - Critical file!                             |
+---------+------------+----------------------------------------------------------------------+
| 100352  | 6          | Whitelisted process 'Cpanel' made changes to a critical file         |
+---------+------------+----------------------------------------------------------------------+
| 100353  | 6          | Whitelisted process 'Unison' made changes to a critical file         |
+---------+------------+----------------------------------------------------------------------+
| 100354  | 6          | Whitelisted process 'Plesx PSA' made changes to a critical file      |
+---------+------------+----------------------------------------------------------------------+
| 100355  | 6          | Whitelisted process 'CPanel' made changes to a critical file         |
+---------+------------+----------------------------------------------------------------------+
| 100356  | 6          | NIDS Module Deployment change a critical file                        |
+---------+------------+----------------------------------------------------------------------+
| 100359  | 12         | Changes to critical file - <Path Name>                               |
+---------+------------+----------------------------------------------------------------------+
| 100370  | 12         | Critical Magento /app/ File Change! - <Path Name>                    |
+---------+------------+----------------------------------------------------------------------+
| 100371  | 12         | Critical Magento /lib/ File Change! - <Path Name>                    |
+---------+------------+----------------------------------------------------------------------+
| 100372  | 12         | Changes to /usr/local/cpanel/logs/panic_log - Critical file!         |
+---------+------------+----------------------------------------------------------------------+
| 100375  | 12         | FIM: Changes to critical file - <Path Name>                          |
+---------+------------+----------------------------------------------------------------------+
```

```eval_rst
   .. meta::
      :title: File Monitoring - Critical File Changes | UKFast Documentation
      :description: Our Threat Surveillance ruleset explained
      :keywords: threat surveillance, alerts, security, compliance, rules, rulesets, ukfast, hosting, file integrity monitoring, rootkit, detection, vulnerability scan, scans, hids, intrusion detection, 100345, 100346, 100347, 100348, 100349, 100352, 100353, 100354, 100355, 100356, 100359, 100370, 100372, 100375
```