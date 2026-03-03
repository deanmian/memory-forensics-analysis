# Memory Forensics Analysis – Malware Incident Investigation

## Overview

This project presents a memory forensics investigation performed on a Windows virtual machine that was compromised after a user opened a malicious email attachment disguised as a PDF.

The objective was to identify indicators of compromise (IOCs), analyze suspicious processes, and reconstruct the infection activity using memory analysis techniques.

⚠️ This analysis was conducted in a controlled academic lab environment for educational purposes.

---

## Scenario

A user reported suspicious activity after opening a PDF received via email. Shortly after, unusual behavior was observed on the system, including potential unauthorized financial activity.

A memory dump was acquired from the affected machine for forensic analysis.

---

## Tools Used

- Volatility 2
- pdfid.py
- strings
- xxd
- Hashing utilities (MD5/SHA)
- WHOIS lookup
- Kali Linux analysis environment

---

## Methodology

The investigation followed standard DFIR practices:

1. Memory image integrity validation via hashing  
2. Process enumeration and anomaly detection  
3. Identification of injected or suspicious processes  
4. Extraction and inspection of suspicious artifacts  
5. Analysis of temporary files related to the infection chain  
6. Basic network attribution of observed connections  

---

## Key Findings

- Evidence of process injection into legitimate Windows processes  
- Recovery of a suspicious PDF-related artifact from memory (TEMP location)  
- Indicators consistent with malware execution following the phishing scenario  
- Network indicators identified through connection analysis  

📄 Full technical report available in Spanish in the repository.

---

## Repository Contents

- `report.pdf` → Full forensic report (Spanish)
- `images/` → Supporting screenshots and evidence excerpts

---

## Notes

This repository is intended for educational and research purposes only.  
No original malware samples or full memory dumps are distributed.

---

## Author

Daniel Demian  
Computer Engineering Student | Aspiring Cybersecurity Analyst
