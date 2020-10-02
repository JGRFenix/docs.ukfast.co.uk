=====================================
Threat Surveillance
=====================================

Threat Surveillance from UKFast is our tailored, all in one HIDS/SIEM system that enables you to continually monitor for malicious activity on your IT environment. Collating and parsing logs from critical services like SSH, RDP and web traffic, Threat Surveillance can hunt down and block attackers automatically, while providing you with real-time alerts of threat activity.

.. toctree::
   :maxdepth: 1

   How does it work? <how-it-works>
   system-requirements
   getting-started
   Installing on a UKFast hosted server <ukfast-hosted-install>
   Installing on a non-UKFast hosted server <non-ukfast-install>
   pci-dss
   alerts
   Alert remediation tips <alert-remediation-tips/index>


How does Threat Surveillance link into PCI-DSS?
************************************************

As per control 12.4.1 of the PCI-DSS standards, businesses that accept card payments are required to employ a form log collection to allow activity to be tracked in the event of a breach.

UKFast's Threat Surveillance handles this for you. By collecting all your server's logs and sending them to our Threat Surveillance infrastructure, we can parse these logs for threats and store them securely for 12 months, as required the PCI-DSS requirements.

This easy, no-fuss solution to this, and many other PCI-DSS requirements ensure your business is compliant and ready to take card payments online.

What attacks can Threat Surveillance detect?
************************************************
As Threat Surveillance is installed onto your servers, it can easily detect and protect against a wide variety of attacks. We employ an advanced ruleset of bespoke detection rules that can identify attacks such as:

* Brute-force attacks
* SQL Injection
* XSS (Cross-Site Scripting)
* Shellshock
* Path Traversal
* Code Injection
* Version Gathering
* Network Scanning/Mapping
* Challange-Response Exploits
* SSH CRC-32 Compensation attacks
* Invalid DNS packets
* Ping of death
* Replay Attacks
* Buffer Overflow attacks
* Rootkits
* Malware and Viruses
* WordPress attacks
* osCommerce Login Bypass attacks
* phpMyAdmin Scans
* POST Bots
* Website Scraping

Any many more...

How will I be alerted?
*****************************

Threat Surveillance alerts can be easily viewed in the form on an email, sent directly from our real-time alerting system. These alerts will contain a brief description of the attack/alert, the agent (your server) IP address and the full log event detailing the attacks. Threat Surveillance alerts can also be found in MyUKFast, paired with additional information.

You can also view a breakdown report of live threat events in your MyUKFast Threat Surveillance dashboard.

.. meta::
     :title: Threat Surveillance and Threat Response | UKFast Documentation
     :description: Guidance relating to UKFast's Threat Surveillance and Threat Response solutions
     :keywords: Threat Monitoring, security, compliance, ukfast, hosting, file integrity monitoring, rootkit, detection, vulnerability scan, scans, hids, intrusion detection, threat response
