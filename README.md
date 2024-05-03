# CVE-2024-29988-exploit
Exploit for Microsoft SmartScreen malicious execution (april 2024)

## Description
A critical vulnerability, CVE-2024-29988, has been discovered in Microsoft's April 2024 Patch Tuesday release. 
This vulnerability allows threat actors to bypass Microsoft's Mark of the Web (MotW) feature, enabling them to execute arbitrary code. 
Peter Girnus, a senior threat researcher at Trend Micro's Zero Day Initiative (ZDI), has observed attackers leveraging this vulnerability in the wild.

Microsoft SmartScreen Prompt contains a security feature bypass vulnerability that allows an attacker to bypass the Mark of the Web (MotW) feature. 
This vulnerability can be chained with CVE-2023-38831 and CVE-2024-21412 to execute a malicious file.

## Published Date: 03.05.2024

## 🔥 CVSS Score: 10/10

## Details of CVE
To exploit CVE-2024-29988, attackers utilize a zipped file containing the exploit code and payload to evade EDR/NDR detection. 
The exploit is sent to the target, whereupon extraction and execution of the payload, the vulnerability allows bypassing MotW. 
Attackers can then execute desired commands or payloads with the bypassed security controls.

## Running Instructions
To execute the exploit, use the provided Python script with the following command:

```python
python3 exploit.py -t http://10.10.10.10 -c 'command'
```

Before running the exploit, refer to the README.txt file in the repository for detailed instructions.

## Disclaimer
For educational purposes only.
