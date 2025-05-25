# Keberoasting-
Simulation attack. 

## 🛠 PART-1 Executing Rebeus. 
This command uses Rubeus to request service tickets (TGS) for all accounts with SPNs in the domain, then saves the Kerberos ticket hashes to spn.txt for offline cracking.
![Rebeus](Kerberoasting-PART1.png) 
## 🔗 PART-2 Sharing File. 
I shared the file using smb. 
![File-Share](PART2.SHRING-SPN.TXT.WITHLINUXMACHINE.png)
## 📥PART-3 Downloading file from Kali machine. 
![File-Get](PART3downloading-SPN.TXT-FROMKALI.png)
## 🔓 PART-4 Using hashcat
This command uses Hashcat to crack Kerberoast hashes (mode 13100) from spn.txt using the wordlist passwords.txt. Cracked passwords are saved to cracked.txt 🔓
![Hashcat](Part4-KEBEROSTING.png)
## 💥🔓 PART-5 Password Cracked 
We got the password. 
![Password](CONTRASEÑA%CRACKEADA.png)
## 📄🔍 PART-6 
I started reviewing the logs  to look for suspicious activity. While analyzing Event ID 4769, which logs Kerberos service ticket requests, I noticed unusual patterns that could indicate a Kerberoasting attempt. These logs helped me identify accounts that were being targeted.
![ ]()
