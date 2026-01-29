# ZIP Password Cracking Practice (John the Ripper)

This repository documents a learning practice of cracking a password-protected ZIP file using **John the Ripper** and the **RockYou** wordlist.

**Ethical Reminder**  
This practice is for educational purposes only and must be performed on files you own or have permission to test.

---

## Tools Used

- John the Ripper
- zip2john
- RockYou wordlist
- Kali Linux

---

## Usage

```bash 
git clone https://github.com/md-samrat/zipfile-cracking.git
cd zipfile-cracking
zip2john secret.zip > hashsecret.txt (optional :already have you can remove the exist hashsecret.txt)
john --wordlist=/usr/share/wordlists/rockyou.txt --rules hashsecret.txt
john --show hashsecret.txt 
