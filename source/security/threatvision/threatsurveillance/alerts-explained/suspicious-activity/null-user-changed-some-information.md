# Null user changed some information

**What does this mean?**


To understand this rule, it's best if we first break down what is meant by null. As you probably know, null is the name given when a value is empty or not present. For example, if we have a variable that is called My_name but we have not saved and data into this variable, this variable will have a value of null or nothing. 

Building on this, when information is changed on your server, the operating system will usually track what user or what process changed that information, for tracking and management purposed. On this occasion, the operating system was unable to determine why or what changed this information, this could be potentially malicious. 

A common objective for an attacker is to remain anonymous as possible, for as long as possible, so they can do as much damage as they can. Preventing the Operating System from tracking what user or process is making changes to specific information can help the attacker to remain anonymous.

This anomalous activity can help us identify that some unexpected activity may be in progress.

Let's not forget however that is it entirely possible that a program/service may have entered an error state or not correctly properly changed the information, not telling the operating system that I changed some information and triggering this alert as a false positive.

**What do I need to do if I receive this alert?**


If you receive this alert, we recommend being extra vigilant and looking out for any other alerts that may be triggered as a result of a potential attackers activity. Your MyUKFast dashboard is a great place to keep track of events on your server. Additionally, UKFast support is always on hand to provide assistance where needed.

Multiple authentication failures from the same IP address followed by success.


**What does this rule mean?**


This is an all-round rule for alerting on multiple failed authentication attempts, followed by a successful login. This is triggered when a user tried to log in multiple times before succeeding. This can indicate that an attacker accessed your server through a brute force attack. Alternatively, this could indicate that a service/process on your solution was unable to authenticate onto this server for a small period. It is also possible that a genuine user has forgotten their password, and has tried many times to authenticate, then remembered their password and logged in.

It's always best to double-check the user account in question and take the appropriate measures to check that this was a genuine login. If you are unsure about this login, one of the quickest ways to take preventative action is to disable the added user account. For more information on this, please see the documentation here.

Additionally, to minimize these alerts and secure your server from this type of brute force attack, it's recommended to lock down access to these services. SSHd, for example, can be locked down to certain IP addresses at a firewall level. This means that only predefined IP addresses will be able to access the SSH port, securing access to this service. A VPN could also be used. More information on this can be found here.

Its best practice to ensure you have a strong password set for all these services. Passwords longer than 8 characters that contain numbers, wildcards and MixEd CaSe letters are very difficult to brute force. You can use a service like AuditD to enforce password strength policies on your server. You can contact UKFast Support for assistance on this.


**Rule(s) details**

```eval_rst
+---------+------------+----------------------------------------------------------------+
| Rule ID | Rule Level | Rule Description                                               |
+=========+============+================================================================+
| 40105   | 12         | "Null" user changed some information.                          |
+---------+------------+----------------------------------------------------------------+
```


```eval_rst
.. meta::
     :title: Null user changed some information | UKFast Documentation
     :description: Threat Surveillance ruleset explained
     :keywords: threat surveillance, alerts, security, compliance, rules, rulesets, detection, hids, intrusion detection, suspicious activity, suspicious, 40105

