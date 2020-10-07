=====================================
Threat Scan
=====================================

.. raw:: html

   <div style="text-align: center;">


.. image:: files/threat-scan.png
   :width: 128
   :alt: ThreatScan

.. raw:: html

   </div>

------------

Threat Scan is our base tier, providing a robust, clear and concise vulnerability scanning platform that can be used to hunt down security holes in your environment via external vulnerability scans. Threat Scan allows for unlimited scans to be ran either on demand or on a schedule, allowing around the clock scanning.

.. toctree::
   :maxdepth: 2

   targets
   launching-a-scan
   managing-scans

Our Threat Scan platform allows you to run both internal and external vulnerability scans, both evaluate based of the PCI DSS 3.2.1 baseline standard.

**What is an External scan?**

An external scan simulates what an attacker would see when scanning your environment for vulnerabilities to exploit. With this information at hand, you can easily implement recommended solutions to mitigate the vulnerability, such as applying patches/updates, making configuration changes or implementing additional security controls into your application.

UKFast recommends that external scans be performed at least every 2 weeks to maintain viability of your environment's vulnerabilities.

**What is an Internal scan?**

Internal scans are also available for UKFast hosted servers when paired with Threat Surveillance. These internal scans use a lightweight software agent installed into your endpoint to scan the running operating system for vulnerabilities. This access to the system allows under the hood vulnerabilities to be found that are not directly exposed to the outside word. For example, internal scans may highlight outdated software, missing kernel patches, misconfigured services and malicious processes.

UKFast recommends that internal scans be performed at least every 2 weeks to maintain viability of your environment's vulnerabilities.

.. meta::
   :title: Threat Scan | UKFast Documentation
   :description: Guidance on Threat Vision from UKFast
   :keywords: security, threat, monitoring, monitoring, scan, surveillance, soc, response, alerts, blocking, hacking, ransomware, protection