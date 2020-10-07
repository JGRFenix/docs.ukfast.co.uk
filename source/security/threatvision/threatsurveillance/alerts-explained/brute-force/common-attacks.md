

## Brute Force Attacks

*What is a brute force attack?*


One of the most common forms of attack is a brute force attack. As its name suggests, this attack is a relentless attempt to gain access to a system by constantly trying user name and password combinations to guess the correct credentials.

A simple brute force attack will try many commonly used usernames and password combinations. For example, the user name admin or administrator coupled with passwords like password, admin or change.

We also see more sophisticated brute force attacks that can detect what service they are trying to gain access to, and then try common user name and password combinations for that service, or even try the default credentials for that service. For example, an SSH or PHPMyAdmin Brute Force attack will usually try the username root, as this the most common user name used by default. Another example could be the administrator for Windows RDP 

*How can I prevent a brute force attack?*


A successful brute force attack can easily be avoided by ensuring a strong user name and password combination is used. For more information on this, please consider reading our guide on how to set secure usernames and passwords here.

One of the best ways to mitigate these attacks is to remove the attacker's access to affected services completely. We can do this by implementing restriction rules to only allow safe, trusted IP addresses to access certain services and ports. By restricting access to SSH, for example, we can ensure that only trusted locations/IP addresses can access SSH and run commands on our server(s). For more information and a step by step guide on creating firewall rules, please follow our documentation here.

## Multiple viruses detected - Possible outbreak.


*What does this rule mean?*


Triggered when more than 8 virus detection events occur during a 360 second period, this rule could indicate that a malware/virus outbreak has occurred. This can occur when a particularly resistant piece of malware has managed to make its way onto your server, and is either replicating itself or is allowing a flood of viruses to be installed onto the system.

This rule will trigger even if your virus/malware scanner has successfully removed the infection(s). To check this out, you can view your alerting history for virus detection events, view your virus malware scanners logs, or contact UKFast support for assistance.

*How can I remediate this.*


If the viruses/malware was not removed by your scanner, you need to jump into action and remove as many infections items as possible. Please refer to this page for more information on how to do this, or contact UKFast support for assistance.

If the viruses/malware has been removed by your scanner, its recommended to immediately run another virus/malware scan to try and detect any missed infections. Then, consult with your developers and UKFast support to secure your server in the future.

```eval_rst
.. meta::
     :title: Common Attacks | UKFast Documentation
     :description: Our Threat Monitoring ruleset explained
     :keywords: threat monitoring, alerts, security, compliance, rules, rulesets, ukfast, hosting, file integrity monitoring, rootkit, detection, vulnerability scan, scans, hids, intrusion detection, set up

