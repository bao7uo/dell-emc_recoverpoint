# Dell EMC RecoverPoint

## Exploits for an enterprise data protection platform

I have discovered the following vulnerabilities in the RecoverPoint enterprise data protection platform, mentioned in Dell EMC's disclosure.
- http://seclists.org/fulldisclosure/2018/May/61

#### Critical unauthenticated remote code execution with root privileges via unspecified attack vector (CVE-2018-1235, CVSS 9.8, critical severity)
- Permits an attacker with visibility of a RecoverPoint device on the network to gain complete control over the underlying Linux operating system.

#### Administrative menu arbitrary file read (CVE-2018-1242, CVSS 6.7, medium severity)
- An attacker with access to the boxmgmt administrative menu can read files from the file system which are accessible to the boxmgmt user.
- [Exploit here](https://github.com/bao7uo/dell-emc_recoverpoint/blob/master/EMC_RPT_CVE-2018-1242.md)

#### LDAP credentials in Tomcat log file (CVE-2018-1241, CVSS 6.2, medium severity)
- In certain conditions, RecoverPoint will leak plaintext credentials into a log file.

## Exploits for third party vulnerabilities

These are exploitation techniques I have found for vulnerabilities I did not discover

CVE-2018-1185 - An OS command injection vulnerability resulting in code execution as the built-in admin user
- [Exploit here](https://github.com/bao7uo/dell-emc_recoverpoint/blob/master/EMC_RPT_CVE-2018-1185.md)

More to follow
