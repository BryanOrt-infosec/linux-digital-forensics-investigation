# Digital Forensics Investigation of a Suspicious File in Ubuntu

## Project Overview

This project demonstrates a beginner-friendly digital forensics investigation performed in Ubuntu Linux using native command-line tools. The goal of the project was to simulate the analysis of a suspicious file discovered on a Linux system and document the investigative process in a structured, professional manner.

The investigation focused on identifying the file type, preserving evidence integrity through hashing, examining the contents of the file, extracting readable strings, searching for suspicious indicators, and documenting forensic findings.

This project was designed to strengthen practical skills in Linux, cybersecurity, and incident investigation while building a portfolio-ready artifact for GitHub.

---

## Objective

The objective of this project was to perform a basic forensic review of a suspicious file and identify potential indicators of malicious activity.

Specifically, this project aimed to:

- Create and organize a simple forensic investigation workspace in Ubuntu
- Examine a suspicious file using Linux command-line tools
- Generate a SHA-256 hash to preserve file integrity
- Search for indicators such as credentials, IP addresses, and suspicious commands
- Document findings in a professional investigation notes file
- Present the work clearly using screenshots and written analysis

---

## Scenario

A suspicious file was discovered on a Linux system during a routine review. As the analyst, I was tasked with examining the file, identifying any suspicious indicators, and documenting the results.

The file contained potential evidence of:
- plaintext credentials
- a private IP address
- an SSH remote access command
- suspicious wording suggesting possible malicious intent

Because the file contained potentially sensitive and suspicious information, it was treated as evidence and analyzed using basic forensic techniques.

---

## Tools Used

This investigation was completed using built-in Ubuntu/Linux utilities:

- `file`
- `sha256sum`
- `cat`
- `strings`
- `grep`
- `nano`

These tools were selected because they are lightweight, accessible to beginners, and commonly used in Linux-based analysis workflows.

---

## Project Structure

```text
it-forensics-project/
├── evidence/
│   ├── suspicious_file.txt
│   └── investigation_notes.txt
├── screenshots/
│   ├── 01-project-folders.png
│   ├── 02-suspicious-file-created.png
│   ├── 03-file-type-check.png
│   ├── 04-sha256-hash.png
│   ├── 05-file-contents.png
│   ├── 06-strings-output.png
│   ├── 07-password-search.png
│   ├── 08-ip-search.png
│   ├── 09-ssh-search.png
│   ├── 10-malicious-phrase-search.png
│   ├── 11-investigation-notes.png
│   └── 12-final-folder-structure.png
└── README.md


## Investigation Steps

### 1. Created the Project Workspace

Commands used:

mkdir it-forensics-project  
cd it-forensics-project  
mkdir evidence  
mkdir screenshots  
ls  
```
![Project Workspace](screenshots/01-project-folders.png)

---

### 2. Identify the File Type

Command used:

file suspicious_file.txt


![File Type](screenshots/03-file-type-check.png)

---

### 3. Generate SHA256 Hash

Command used:

sha256sum suspicious_file.txt

![SHA256 Hash](screenshots/04-sha256-hash.png)

---

### 4. View File Contents

Command used:

cat suspicious_file.txt

![File Contents](screenshots/05-file-contents.png)

---

### 5. Extract Strings

Command used:

strings suspicious_file.txt

![Strings Output](screenshots/06-strings-output.png)

---

### 6. Search for Password

Command used:

grep "password" suspicious_file.txt

![Password Search](screenshots/07-password-search.png)

---

### 7. Search for IP Address

Command used:

grep "192.168.1.50" suspicious_file.txt

![IP Search](screenshots/08-ip-search.png)

---

### 8. Search for SSH Command

Command used:

grep "ssh" suspicious_file.txt

![SSH Search](screenshots/09-ssh-search.png)

---

### 9. Search for Suspicious Phrase

Command used:

grep "steal data" suspicious_file.txt

![Malicious Phrase](screenshots/10-malicious-phrase-search.png)

---

### 10. Investigation Notes

The findings were documented in a notes file.

![Investigation Notes](screenshots/11-investigation-notes.png)

---

## Conclusion

This project demonstrates how Linux command-line tools can be used to perform a basic digital forensics investigation, identify suspicious indicators, and document findings in a structured manner.
