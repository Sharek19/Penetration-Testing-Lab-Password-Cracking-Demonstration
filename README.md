# Penetration Testing Lab: Password Cracking Demonstration

## Overview

This project demonstrates ethical penetration testing techniques by performing a password cracking exercise on a simulated leaked shadow file. The lab was conducted in a controlled environment to evaluate the strength of password policies and to understand the methods an attacker might use in real-world scenarios. All data used in this project is fictitious and provided for educational purposes only.

## Project Description

In this lab, a shadow file containing hashed passwords was used to simulate a real-world penetration testing scenario. The objective was to use various password cracking techniques to identify weak credentials. The methods employed include:

- **Dictionary Attacks:** Using wordlists to match common passwords.
- **Hybrid Attacks:** Combining a wordlist with mask rules to account for simple modifications (like appending a digit or symbol).
- **Brute Force (Incremental):** Applying exhaustive search where necessary.

The successfully cracked passwords are saved in a file named `cracked.txt` in the format `username:password`.

## Tools and Technologies Used

- **John the Ripper:** The primary tool used to crack password hashes.
- **Wordlists:** Various publicly available wordlists were used as the basis for the dictionary attacks.
- **Linux Environment:** The lab was performed on an Ubuntu VM to provide a controlled and isolated environment.
- **Multi-Core Processing:** The `--fork` option in John the Ripper was used to leverage multiple CPU cores and speed up the cracking process.

## Lab Methodology

1. **Preparation:**
   - A simulated leaked shadow file was provided, containing hashed passwords (using the MD5 crypt format).
   - The file was processed to extract username and hash pairs.
  
![image](https://github.com/user-attachments/assets/2260fb60-3ade-48e0-9e0f-a17acd6fd7b7)
   

2. **Password Cracking:**
   - **Dictionary Attack:** Run John the Ripper with wordlists and mutation rules.
   - **Hybrid Attack:** Combine the wordlist with mask options to capture common variations.
   - **Incremental Mode:** Optionally, brute force remaining password spaces if needed.

![image](https://github.com/user-attachments/assets/3e04faf4-045f-41a9-b4ab-4637adb1bea8)


3. **Results:**
   - The cracked credentials were stored in `cracked.txt` in the following format:
   
![image](https://github.com/user-attachments/assets/501111ee-9707-407c-a53e-b58baee07477)


## Ethical Considerations

- **Controlled Environment:** This exercise was conducted in a lab setting using simulated data to ensure no real systems or sensitive data were compromised.
- **Educational Purpose:** The project is designed purely for educational purposes, to understand how attackers may exploit weak passwords and to improve defensive security practices.
- **Responsible Use:** The techniques demonstrated are to be used only in authorized environments. Unauthorized password cracking is illegal and unethical.

## Disclaimer

This project is for **educational purposes only**. All password cracking activities were performed on fictitious data in a controlled lab environment. The methods demonstrated should not be applied to any real systems without explicit permission.
