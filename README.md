🔐 Networkwalks Week 3 – PDF Password Security & Cryptography
Password Hash Extraction and Dictionary-Based Password Recovery
<p align="center">
  <img src="https://img.shields.io/badge/Networkwalks-Cybersecurity%20Internship-blue?style=for-the-badge" alt="Networkwalks Internship"/>
  <img src="https://img.shields.io/badge/Batch-B082-success?style=for-the-badge" alt="Batch B082"/>
  <img src="https://img.shields.io/badge/Week-03-orange?style=for-the-badge" alt="Week 3"/>
  <img src="https://img.shields.io/badge/Focus-PDF%20Password%20Security-purple?style=for-the-badge" alt="PDF Password Security"/>
</p>
---
📌 Project Overview
This repository documents my Week 3 practical cybersecurity project as part of the Networkwalks Cybersecurity Internship (Batch B082).
The project focuses on PDF password security, hash extraction, and dictionary-based password recovery. The objective was to examine the strength of a password-protected PDF by extracting its password hash and testing whether a dictionary attack could recover the password.
To compare two different approaches, I completed the practical exercise using:
John the Ripper (JTR) with Johnny GUI – a local password-auditing workflow.
Networkwalks (NW) online tools – the Hash Calculator and Password Cracker.
Both methods successfully recovered the password used for the test PDF. The recovered password was then used to open the document and capture the flag.
🎯 Project Objectives
Understand the role of password hashes in protected PDF documents.
Extract a PDF password hash in the supported `$pdf$` format.
Configure and use John the Ripper Jumbo through the Johnny graphical interface.
Perform a dictionary attack using a local password-auditing tool.
Extract a PDF hash using the Networkwalks Hash Calculator.
Test the extracted hash using the Networkwalks Password Cracker.
Compare the results of local and web-based password-auditing methods.
Document the practical workflow with clearly separated screenshot evidence.
📚 Practical Activities Completed
Activity	Description	Status
Local password auditing	PDF hash extraction and dictionary attack using John the Ripper / Johnny	✅ Completed
Online password auditing	Hash extraction and dictionary attack using Networkwalks tools	✅ Completed
PDF verification	Used the recovered password to open the test PDF and capture the flag	✅ Completed
Technical documentation	Organized screenshots and documented the practical results	✅ Completed
🛠️ Tools and Technologies
Tool	Purpose
John the Ripper (Jumbo)	Local password auditing and dictionary-based password recovery
Johnny GUI	Graphical frontend used to configure and operate John the Ripper
Networkwalks Hash Calculator	Online extraction of the password hash from the test PDF
Networkwalks Password Cracker	Online dictionary attack against the extracted hash
Encrypted PDF	Authorized test document used during the practical exercise
---
🔎 Part 1 – Local Password Auditing with John the Ripper (JTR)
Objective: Extract the password hash from the encrypted test PDF and evaluate its password strength using John the Ripper.
Activities Performed
Prepared the encrypted test PDF for password-security analysis.
Extracted the PDF password hash in the `$pdf$` format.
Configured and launched Johnny, the graphical frontend for John the Ripper Jumbo, on Windows.
Loaded the extracted hash into the John the Ripper workflow.
Executed a dictionary attack against the hash.
Successfully recovered the password.
Used the recovered password to open the protected PDF.
Key Learning Outcomes
Understood how PDF password hashes can be used in password-auditing workflows.
Gained practical experience with John the Ripper Jumbo and Johnny.
Learned how dictionary attacks test candidate passwords against a hash.
Observed how weak and commonly used passwords can be recovered by automated tools.
📸 JTR – Practical Screenshots (14 Images)
The following screenshots document the local John the Ripper workflow, from the initial setup and hash-handling process through the password-recovery result.

