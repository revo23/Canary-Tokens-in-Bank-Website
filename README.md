# Canary-Tokens-in-Bank-Website

<img width="324" height="324" alt="image" src="https://github.com/user-attachments/assets/0b201f08-bfb0-4c01-8dde-63e71274600c" />
sample image  

**Situation**
From Fraudwatch phishing takedowns, it appears some threat actors cloned the banking login page and hosted the on newly created domains to target bank customers in order to obtain banking credentials.
Current Phishtank detections does not appear high-fidelity as it merely uses the regex to match the bank name's string, which resulted in many entries that were not even related to the bank, let alone phishing.

**Task**
As the SOC Analyst on the frontlines doing phishing login page takedowns, I was the most familiar with the situation of a constant phishing domains and looked to reduce the impact of such actions by threat actors whilst enchancing detections.

**Action**
Do a Proof-of-concept (PoC) on a local machine by deploying an obfuscated 'Cloned website Canarytoken' within the JavaScript of copied website (via HTTrack), to see where the attack originated from (source IP) and gain greater visibility into the attackers and any other possible accompanying phishing domains (from Virustotal > relations > passive DNS replication).


**Result**
Althought bank regulatory requirements prevent the implementation of Canary Tokens onto existing live bank login pages, this exercise was useful in understanding threat actor procedures and the process of crafting phishing pages.


