# Keberoasting-
Simulation attack. 

## 🛠 PART1. Executing Rebeus. 
This command uses Rubeus to request service tickets (TGS) for all accounts with SPNs in the domain, then saves the Kerberos ticket hashes to spn.txt for offline cracking.
![Rebeus](Kerberoasting-PART1.png) 
## PART2. Sharing File. 
I shared the file using smb. 
![File-Share](PART2.SHRING-SPN.TXT.WITHLINUXMACHINE.png)
## PART3. Downloading file from Kali machine. 
![File-Get](PART3downloading-SPN.TXT-FROMKALI.png)
## 🔓 PART4 Using hashcat
This command uses Hashcat to crack Kerberoast hashes (mode 13100) from spn.txt using the wordlist passwords.txt. Cracked passwords are saved to cracked.txt 🔓
![Hashcat]()
