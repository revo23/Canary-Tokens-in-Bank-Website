# Canary-Tokens-in-Bank-Website

<img width="524" height="524" alt="image" src="https://github.com/user-attachments/assets/0b201f08-bfb0-4c01-8dde-63e71274600c" />  
<br/>
<img width="893" height="416" alt="image" src="https://github.com/user-attachments/assets/c6707157-d065-4118-96ec-972dff3b234c" />
<br/>
<img width="975" height="449" alt="image" src="https://github.com/user-attachments/assets/05cf2f65-9b4a-4583-acf3-185c095d00e9" />
<br/><br/><br/>


Canary tokens are deceptive digital assets, like embedded files or API keys, that act as tripwires to alert you when an attacker accesses them. When an attacker interacts with the token, it triggers an automatic notification, providing valuable information about the intruder, such as their IP address and the time of access. This allows defenders to instantly become aware of a potential breach and gather data to thwart further attacks. 


**Situation**
From Fraudwatch phishing takedowns, it appears some threat actors cloned the banking login page and hosted the on newly created domains to target bank customers in order to obtain banking credentials.
Current Phishtank detections does not appear high-fidelity as it merely uses the regex to match the bank name's string, which resulted in many entries that were not even related to the bank, let alone phishing.

**Task**
As the SOC Analyst on the frontlines doing phishing login page takedowns, I was the most familiar with the situation of a constant phishing domains and looked to reduce the impact of such actions by threat actors whilst enhancing detections.

**Action**
Did a Proof-of-concept (PoC) on a local machine by deploying an obfuscated 'Cloned website Canarytoken' within the JavaScript of copied website (via HTTrack), to see where the attack originated from (source IP) and gain greater visibility into the attackers and any other possible accompanying phishing domains (from Virustotal > relations > passive DNS replication).

**Result**
Althought bank regulatory requirements prevent the implementation of Canary Tokens onto existing live bank login pages, this exercise was useful in understanding threat actor procedures/process of crafting phishing pages.


