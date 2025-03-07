
# **Wi-Fi Password Cracking Tool**

This tool automates Wi-Fi WPA/WPA2 password cracking using `aircrack-ng` and supports password generation, brute-force attacks, and logging cracked credentials to your devices.

---

## **Features**

1. **Multiple Password Generation Modes**
   - **Password List File**: Use an existing password list to attempt cracking.
   - **Brute-force 8-Digit Numbers**: Generate sequential, descending, or random numeric combinations.
   - **Bangladeshi Mobile Numbers**: Check combinations for specific mobile number prefixes.
   - **Name + Random Characters**: Generate passwords based on a base name and random characters.

2. **Aircrack-ng Automation**
   - Automates the execution of `aircrack-ng` with generated passwords.
   - Detects successful cracks and displays the Wi-Fi password.

3. **Password Logging**
   - Saves cracked passwords to a predefined location: `Found_handshake/`.

4. **User-Friendly Interface**
   - ASCII banners, success messages, and interactive menus make the tool easy to use.

5. **Internet Connectivity Check**
   - Ensures an active internet connection before execution.

---

## **Download**

Click [here](https://items.kesug.com/Product/product-24) to download the latest version of the tool.(2.0 Version)

---

## **Dependencies**

### **Required Tools**
- `aircrack-ng` (must be installed and available in the system PATH). You can install from telegram [here](https://t.me/SQBeh/2)

### **Python Libraries**
Install the required libraries using `pip`:

```bash
pip install requests colorama
```

---

## **Termux Usage**

1. **Install to Your Devices**
     ```bash
     git clone https://github.com/SQBEHPS2/WPA2-Cracking
     ```
   **Copy Handshake:**
     You need to copy of handshake pcap or hccapx file to tools folder.
     ```bash
     cp <Address of Handshake file> ~/WPA2-Cracking/
     ```
   **Use Password Dictionary:**
     If you check password with your dictionary password. Make sure copy dictionary to tools folder. Copy dictionary with run the command.
     ```bash
     cp <Address of Dictionary> ~/WPA2-Cracking/
     ```
   **Run the Script**  
     ```bash
     python wpa2-cracking.py
     ```

2. **Choose an Option**  
   On startup, you’ll see the main menu:
   ```
   Choose an option:
   1: Use a password list file
   2: Brute-force 8-digit numbers
   3: Check Bangladeshi mobile numbers
   4: Name + Letter characters generation
   5: About
   ```

3. **Option Breakdown**  
   - **Option 1**: Provide a path to a password list file.
   - **Option 2**: Generate 8-digit numeric passwords (ascending, descending, or random).
   - **Option 3**: Generate mobile number combinations for Bangladeshi prefixes.
   - **Option 4**: Generate passwords based on a base name and random letters/characters.

4. **Monitor Progress**  
   Once started, the tool will attempt to crack the Wi-Fi password using `aircrack-ng`.

5. **Results**  
   - Successful passwords are displayed with a success banner.
   - Passwords are saved in the `Found_handshake/` folder.


## **Important Notes**

- **Legal Disclaimer**: This tool is intended for educational purposes and authorized penetration testing only. Unauthorized use to crack Wi-Fi networks is illegal.


---

## **Screenshots**

- Success Banner Example:
```
══════════════════════════════════════════════════════════════════════════════
                       ✨ 🎆 PASSWORD SUCCESSFULLY CRACKED! 🎆 ✨
══════════════════════════════════════════════════════════════════════════════

                      🌟         🔐 PASSWORD: 12345678 🔐         🌟

══════════════════════════════════════════════════════════════════════════════

          💾 Your password has been saved at: Found_handshake/example.txt 💾

══════════════════════════════════════════════════════════════════════════════

                  🎉 🎈 CONGRATULATIONS ON YOUR SUCCESS! 🎈 🎉
══════════════════════════════════════════════════════════════════════════════
```

---

## **Credits**

- Developed by: **SQB EHPS**
- **YouTube**: [@SQBEHPS](https://www.youtube.com/@SQBEHPS)  
- **GitHub**: [github.com/SQBEHPS](https://github.com/SQBEHPS)  
- **Second GitHub**: [github.com/SQBEHPS2](https://github.com/SQBEHPS2)  
- **Facebook**: [SQB EHPS Service](https://facebook.com)

---

## **License**

This project is licensed under the MIT License. Use responsibly.
