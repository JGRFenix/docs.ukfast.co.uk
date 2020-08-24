
# How does Threat Surveillance work?

Once Threat Surveillance agents are installed on your server(s) they will be automatically configured to deliver the following services.

<div style="text-align: center;">

![how-it-works](files/how-it-works.png)

</div>

## Threat Detection, Attack Protection and log file collation

### Detection
UKFast's Host-Based Intrusion Detection (HIDS) solution, Threat Surveillance, will monitor numerous aspects of your infrastructure to detect suspicious activity. UKFast provide a full list of log locations to be monitored and event types that are collected as standard. Log locations can be customized for your environment, you can work with a UKFast security analyst to find the optimal configuration for your solution.

UKFast have created rule sets which analyse log files from all core technologies such as syslog, MySQL, FTP, Postfix, SSHd, CPanel, MS-auth, Apache, Nginx, PHP and more. These events are parsed through our 2,000+ rules, should a high-level event trigger, an alert will be sent to a nominated email address (or multiple contact addresses) for you to investigate.

If you have the additional Threat SOC service then the UKFast security team will pro-actively investigate the alert and consult with you with recommended mitigating actions.

Additionally, you can [view a dashboard](/security/threatvision/alerts.md), highlighting all activity detected through MyUKFast.

Example rules often triggered:
1.    Multiple attempts to log in to a server followed by a successful authentication
2.    Attempts to escalate account privileges to that of a superuser
3.    SQL Injection attacks
4.    XSS (Cross-Site Scripting) Attacks

Shown below is an example Threat Surveillance email alert. In the below alert, we can see that a SSH Brute Force Attack, a level 10 alert has been detected.

<div style="text-align: center;">

![example-alert](files/example-alert.PNG)

</div>

### Dynamic Protection

Providing real-time protection against incoming attacks, UKFast's Threat Surveillance solution can block attacking IP addresses, through the use of a host-based firewall, such as IPTables (Linux) or Windows firewall. This protection, called Dynamic Protection, will block an attacker for 30 minutes, afterwards, removing the block. Should the attacker continue, the IP address is placed on a global blocklist for 30 days. This global blocklist spans across all customers protected with Threat Surveillance, enabling a wide area of protection, from a wide and varied attack base.

### Log collation

As per PCI-DSS requirements, all collected logs are securely stored on our Threat Surveillance infrastructure for 12 months. The last 3 months of this data is readily accessible and can be accessed through your MyUKFast dashboard.

## File Integrity Monitoring (FIM)

As part of your setup of Threat Surveillance, you can provide UKFast with a list of core system files and directories for which you wish to have [alerts raised](/security/threatvision/alerts) if any changes are made. This is known as File Integrity Monitoring (FIM). A common use of FIM is to ensure payment gateways or redirect pages are not manipulated to divert customer payments elsewhere.

FIM works by taking a hash of each file or utilizing audit processes such as 'AuditD' in Linux and the 'Microsoft Windows audit system', any changes to these files are alerted with the time, date, process and user who made the changes.

File Integrity Monitoring alerts are accessible through MyUKFast, under the 'Alerts' sections on your Threat Surveillance dashboard. Shown below is an example FIM alert in MyUKFast, here we can see what file has changed, when, what process changed the file and exactly what has changed.

<div style="text-align: center;;">

![fim-alert](files/fim-alert.PNG)


</div>


## Rootkit and Malware detection

A "Rootkit" is a combination of software designed to enable administrator-level access to a computer or network, typically with malicious intent. Using deception techniques and interfacing directly with the kernel, rootkits are often very difficult to detect. UKFast's Threat Surveillance can detect common rootkits, searching for suspicious processes with root access to your IT systems. Rootkits are often combined with Malware; there are different types of rootkits but they all attempt to disguise classic Malware activity to prevent Rootkit detection.

Threat Surveillance has been designed to detect rootkits in several ways, for example scanning the /dev directory and file system to detect anomalies, searching for the presence of hidden processes and ports, and scanning system interfaces to detect those in promiscuous mode.

Through close integration with industry-leading Anti Virus scanners, such as McAfee AV and Clam AV, Threat Surveillance can alert you when a detection event has accrued, allowing for rapid response and threat removal from your IT Infrastructure. When coupled with Threat SOC, Threat Surveillance Malware alerts prove to be a powerful tool against viruses and Malware.


## Server Baseline Hardening (available on Linux servers only)

To minimize the threat of an attack on computer infrastructure, a security baseline should be implemented. Our Threat Surveillance solution can scan your servers and compare them to industry-recognized baselines (PCI-DSS, CIS, NIST), to show where security enhancements can be made. Though security vulnerabilities are difficult or even impossible to predict, many of them require multiple conditions to be met at once to be successfully exploited.  Often by changing configuration files and disabling unused services, you can ensure that your infrastructure won't meet these conditions. For Linux servers, we can run baseline scans upon request, providing you with a report of insecure settings that exist on your operating system, along with suggestions on how to improve them.


```eval_rst
   .. title:: How Threat Surveillance Works
   .. meta::
      :title: How Threat Surveillance Works | UKFast Documentation
      :description: Guidance relating to UKFast's Threat Surveillance solution
      :keywords: threat surveillance, alerts, security, compliance, rules, rulesets, ukfast, hosting, file integrity monitoring, rootkit, detection, vulnerability scan, scans, hids, intrusion detection
```