JTR Screenshot 01
![John the Ripper JTR Screenshot 01](https://github.com/user-attachments/assets/110c95d8-db2f-4027-ba3d-8b49025cbe34)
JTR Screenshot 02
![John the Ripper JTR Screenshot 02](https://github.com/user-attachments/assets/b2ba1971-8678-4fbe-b703-b28ee0bd5301)
JTR Screenshot 03
![John the Ripper JTR Screenshot 03](https://github.com/user-attachments/assets/f662cf0e-153c-4591-8c9a-5f3aff82005b)
JTR Screenshot 04
![John the Ripper JTR Screenshot 04](https://github.com/user-attachments/assets/2eddb788-9cce-4606-abee-339acedb2908)
JTR Screenshot 05
![John the Ripper JTR Screenshot 05](https://github.com/user-attachments/assets/8813feb0-09b3-42e6-85c2-de91fd603f95)
JTR Screenshot 06
![John the Ripper JTR Screenshot 06](https://github.com/user-attachments/assets/fa080fb1-92d7-4a45-9a42-c4de6af6be0e)
JTR Screenshot 07
![John the Ripper JTR Screenshot 07](https://github.com/user-attachments/assets/65966297-338a-4556-9a2d-3bd58be1e564)
JTR Screenshot 08
![John the Ripper JTR Screenshot 08](https://github.com/user-attachments/assets/672e6f5e-0ab0-4a51-85c0-5fb6764ad969)
JTR Screenshot 09
![John the Ripper JTR Screenshot 09](https://github.com/user-attachments/assets/8c65c364-2264-4bb7-9cc2-4e2ea107b0a9)
JTR Screenshot 10
![John the Ripper JTR Screenshot 10](https://github.com/user-attachments/assets/340a2fc1-909c-45b1-a0c0-c814b8986ef8)
JTR Screenshot 11
![John the Ripper JTR Screenshot 11](https://github.com/user-attachments/assets/d9925ba8-62c8-4637-84ef-499523185773)
JTR Screenshot 12
![John the Ripper JTR Screenshot 12](https://github.com/user-attachments/assets/143ce2c6-30be-4dd9-abb5-15122ac2316d)
JTR Screenshot 13
![John the Ripper JTR Screenshot 13](https://github.com/user-attachments/assets/ef33dfd6-4a64-485c-bdab-45df6c09eae0)
JTR Screenshot 14
![John the Ripper JTR Screenshot 14](https://github.com/user-attachments/assets/0f353cf5-32de-4bbf-aadb-86fc92e3da74)
---
🌐 Part 2 – Online Password Auditing with Networkwalks Tools
Objective: Repeat the PDF password-recovery exercise using the online tools provided by Networkwalks.
Activities Performed
Opened the Networkwalks Hash Calculator.
Submitted the authorized test PDF to extract its password hash.
Copied the extracted hash.
Opened the Networkwalks Password Cracker.
Submitted the hash and ran the built-in dictionary attack.
Successfully recovered the password.
Used the recovered password to unlock the PDF and capture the flag.
Key Learning Outcomes
Practised extracting a PDF hash through a browser-based tool.
Understood the workflow between hash extraction and password testing.
Compared an online password-auditing process with a local tool.
Recognized that weak passwords may be vulnerable regardless of the interface used to test them.
📸 Networkwalks Tools – Practical Screenshots (7 Images)
The following screenshots document the Networkwalks Hash Calculator and Password Cracker workflow.

Networkwalks Screenshot 01
![Networkwalks Tool Screenshot 01](https://github.com/user-attachments/assets/8979a3ae-d7d1-4c2c-8bc3-557bc7686deb)
Networkwalks Screenshot 02
![Networkwalks Tool Screenshot 02](https://github.com/user-attachments/assets/b06467ae-a392-4502-ade9-b3bd00428195)
Networkwalks Screenshot 03
![Networkwalks Tool Screenshot 03](https://github.com/user-attachments/assets/302c9bbc-8a66-45d5-8306-f12a25aac272)
Networkwalks Screenshot 04
![Networkwalks Tool Screenshot 04](https://github.com/user-attachments/assets/5c6e2a84-5780-4913-9f92-bbffe62cc759)
Networkwalks Screenshot 05
![Networkwalks Tool Screenshot 05](https://github.com/user-attachments/assets/c0148e17-fa4a-4f6b-a056-c896f46b3bad)
Networkwalks Screenshot 06
![Networkwalks Tool Screenshot 06](https://github.com/user-attachments/assets/24c6ccb7-6040-4230-878d-313a08a5383e)
Networkwalks Screenshot 07
![Networkwalks Tool Screenshot 07](https://github.com/user-attachments/assets/3c5d7a39-7add-412f-97cc-0f614e0fd2fc)
---
🏁 Results and Comparison
Both methods successfully recovered the password used to protect the test PDF.
Method	Technique	Result
John the Ripper / Johnny	Local PDF hash auditing with a dictionary attack	✅ Password recovered
Networkwalks tools	Online PDF hash extraction followed by a dictionary attack	✅ Password recovered
Recovered test password: `password1`
The recovered password was used to open the encrypted PDF and capture the flag. This result demonstrates that common and predictable passwords can be vulnerable to dictionary-based guessing.
🔐 Security Analysis and Recommendations
The practical exercise highlighted the importance of choosing strong passwords for encrypted documents. A password such as `password1` is predictable and may be included in commonly used password dictionaries.
Recommendations:
Use long, unique passphrases rather than common words or predictable combinations.
Avoid reusing passwords across accounts and protected documents.
Use a reputable password manager to generate and store strong passwords.
Protect sensitive PDF files with strong, unique passwords and appropriate encryption settings.
Treat extracted password hashes and recovered credentials as sensitive information.
Never publish real passwords, private hashes, or confidential document contents in a public repository.
📄 Full Week 3 Technical Report
The detailed technical report provides additional information about the project, including:
Project introduction, objectives, and authorized scope.
Tools and technologies used.
John the Ripper / Johnny methodology.
Networkwalks Hash Calculator and Password Cracker methodology.
Results and comparison of both methods.
Security analysis and recommendations.
Evidence index linking to all 21 practical screenshots.
📥 View / Download the Complete Week 3 Report (PDF)
📁 Recommended Repository Structure
```text
Networkwalks-Week-3/
│
├── README.md
├── Week3_Report.pdf
│
└── Screenshots/
    ├── John-the-Ripper/
    │   ├── JTR-01.png
    │   ├── JTR-02.png
    │   ├── ...
    │   └── JTR-14.png
    │
    └── Networkwalks-Tools/
        ├── NW-01.png
        ├── NW-02.png
        ├── ...
        └── NW-07.png
```
🛡️ Security, Scope and Ethical Considerations
This project was completed for educational cybersecurity training using the authorized test PDF supplied for the exercise.
Password auditing should only be performed on documents that you own or have explicit permission to assess.
Extracted hashes and recovered passwords should be handled as sensitive information.
Do not use these techniques to access another person's protected documents without authorization.
The screenshots and report are included to document the learning process, not to encourage unauthorized access.
💡 Skills Developed
Through this project, I strengthened my practical understanding of:
PDF password security.
Password hash extraction.
John the Ripper Jumbo.
Johnny graphical interface.
Dictionary-based password attacks.
Browser-based password-auditing tools.
Password-strength assessment.
Comparing local and online security tools.
Technical documentation and evidence organization.
Ethical and authorized security testing.
🚀 Conclusion
Completing Week 3 of the Networkwalks Cybersecurity Internship provided valuable hands-on experience in PDF password security and password auditing.
By performing the exercise with both John the Ripper / Johnny and the Networkwalks online tools, I gained practical insight into how password hashes can be tested through dictionary attacks. Both approaches recovered the test password, demonstrating why strong, unique passwords are essential when protecting sensitive documents.
This project represents another step in my continuous journey toward developing practical cybersecurity skills and building a professional cybersecurity portfolio.
---
<p align="center">
  <b>🔐 Learn • Practise • Analyze • Secure</b>
  <br/>
  <i>Building practical cybersecurity knowledge, one project at a time.</i>
</p>
