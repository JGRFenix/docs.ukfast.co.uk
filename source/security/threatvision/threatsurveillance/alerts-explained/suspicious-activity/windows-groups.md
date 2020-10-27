## Windows Groups

*What are windows groups?*

Windows groups are a way to provide permissions to multiple users or computers at once. Microsoft recommends that all permissions should be applied to groups and then the users are added to the groups to get the permissions that they need rather than applying the permissions to the users. This saves time since you can set up groups like the sales team and set the permissions that the sales team need and then just add the users to this group and they receive those permissions.

There are lots of default groups that you might find on a windows environment. Some of the important ones include: 
     * Administrators
     * Domain Administrators
     * Domain Guests
     * Domain Controllers
     * Enterprise Domain Controllers
     * Enterprise Read-only Domain Controllers
     * Remote Desktop Users
     * Server Operators

UKFast Threat Surveillance will monitor all of these and more, to see if any of these change (Have users or computers/servers added or removed from it)

**Rule(s) details**

```eval_rst
+---------------+------------+----------------------------------------------------------------------+
| Rule ID      | Rule Level | Rule Description                                                     |
+==============+============+======================================================================+
| 18210, 60147 | 5          | Windows: Security Enabled Local Group Changed                        |
+--------------+------------+----------------------------------------------------------------------+
| 18211, 60148 | 5          | Windows: Security Enabled Global Group Changed                       |
+--------------+------------+----------------------------------------------------------------------+
| 18213, 60150 | 5          | Windows: Security Enabled Universal Group Changed                    |
+--------------+------------+----------------------------------------------------------------------+
| 18217, 60154 | 12         | Windows: Administrators Group Changed                                |
+--------------+------------+----------------------------------------------------------------------+
| 18218, 60156 | 12         | Windows: Enterprise Domain Controllers Group Changed                 |
+--------------+------------+----------------------------------------------------------------------+
| 18220, 60157 | 5          | Windows: Authenticated Users Group Changed                           |
+--------------+------------+----------------------------------------------------------------------+
| 18221, 60158 | 5          | Windows: Terminal Server Users Group Changed                         |
+--------------+------------+----------------------------------------------------------------------+
| 18222, 60159 | 12         | Windows: Domain Admins Group Changed                                 |
+--------------+------------+----------------------------------------------------------------------+
| 18223, 60160 | 5          | Windows: Domain Users Group Changed                                  |
+--------------+------------+----------------------------------------------------------------------+
| 18225, 60162 | 12         | Windows: Domain Guests Group Changed                                 |
+--------------+------------+----------------------------------------------------------------------+
| 18226, 60163 | 5          | Windows: Domain Computers Group Changed                              |
+--------------+------------+----------------------------------------------------------------------+
| 18227, 60164 | 12         | Windows: Domain Controllers Group Changed                            |
+--------------+------------+----------------------------------------------------------------------+
| 18228, 60165 | 10         | Windows: Cert Publishers Group Changed                               |
+--------------+------------+----------------------------------------------------------------------+
| 18229, 60166 | 12         | Windows: Schema Admins Group Changed                                 |
+--------------+------------+----------------------------------------------------------------------+
| 18230, 60167 | 12         | Windows: Enterprise Admins Group Changed                             |
+--------------+------------+----------------------------------------------------------------------+
| 18231, 60168 | 10         | Windows: Group Policy Creator Owners Group Changed                   |
+--------------+------------+----------------------------------------------------------------------+
| 18232, 60169 | 10         | Windows: RAS and IAS Servers Group Changed                           |
+--------------+------------+----------------------------------------------------------------------+
| 18233, 60170 | 5          | Windows: Users Group Changed                                         |
+--------------+------------+----------------------------------------------------------------------+
| 18234, 60171 | 12         | Windows: Guests Group Changed                                        |
+--------------+------------+----------------------------------------------------------------------+
| 18235, 60172 | 10         | Windows: Power Users Group Changed                                   |
+--------------+------------+----------------------------------------------------------------------+
| 18236, 60173 | 10         | Windows: Account Operators Group Changed                             |
+--------------+------------+----------------------------------------------------------------------+
| 18237, 60174 | 10         | Windows: Server Operators Group Changed                              |
+--------------+------------+----------------------------------------------------------------------+
| 18238, 60175 | 8          | Windows: Print Operators Group Changed                               |
+--------------+------------+----------------------------------------------------------------------+
| 18239, 60176 | 12         | Windows: Backup Operators Group Changed                              |
+--------------+------------+----------------------------------------------------------------------+
| 18240, 60177 | 10         | Windows: Replicators Group Changed                                   |
+--------------+------------+----------------------------------------------------------------------+
| 18241, 60178 | 8          | Windows: Pre-Windows 2000 Compatible Access Group Changed            |
+--------------+------------+----------------------------------------------------------------------+
| 18242, 60179 | 10         | Windows: Remote Desktop Users Group Changed                          |
+--------------+------------+----------------------------------------------------------------------+
| 18243, 60180 | 10         | Windows: Network Confioguration Operators Group Changed              |
+--------------+------------+----------------------------------------------------------------------+
| 18244, 60181 | 10         | Windows: Incoming Forest Trust Builders Group Changed                |
+--------------+------------+----------------------------------------------------------------------+
| 18245, 60182 | 8          | Windows: Performance Monitor Users Group Changed                     |
+--------------+------------+----------------------------------------------------------------------+
| 18246, 60183 | 8          | Windows: Performance Log Users Group Changed                         |
+--------------+------------+----------------------------------------------------------------------+
| 18247, 60184 | 8          | Windows: Authorization Access Group Changed                          |
+--------------+------------+----------------------------------------------------------------------+
| 18248, 60185 | 8          | Windows: Terminal Server License Servers Group Changed               |
+--------------+------------+----------------------------------------------------------------------+
| 18249, 60186 | 8          | Windows: Distributed COM Users Group Changed                         |
+--------------+------------+----------------------------------------------------------------------+
| 18250, 60187 | 12         | Windows: Enterprise Read-Only Domain Controllers Group Changed       |
+--------------+------------+----------------------------------------------------------------------+
| 18251, 60188 | 12         | Windows: Read-Only Domain Controllers Group Changed                  |
+--------------+------------+----------------------------------------------------------------------+
| 18252, 60189 | 12         | Windows: Cryptographic OPerators Group Changed                       |
+--------------+------------+----------------------------------------------------------------------+
| 18253, 60190 | 10         | Windows: Allowed RODC Password Replication Group Changed             |
+--------------+------------+----------------------------------------------------------------------+
| 18254, 60191 | 10         | Windows: Denied RODC Password Replication Group Changed              |
+--------------+------------+----------------------------------------------------------------------+
| 18255, 60192 | 10         | Windows: Event Log Readers Group Changed                             |
+--------------+------------+----------------------------------------------------------------------+
| 18256, 60193 | 10         | Windows: Certificate Service DCOM Access Group Changed               |
+--------------+------------+----------------------------------------------------------------------+

```

```eval_rst
   .. title:: File Monitoring - Windows Groups | UKFast Documentation
   .. meta::
      :title: File Monitoring | UKFast Documentation
      :description: Our Threat Surveillance ruleset explained
      :keywords: threat surveillance, alerts, security, compliance, rules, rulesets, ukfast, hosting, file integrity monitoring, rootkit, detection, vulnerability scan, scans, hids, intrusion detection, windows, 18210, 18211, 18213, 18217, 18218, 18219, 18220, 18222, 18223, 18225, 18226, 18227, 18228, 18229, 18230, 18231, 18232, 18233, 18234, 18236, 18237, 18238, 18239, 18240, 18241, 18242, 18243, 18244, 18245, 18246, 18247, 18248, 18249, 18250, 18251, 18252, 18253, 18254, 18255, 18256, 60147, 60148, 60150, 60154, 60155, 60156, 60157, 60158, 60159, 60160, 60162, 60163, 60164, 60165, 60166, 60167, 60168, 60169, 60170, 60171, 60172, 60173, 60174, 60175, 60176, 60177, 60178, 60179, 60180, 60181, 60182, 60183, 60183, 60184, 60185, 60186, 60187, 60188, 60189, 60190, 60191, 60192, 60193 
```