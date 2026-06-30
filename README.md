# Apache Struts S2-045

## Objective

The objective of this lab is to identify and exploit the Apache Struts S2-045 Remote Code Execution (RCE) vulnerability. The assessment demonstrates the process of identifying a vulnerable web application, leveraging a known exploit to achieve remote code execution, and validating the impact of the vulnerability in a controlled environment.

## Skills Learned

- Web application reconnaissance and service enumeration
- Identifying vulnerable Apache Struts applications
- Understanding the Apache Struts S2-045 (CVE-2017-5638) vulnerability
- Remote Code Execution (RCE) exploitation
- Using Metasploit Framework to exploit known vulnerabilities
- Gaining remote access to a compromised system
- Post-exploitation validation and information gathering
- Assessing the security impact of RCE vulnerabilities
- Documenting exploitation methodology and findings

## Tools Used

- Metasploit Framework (msfconsole)
- Kali Linux Terminal
- Searchsploit / Exploit-DB

## Step

Clone the lab repository using the following command: 

bash:
```
https://github.com/SamSothavy/Apache-Struts-S2-045-lab.git
```

After cloning the repository, start the lab environment using Docker.

If the Docker containers start successfully, you should see output similar to the example below:

<img width="1715" height="643" alt="Screenshot 2026-06-30 131557" src="https://github.com/user-attachments/assets/e1e8ba52-1edb-473d-b480-a21ae8363520" />

As we know S2-045 is a critical Remote Code Execution (RCE) vulnerability (CVE-2017-5638) in the Apache Struts2 framework

<img width="1715" height="914" alt="Screenshot 2026-06-30 132308" src="https://github.com/user-attachments/assets/2f924d3b-4c47-4db8-a65b-0f9b273edf62" />

Apache Struts Jakarta Multipart Parser OGNL Injection is a critical vulnerability where a malicious Content-Type header causes the multipart parser to fail, and the resulting error message is incorrectly evaluated as an OGNL expression. This allows an attacker to execute arbitrary code on the server, leading to full remote compromise.

<img width="1713" height="469" alt="Screenshot 2026-06-30 132625" src="https://github.com/user-attachments/assets/f8359d93-caa1-4407-8da9-fa8eb28fdda8" />

<img width="1711" height="945" alt="Screenshot 2026-06-30 134855" src="https://github.com/user-attachments/assets/b1d19a6d-c24d-4322-a30d-0a93508c1a4e" />

After configuring all the required options, we try exploit

<img width="1715" height="483" alt="Screenshot 2026-06-30 135135" src="https://github.com/user-attachments/assets/b466d305-480a-4615-8a67-cd643161ee09" />

<img width="1708" height="946" alt="Screenshot 2026-06-30 135236" src="https://github.com/user-attachments/assets/63e89cc1-8f69-4260-9271-a77b66262058" />





