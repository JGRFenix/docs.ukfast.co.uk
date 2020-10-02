# System Requirements

To ensure the best possible experience, Threat Surveillance may only be installed on systems that meet or exceed the below system requirements. These requirements may be subject to change as Threat Surveillance improves.

If you have any questions regarding the below or would like further information regarding a custom installation, please [contact UKFast support](https://my.ukfast.co.uk/pss/create).

### Hardware requirements

Please refer to the below compatibility matrix before installing Threat Surveillance onto a server to understand what hardware is required.

```eval_rst
+---------------------+-----------------------+
|       Hardware      |      Requirement      |
+=====================+=======================+
| System Architecture | x86                   |
+---------------------+-----------------------+
| CPU Cores           | 2 (Dual-core) or more |
+---------------------+-----------------------+
| CPU Speed           | 1Ghz or more          |
+---------------------+-----------------------+
| Memory (RAM)        | 2GB or more           |
+---------------------+-----------------------+
| Free disk space     | 8GB or more           |
+---------------------+-----------------------+
| Disk Speed          | 600 IOPS or more      |
+---------------------+-----------------------+
```

### Virtual Servers

Threat Surveillance may also be installed onto virtual servers. 

OS Container-based servers and applications containers (Such as docker) are not currently supported. 

Please refer to the below compatibility matrix before installing Threat Surveillance onto a virtual server to understand what virtualization types are supported. Any virtualization not mentioned below are not supported.

If you don't know your virtual server's virtualisation type, please contact your hosting provider for more information. Additionally, the below commands may be able to show you your system's virtualisation type on a Linux system.

`hostnamectl status`

`dmidecode -s system-product-name`

```eval_rst
+---------------------+-----------+
| Virtualization Type | Supported |
+=====================+===========+
| KVM                 | Yes       |
+---------------------+-----------+
| vmware              | Yes       |
+---------------------+-----------+
| hyperv              | Yes       |
+---------------------+-----------+
| xen                 | No        |
+---------------------+-----------+
| openvz              | No        |
+---------------------+-----------+
| LXC/LXD             | No        |
+---------------------+-----------+
| AWS                 | No        |
+---------------------+-----------+
```

Please note Threat Surveillance does **not** support cloud services such as Amazon AWS, Microsoft Azure or Google Cloud.

### Operating System compatibility matrix

Please refer to the below compatibility matrix before installing Threat Surveillance onto a server to understand which Threat Surveillance modules may be installed onto a target server. 

Threat Surveillance Core is required, any other modules are optional but highly recommended for full protection.

```eval_rst
+---------------------+---------------+-------------------+--+------+-------------+
|   Operating System  | UKFast Hosted | Non-UKFast Hosted |  | Core | NIDS Module |
+=====================+===============+===================+==+======+=============+
| Centos 6            | Yes           | Yes               |  | Yes  | No          |
+---------------------+---------------+-------------------+--+------+-------------+
| Centos 7            | Yes           | Yes               |  | Yes  | Yes         |
+---------------------+---------------+-------------------+--+------+-------------+
| Centos 8            | Yes           | Yes               |  | Yes  | Yes         |
+---------------------+---------------+-------------------+--+------+-------------+
| RHEL 6              | Yes           | Yes               |  | Yes  | Yes         |
+---------------------+---------------+-------------------+--+------+-------------+
| RHEL 7              | Yes           | Yes               |  | Yes  | Yes         |
+---------------------+---------------+-------------------+--+------+-------------+
| RHEL 8              | Yes           | Yes               |  | Yes  | Yes         |
+---------------------+---------------+-------------------+--+------+-------------+
| Ubuntu 16.04        | Yes           | Yes               |  | Yes  | Yes         |
+---------------------+---------------+-------------------+--+------+-------------+
| Ubuntu 18.04        | Yes           | Yes               |  | Yes  | Yes         |
+---------------------+---------------+-------------------+--+------+-------------+
| Ubuntu 20.04        | Yes           | Yes               |  | Yes  | Yes         |
+---------------------+---------------+-------------------+--+------+-------------+
| Debian 8            | Yes           | Yes               |  | Yes  | Yes         |
+---------------------+---------------+-------------------+--+------+-------------+
| Debian 9            | Yes           | Yes               |  | Yes  | Yes         |
+---------------------+---------------+-------------------+--+------+-------------+
| Windows Server 2012 | Yes           | No                |  | Yes  | No          |
+---------------------+---------------+-------------------+--+------+-------------+
| Windows Server 2016 | Yes           | No                |  | Yes  | No          |
+---------------------+---------------+-------------------+--+------+-------------+
| Windows Server 2019 | Yes           | No                |  | Yes  | No          |
+---------------------+---------------+-------------------+--+------+-------------+
```

**Any operating systems not mentioned above are not supported.**


```eval_rst
   .. title:: Threat Surveillance system requirements
   .. meta::
        :title: Threat Surveillance system requirements | UKFast Documentation
        :description: UKFast Threat Surveillance system requirements
        :keywords: Threat Surveillance, alerts, security, compliance, rules, rulesets, ukfast, hosting, file integrity monitoring, rootkit, detection, vulnerability scan, scans, hids, intrusion detection, set up
