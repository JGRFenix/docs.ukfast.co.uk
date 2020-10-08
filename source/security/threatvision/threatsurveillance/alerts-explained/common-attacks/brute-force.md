# Brute Force

**What is a brute force attack?**


One of the most common forms of attack is a brute force attack. As its name suggests, this attack is a relentless attempt to gain access to a system by constantly trying user name and password combinations to guess the correct credentials.

A simple brute force attack will try many commonly used usernames and password combinations. For example, the user name admin or administrator coupled with passwords like password, admin or change.

We also see more sophisticated brute force attacks that can detect what service they are trying to gain access to, and then try common user name and password combinations for that service, or even try the default credentials for that service. For example, an SSH or PHPMyAdmin Brute Force attack will usually try the username root, as this the most common user name used by default. Another example could be the administrator for Windows RDP 

**How can I prevent a brute force attack?**


A successful brute force attack can easily be avoided by ensuring a strong user name and password combination is used. For more information on this, please consider reading our guide on how to set secure usernames and passwords here.

One of the best ways to mitigate these attacks is to remove the attacker's access to affected services completely. We can do this by implementing restriction rules to only allow safe, trusted IP addresses to access certain services and ports. By restricting access to SSH, for example, we can ensure that only trusted locations/IP addresses can access SSH and run commands on our server(s). For more information and a step by step guide on creating firewall rules, please follow our documentation here.

**Rule(s) details**

```eval_rst
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| Rule ID | Rule Level | Rule Description                                                                                                      |
+=========+============+=======================================================================================================================+
| 3910    | 10         | Courier brute force (multiple failed logins).                                                                         |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 5712    | 10         | sshd: brute force trying to get access to the system.                                                                 |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 9351    | 10         | Horde brute force (multiple failed logins).                                                                           |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 9403    | 10         | Roundcube brute force (multiple failed logins).                                                                       |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 9751    | 9          | Dovecot brute force attack (multiple auth failures).                                                                  |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 9820    | 10         | vm-pop3d: POP3 brute force (multiple failed logins).                                                                  |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 9951    | 9          | vpopmail: brute force (multiple failed logins).                                                                       |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 9952    | 9          | vpopmail: brute force (email harvesting).                                                                             |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 9953    | 9          | vpopmail: brute force (empty password).                                                                               |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 11251   | 10         | proftpd: FTP brute force (multiple failed logins).                                                                    |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 11306   | 10         | pure-ftpd: FTP brute force (multiple failed logins).                                                                  |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 11451   | 10         | vsftpd: FTP brute force (multiple failed logins).                                                                     |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 11510   | 10         | MS-FTP: FTP brute force (multiple failed logins).                                                                     |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 31510   | 9          | CMS (WordPress or Joomla) brute force attempt.                                                                        |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 51004   | 6          | Dropbear: dropbear brute force attempt.                                                                               |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 51007   | 10         | Dropbear: brute force attempt.                                                                                        |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 51011   | 10         | Dropbear: dropbear brute force attempt for nonexistent user.                                                          |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 64252   | 10         | sshd: brute force trying to get access to the system.                                                                 |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 86806   | 12         | VShell multiple connection attempts within 2 minute by a host in the deny file, potential DOS or brute force attempt. |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 87202   | 10         | Proxmox VE brute force (multiple failed logins).                                                                      |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 87302   | 10         | ownCloud brute force (multiple failed logins).                                                                        |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 87507   | 6          | Exim brute force attack (multiple auth failures).                                                                     |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 87602   | 10         | OpenVAS (gsad) brute force (multiple failed logins).                                                                  |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 87610   | 10         | OpenVAS (openvasmd) brute force (multiple failed logins).                                                             |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 88203   | 10         | NextCloud brute force (multiple failed logins).                                                                       |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 100014  | 9          | RDP: Brute force attack                                                                                               |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 200235  | 6          | CPanel: Cpanel (Cpaneld) Brute Force attempt                                                                          |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 200236  | 6          | CPanel: Web Mail (webmaild) Brute Force attempt                                                                       |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 200237  | 6          | CPanel: WHM (whostmgrd) Brute Force attempt                                                                           |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 300227  | 9          | CMS (WordPress or Joomla) brute force attempt.                                                                        |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
| 300271  | 8          | WordPress XML RPC POST Brute Force Attack                                                                             |
+---------+------------+-----------------------------------------------------------------------------------------------------------------------+
```


```eval_rst
.. meta::
     :title: Brute force Attacks | UKFast Documentation
     :description: Threat Surveillance ruleset explained
     :keywords: threat surveillance, alerts, security, compliance, rules, rulesets, detection, hids, intrusion detection, bruteforce, brute force, 3910, 5712, 9351, 9403, 9751, 9820, 9951, 9952, 9953, 11251, 11306, 11451, 11510, 31510, 51004, 51007, 51011, 64252, 86806, 87202, 87302, 87507, 87602, 87610, 88203, 100014, 200235, 200236, 200237, 300227, 300271 
