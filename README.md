# Password-recovery-with-Johnny-the-ripper-and-Networkwalks-free-tools

# Password Cracking Lab – Week 3 (Project Modules 1 & 2)

This project is part of my Cybersecurity & Ethical Hacking training (Networkwalks).
In Week 3, I completed two labs focused on **password cracking** — testing how
weak passwords protect (or fail to protect) encrypted files such as PDFs.

## 🛠️ Tools Used
- **John the Ripper (JTR)** – CLI password cracker (openwall.com)
- **Johnny GUI** – Graphical front-end for JTR
- **Networkwalks Hash Calculator** – Extracts crackable hashes from protected PDFs
- **Networkwalks Password Cracker** – Recovers passwords from extracted hashes
- **OnlineHashCrack PDF Hash Extractor** – Alternate hash extraction method

## 📋 Project Modules

### Module 1 – Password Cracking with JTR
1. Installed John the Ripper and the Johnny GUI on Windows.
2. Configured Johnny by pointing it to `john.exe` in the run folder.
3. Extracted the `$pdf$2*...` hash from `My Locked PDF1.pdf`.
4. Saved the hash to `hash1.txt` and loaded it into Johnny.
5. Ran "Start new attack" — password recovered: **good-luck**
6. Opened the protected PDF with the cracked password and captured the flag.

 **Module 2 – Password Cracking with Networkwalks Tools**
1. Uploaded `My Locked PDF1.pdf` to the Networkwalks Hash Calculator.
2. Copied the full PDF hash (revision 4, 128-bit key length).
3. Pasted it into the Networkwalks Password Cracker.
4. Recovered the same password: **`password1`**

**Key to Note**
- Encrypted PDFs store their password as a **hash** extractable and crackable.
- Weak, common passwords like `password1` are cracked in seconds.
- **Encryption is two-way** (reversible with a key); **hashing is one-way**
  (verified by matching, not decrypting).
- Strong, long, unique passphrases + MFA are essential.

- Uploaded are screenshot of the exercise for further consideration.


##  References
- John the Ripper: https://www.openwall.com/john/
- Johnny GUI: https://openwall.info/wiki/john/johnny
- Networkwalks Hash Calculator: https://networkwalks.com/hash-calculator/
- Networkwalks Password Cracker: https://networkwalks.com/password-cracker/
