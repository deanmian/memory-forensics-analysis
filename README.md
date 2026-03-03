# Memory Forensics Analysis – Malware Incident Investigation

## Overview

This project presents a memory forensics investigation performed on a Windows virtual machine that was intentionally infected in a controlled laboratory environment.

The scenario simulates a phishing incident in which a user opened a malicious email attachment disguised as a PDF, leading to system compromise.

⚠️ The company name used in this case study (ETOLEPSED S.A.) is entirely fictitious and used solely for educational purposes.

⚠️ All analysis was conducted in an isolated academic environment.

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

This project was developed for educational and research purposes within an academic digital forensics module.

- The organization referenced (ETOLEPSED S.A.) is fictional.
- The analyzed system was part of a controlled lab environment.
- No real user data or production systems were involved.
- No original malware samples or full memory dumps are distributed.

This repository is intended strictly for learning and portfolio demonstration.

---

## Author

Daniel Demian  
Computer Engineering Student | Aspiring Cybersecurity Analyst
