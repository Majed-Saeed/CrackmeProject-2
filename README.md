# CrackmeProject – ELF Reverse Engineering Challenge

This repository contains a simple **ELF x86 crackme binary** analyzed as part of my reverse engineering practice.  
The goal of the challenge was to identify the correct password using static analysis with **Ghidra**.

---

## 🔍 Overview

The challenge provides an ELF binary (`ch1.bin`) that asks the user for a password.  
By reversing the binary in Ghidra, I located the internal comparison routine and extracted the hardcoded password.

This project demonstrates my ability to:
- Analyze x86 ELF binaries  
- Use Ghidra for decompilation and symbol exploration  
- Understand program flow and string comparison logic  
- Apply reverse-engineering methodology

---

## 🛠 Tools Used

| Tool | Purpose |
|------|---------|
| **Ghidra 11.x** | Disassembly & decompiler analysis |
| **Linux (VMware)** | Binary execution & testing |
| **Terminal utilities** | Running ELF binaries |

Screenshots of the analysis are included in this repository.

---

## 📂 Repository Structure



├── ch1.bin # ELF x86 crackme binary
├── Pasted image.png # Ghidra analysis screenshot
├── Pasted image (2).png # Execution screenshot
└── README.md # Documentation


---

## 🔬 Reverse Engineering Summary

After loading the binary in Ghidra, the program flow shows:

- Displaying a welcome banner  
- Requesting user input via `getString`  
- Comparing input using `strcmp` against a hardcoded string  

Ghidra revealed the password inside the code:

### ✔️ Extracted Password:


123456789


Entering this value validates the challenge successfully.

---

## ▶️ Running the Binary

```bash
chmod +x ch1.bin
./ch1.bin


Enter the extracted password when prompted.

🎯 Key Takeaways

Practical ELF reverse engineering

Understanding binary logic and comparison functions

Applying Ghidra effectively

Strengthening RE and software security skills

📫 Contact

GitHub: https://github.com/Majed-Saeed
