.. meta::
   :title: File Integrity Monitoring | UKFast Documentation
   :description: Guidance on Threat Surveillance Alerts
   :keywords: threat surveillance, alerts, security, compliance, rules, rulesets, detection, hids, intrusion detection, exploit attempts, exploit

=====================================
File Integrity monitoring
=====================================

File Integrity Monitoring alerts can be found in the 'Alerts' section of your MyUKFast area. Critical File Changes are also sent as an email alert to the selected contacts. Both of these alert types will contain important information regarding the event.

By default, File Integrity Monitoring scans run every 12 hours and will alert when the MD5/SHA1/SHA256 sum of monitored files change, prompting for further investigation. This is useful however it can sometimes be difficult to investigate these alerts as little information is captured.

To combat this, realtime monitoring can be configured, utilising 'Auditd' on Linux systems and Windows Auditing. When realtime FIM is configured, changes to these files are reported within 30 seconds. Additionally, extra data such as what user changed the file, what the effective user was (for example root if sudo was used), the process name that changed the file, and what exactly what changed is provided in the alert.

With this additional information, a File Change Alert can easily be recognised as suspicious or as a false positive. The needed action can then be taken quickly by either yourself or by the Threat SOC Team when coupled with our Threat SOC service for active alert investigation. 


.. toctree::
   :maxdepth: 2
   fim-critical-file
   fim-file-added
   fim-file-changed
   fim-file-deleted
   