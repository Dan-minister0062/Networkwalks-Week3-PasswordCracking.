<div align="center">
🔐 NETWORKWALKS CYBERSECURITY INTERNSHIP
WEEK 3 — PDF PASSWORD SECURITY & CRYPTOGRAPHY
Batch B082 | Practical Lab Report & Evidence
![John the Ripper](https://img.shields.io/badge/Tool-John%20the%20Ripper-red?style=for-the-badge)
![Networkwalks](https://img.shields.io/badge/Tool-Networkwalks%20Tools-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
</div>
---
📌 Project Overview
During Week 3 of the NETWORKWALKS Cybersecurity Internship, I carried out a practical exercise focused on PDF password security, hash extraction, and dictionary-based password recovery.
The objective was to examine the security of an encrypted PDF by extracting its password hash and testing whether a dictionary attack could recover the password. To compare two approaches, I completed the exercise with:
John the Ripper (JTR) — a local password-auditing tool, using the Johnny graphical interface.
Networkwalks (NW) online tools — the Hash Calculator and Password Cracker.
Both approaches successfully recovered the test PDF password. The recovered value is documented in the results section below.
> **Scope note:** This was an educational exercise performed on the supplied/test PDF as part of the internship. Password recovery should only be attempted on files that you own or are explicitly authorized to assess.
🎯 Objectives
Understand how password-protected PDF files store password-verification data.
Extract a PDF hash for password-auditing purposes.
Use John the Ripper/Johnny to perform a dictionary attack locally.
Use the Networkwalks Hash Calculator and Password Cracker to repeat the test online.
Compare the outcomes of the two methods.
Document the process with organized screenshot evidence.
🧰 Tools & Technologies
Tool	Purpose
John the Ripper (Jumbo)	Local password auditing and dictionary attack
Johnny GUI	Graphical frontend for John the Ripper
Networkwalks Hash Calculator	Extract the hash from the test PDF
Networkwalks Password Cracker	Test the extracted hash with a dictionary attack
Encrypted PDF	Test file used for the authorized exercise
---
🧪 Part 1 — John the Ripper (JTR)
Evidence: 14 screenshots — `JTR-01` to `JTR-14`.
The first method used a local password-auditing workflow. The PDF hash was extracted and supplied to John the Ripper through the Johnny interface. A dictionary attack was then performed against the extracted hash.
Workflow
Prepared the encrypted test PDF for analysis.
Extracted the PDF password hash in the `$pdf$` format.
Configured and opened Johnny, the graphical frontend for John the Ripper Jumbo, on Windows.
Loaded the extracted hash into the password-auditing workflow.
Ran a dictionary attack.
Confirmed that the password was recovered and used it to open the test PDF.
JTR Screenshot Evidence
Click any screenshot to open the original full-size image.
<a href="https://github.com/user-attachments/assets/110c95d8-db2f-4027-ba3d-8b49025cbe34"><img src="https://github.com/user-attachments/assets/110c95d8-db2f-4027-ba3d-8b49025cbe34" alt="John the Ripper evidence 01" width="48%"></a>
<a href="https://github.com/user-attachments/assets/b2ba1971-8678-4fbe-b703-b28ee0bd5301"><img src="https://github.com/user-attachments/assets/b2ba1971-8678-4fbe-b703-b28ee0bd5301" alt="John the Ripper evidence 02" width="48%"></a>
<a href="https://github.com/user-attachments/assets/f662cf0e-153c-4591-8c9a-5f3aff82005b"><img src="https://github.com/user-attachments/assets/f662cf0e-153c-4591-8c9a-5f3aff82005b" alt="John the Ripper evidence 03" width="48%"></a>
<a href="https://github.com/user-attachments/assets/2eddb788-9cce-4606-abee-339acedb2908"><img src="https://github.com/user-attachments/assets/2eddb788-9cce-4606-abee-339acedb2908" alt="John the Ripper evidence 04" width="48%"></a>
<a href="https://github.com/user-attachments/assets/8813feb0-09b3-42e6-85c2-de91fd603f95"><img src="https://github.com/user-attachments/assets/8813feb0-09b3-42e6-85c2-de91fd603f95" alt="John the Ripper evidence 05" width="48%"></a>
<a href="https://github.com/user-attachments/assets/fa080fb1-92d7-4a45-9a42-c4de6af6be0e"><img src="https://github.com/user-attachments/assets/fa080fb1-92d7-4a45-9a42-c4de6af6be0e" alt="John the Ripper evidence 06" width="48%"></a>
<a href="https://github.com/user-attachments/assets/65966297-338a-4556-9a2d-3bd58be1e564"><img src="https://github.com/user-attachments/assets/65966297-338a-4556-9a2d-3bd58be1e564" alt="John the Ripper evidence 07" width="48%"></a>
<a href="https://github.com/user-attachments/assets/672e6f5e-0ab0-4a51-85c0-5fb6764ad969"><img src="https://github.com/user-attachments/assets/672e6f5e-0ab0-4a51-85c0-5fb6764ad969" alt="John the Ripper evidence 08" width="48%"></a>
<a href="https://github.com/user-attachments/assets/8c65c364-2264-4bb7-9cc2-4e2ea107b0a9"><img src="https://github.com/user-attachments/assets/8c65c364-2264-4bb7-9cc2-4e2ea107b0a9" alt="John the Ripper evidence 09" width="48%"></a>
<a href="https://github.com/user-attachments/assets/340a2fc1-909c-45b1-a0c0-c814b8986ef8"><img src="https://github.com/user-attachments/assets/340a2fc1-909c-45b1-a0c0-c814b8986ef8" alt="John the Ripper evidence 10" width="48%"></a>
<a href="https://github.com/user-attachments/assets/d9925ba8-62c8-4637-84ef-499523185773"><img src="https://github.com/user-attachments/assets/d9925ba8-62c8-4637-84ef-499523185773" alt="John the Ripper evidence 11" width="48%"></a>
<a href="https://github.com/user-attachments/assets/143ce2c6-30be-4dd9-abb5-15122ac2316d"><img src="https://github.com/user-attachments/assets/143ce2c6-30be-4dd9-abb5-15122ac2316d" alt="John the Ripper evidence 12" width="48%"></a>
<a href="https://github.com/user-attachments/assets/ef33dfd6-4a64-485c-bdab-45df6c09eae0"><img src="https://github.com/user-attachments/assets/ef33dfd6-4a64-485c-bdab-45df6c09eae0" alt="John the Ripper evidence 13" width="48%"></a>
<a href="https://github.com/user-attachments/assets/0f353cf5-32de-4bbf-aadb-86fc92e3da74"><img src="https://github.com/user-attachments/assets/0f353cf5-32de-4bbf-aadb-86fc92e3da74" alt="John the Ripper evidence 14" width="48%"></a>
---
🌐 Part 2 — Networkwalks (NW) Online Tools
Evidence: 7 screenshots — `NW-01` to `NW-07`.
The second method used the online tools provided by Networkwalks. This allowed the same PDF password-recovery exercise to be carried out through a browser-based workflow.
Workflow
Opened the Networkwalks Hash Calculator.
Submitted the authorized test PDF and extracted its hash.
Copied the resulting hash.
Opened the Networkwalks Password Cracker.
Submitted the hash and ran the built-in dictionary attack.
Recovered the password and used it to unlock the PDF and capture the flag.
Networkwalks Screenshot Evidence
Click any screenshot to open the original full-size image.
<a href="https://github.com/user-attachments/assets/8979a3ae-d7d1-4c2c-8bc3-557bc7686deb"><img src="https://github.com/user-attachments/assets/8979a3ae-d7d1-4c2c-8bc3-557bc7686deb" alt="Networkwalks tool evidence 01" width="48%"></a>
<a href="https://github.com/user-attachments/assets/b06467ae-a392-4502-ade9-b3bd00428195"><img src="https://github.com/user-attachments/assets/b06467ae-a392-4502-ade9-b3bd00428195" alt="Networkwalks tool evidence 02" width="48%"></a>
<a href="https://github.com/user-attachments/assets/302c9bbc-8a66-45d5-8306-f12a25aac272"><img src="https://github.com/user-attachments/assets/302c9bbc-8a66-45d5-8306-f12a25aac272" alt="Networkwalks tool evidence 03" width="48%"></a>
<a href="https://github.com/user-attachments/assets/5c6e2a84-5780-4913-9f92-bbffe62cc759"><img src="https://github.com/user-attachments/assets/5c6e2a84-5780-4913-9f92-bbffe62cc759" alt="Networkwalks tool evidence 04" width="48%"></a>
<a href="https://github.com/user-attachments/assets/c0148e17-fa4a-4f6b-a056-c896f46b3bad"><img src="https://github.com/user-attachments/assets/c0148e17-fa4a-4f6b-a056-c896f46b3bad" alt="Networkwalks tool evidence 05" width="48%"></a>
<a href="https://github.com/user-attachments/assets/24c6ccb7-6040-4230-878d-313a08a5383e"><img src="https://github.com/user-attachments/assets/24c6ccb7-6040-4230-878d-313a08a5383e" alt="Networkwalks tool evidence 06" width="48%"></a>
<a href="https://github.com/user-attachments/assets/3c5d7a39-7add-412f-97cc-0f614e0fd2fc"><img src="https://github.com/user-attachments/assets/3c5d7a39-7add-412f-97cc-0f614e0fd2fc" alt="Networkwalks tool evidence 07" width="48%"></a>
---
🏁 Results & Comparison
Test method	Approach	Outcome
John the Ripper / Johnny	Local hash-based dictionary attack	Password recovered
Networkwalks tools	Online hash extraction and dictionary attack	Password recovered
Recovered test password: `password1`
Both methods recovered the same password and allowed the protected PDF to be opened. This demonstrates how a weak, commonly used password can be vulnerable to dictionary-based guessing.
🔎 Security Lessons
A password that is common or predictable can be recovered by automated guessing.
Password length and uniqueness matter; avoid dictionary words, predictable patterns, and reused passwords.
Use a long, unique passphrase or a password manager to generate and store strong passwords.
Apply encryption with a strong password when protecting sensitive PDF documents.
Treat extracted password hashes as sensitive security material and do not publish them.
📄 Full Technical Report
The detailed report contains the project background, objectives, methodology, comparison of both approaches, findings, security recommendations, and a clickable evidence index.
➡️ Open / Download the Week 3 Technical Report (PDF)
📁 Suggested Repository Structure
```text
Networkwalks-Week-3/
├── README.md
├── Week3_Report.pdf
└── Screenshots/
    ├── John-the-Ripper/
    │   ├── JTR-01.png
    │   ├── ...
    │   └── JTR-14.png
    └── Networkwalks-Tools/
        ├── NW-01.png
        ├── ...
        └── NW-07.png
```
The screenshot gallery above uses the original GitHub attachment links. If you also download the images into the folders shown above, you can replace the remote image URLs with relative repository paths later.
⚖️ Ethical Use & Disclaimer
This project was completed for educational and authorized cybersecurity training. Password-auditing tools must only be used on files and systems that you own or have explicit permission to assess. Do not use these techniques to access another person's protected documents.
🙌 Acknowledgement
Thanks to NETWORKWALKS for the practical learning opportunity and hands-on exposure to password security and cryptographic auditing.
<div align="center">
Learning by doing. Building practical cybersecurity skills.
</div>
