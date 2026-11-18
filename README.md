# 🔐 Networkwalks Week 3 – PDF Password Cracking

<p align="center">
  <img src="https://img.shields.io/badge/Networkwalks-Cybersecurity%20Internship-blue?style=for-the-badge" alt="Networkwalks Internship"/>
  <img src="https://img.shields.io/badge/Batch-B082-success?style=for-the-badge" alt="Batch B082"/>
  <img src="https://img.shields.io/badge/Week-03-orange?style=for-the-badge" alt="Week 3"/>
  <img src="https://img.shields.io/badge/Focus-PDF%20Password%20Security-purple?style=for-the-badge" alt="PDF Password Security"/>
</p>

---

## 📌 Project Overview

This repository documents my Week 3 practical project for the Networkwalks Cybersecurity Internship. The objective was to assess the password strength of an authorized, password-protected PDF by extracting its hash and testing whether a dictionary attack could recover the password.

To provide a comprehensive comparison, I completed the practical using two distinct methodologies: a local desktop tool (**John the Ripper**) and a browser-based tool (**Networkwalks Web Tools**).

---

## 🛠️ Tools and Technologies Used

| Tool | Environment | Purpose |
| :--- | :--- | :--- |
| **John the Ripper (Jumbo) / Johnny GUI** | Local (Windows) | Local password auditing and dictionary-based recovery. |
| **Networkwalks Hash Calculator** | Web-based | Online extraction of the `$pdf$` password hash. |
| **Networkwalks Password Cracker** | Web-based | Online dictionary attack against the extracted hash. |

---

## 🧪 Lab 1: Local Password Auditing (John the Ripper)

**Objective:** Extract the hash from the encrypted PDF and crack it using local tools.

**Methodology:**
1. Extracted the PDF password hash in the standard `$pdf$` format.
2. Configured and launched **Johnny** (the GUI for John the Ripper Jumbo) on Windows.
3. Loaded the hash into the Johnny workflow and executed a dictionary attack.
4. Successfully recovered the password: `password1`.
5. Used the recovered password to unlock the test PDF and capture the flag.

### 📸 Evidence (14 Screenshots)
The following gallery documents the local John the Ripper / Johnny workflow.

<details>
<summary>👉 Click to expand and view all 14 John the Ripper screenshots</summary>
<br>

**JTR Screenshot 01 – Initial setup**
![JTR Screenshot 01 – Initial setup](https://github.com/user-attachments/assets/110c95d8-db2f-4027-ba3d-8b49025cbe34)

**JTR Screenshot 02 – PDF hash extraction**
![JTR Screenshot 02 – PDF hash extraction](https://github.com/user-attachments/assets/b2ba1971-8678-4fbe-b703-b28ee0bd5301)

**JTR Screenshot 03 – Hash format**
![JTR Screenshot 03 – Hash format](https://github.com/user-attachments/assets/f662cf0e-153c-4591-8c9a-5f3aff82005b)

**JTR Screenshot 04 – Johnny configuration**
![JTR Screenshot 04 – Johnny configuration](https://github.com/user-attachments/assets/2eddb788-9cce-4606-abee-339acedb2908)

**JTR Screenshot 05 – Loading the hash**
![JTR Screenshot 05 – Loading the hash](https://github.com/user-attachments/assets/8813feb0-09b3-42e6-85c2-de91fd603f95)

**JTR Screenshot 06 – Dictionary attack setup**
![JTR Screenshot 06 – Dictionary attack setup](https://github.com/user-attachments/assets/fa080fb1-92d7-4a45-9a42-c4de6af6be0e)

**JTR Screenshot 07 – Attack execution**
![JTR Screenshot 07 – Attack execution](https://github.com/user-attachments/assets/65966297-338a-4556-9a2d-3bd58be1e564)

**JTR Screenshot 08 – Password auditing progress**
![JTR Screenshot 08 – Password auditing progress](https://github.com/user-attachments/assets/672e6f5e-0ab0-4a51-85c0-5fb6764ad969)

**JTR Screenshot 09 – Recovery result**
![JTR Screenshot 09 – Recovery result](https://github.com/user-attachments/assets/8c65c364-2264-4bb7-9cc2-4e2ea107b0a9)

**JTR Screenshot 10 – Recovered password**
![JTR Screenshot 10 – Recovered password](https://github.com/user-attachments/assets/340a2fc1-909c-45b1-a0c0-c814b8986ef8)

**JTR Screenshot 11 – PDF verification**
![JTR Screenshot 11 – PDF verification](https://github.com/user-attachments/assets/d9925ba8-62c8-4637-84ef-499523185773)

**JTR Screenshot 12 – Opening the test PDF**
![JTR Screenshot 12 – Opening the test PDF](https://github.com/user-attachments/assets/143ce2c6-30be-4dd9-abb5-15122ac2316d)

**JTR Screenshot 13 – Practical evidence**
![JTR Screenshot 13 – Practical evidence](https://github.com/user-attachments/assets/ef33dfd6-4a64-485c-bdab-45df6c09eae0)

**JTR Screenshot 14 – Final lab evidence**
![JTR Screenshot 14 – Final lab evidence](https://github.com/user-attachments/assets/0f353cf5-32de-4bbf-aadb-86fc92e3da74)

</details>

---

## 🌐 Lab 2: Online Password Auditing (Networkwalks Tools)

**Objective:** Repeat the password-recovery exercise using browser-based tools.

**Methodology:**
1. Opened the **Networkwalks Hash Calculator** and uploaded the authorized test PDF.
2. The tool extracted the crackable hash directly from the document.
3. Pasted the hash into the **Networkwalks Password Cracker**.
4. Initiated the built-in dictionary attack, which successfully recovered the password: `password1`.
5. Unlocked the PDF and captured the flag.

### 📸 Evidence (7 Screenshots)
The following gallery documents the Networkwalks online-tool workflow.

<details>
<summary>👉 Click to expand and view all 7 Networkwalks screenshots</summary>
<br>

**Networkwalks Screenshot 01 – Hash Calculator**
![Networkwalks Screenshot 01 – Hash Calculator](https://github.com/user-attachments/assets/8979a3ae-d7d1-4c2c-8bc3-557bc7686deb)

**Networkwalks Screenshot 02 – PDF hash extraction**
![Networkwalks Screenshot 02 – PDF hash extraction](https://github.com/user-attachments/assets/b06467ae-a392-4502-ade9-b3bd00428195)

**Networkwalks Screenshot 03 – Extracted hash**
![Networkwalks Screenshot 03 – Extracted hash](https://github.com/user-attachments/assets/302c9bbc-8a66-45d5-8306-f12a25aac272)

**Networkwalks Screenshot 04 – Password Cracker**
![Networkwalks Screenshot 04 – Password Cracker](https://github.com/user-attachments/assets/5c6e2a84-5780-4913-9f92-bbffe62cc759)

**Networkwalks Screenshot 05 – Dictionary attack**
![Networkwalks Screenshot 05 – Dictionary attack](https://github.com/user-attachments/assets/c0148e17-fa4a-4f6b-a056-c896f46b3bad)

**Networkwalks Screenshot 06 – Password recovery**
![Networkwalks Screenshot 06 – Password recovery](https://github.com/user-attachments/assets/24c6ccb7-6040-4230-878d-313a08a5383e)

**Networkwalks Screenshot 07 – PDF and flag verification**
![Networkwalks Screenshot 07 – PDF and flag verification](https://github.com/user-attachments/assets/3c5d7a39-7add-412f-97cc-0f614e0fd2fc)

</details>

---

## 🏁 Results and Security Analysis

Both methods successfully recovered the test password: **`password1`**. 

This result demonstrates that common, predictable passwords can be vulnerable to dictionary-based guessing, whether the audit is performed with a local tool or a browser-based tool.

**Key Takeaways & Recommendations:**
*   **Use Passphrases:** Avoid common dictionary words with predictable number additions. Use long, unique passphrases instead.
*   **Password Managers:** Use a reputable password manager to generate and store strong, unique passwords for encrypted documents.
*   **Handle with Care:** Treat extracted hashes and recovered credentials as sensitive information.

---

## 📄 Full Week 3 Technical Report

For a more detailed explanation of the practical exercise, tools, methodology, results, and security recommendations, view the accompanying report:

📥 **[View / Open the Complete Week 3 Report (PDF)](./Week3_Report.pdf)**

> **Note:** Ensure `Week3_Report.pdf` is uploaded to the repository's main folder, alongside this `README.md`, so the link above opens correctly.

---

## 📁 Repository Structure

```text
Networkwalks-Week3-PasswordCracking/
│
├── README.md
├── Week3_Report.pdf
│
└── Screenshots/
    ├── John-the-Ripper/
    │   ├── JTR-01.png to JTR-14.png
    │
    └── Networkwalks-Tools/
        ├── NW-01.png to NW-07.png
```

---

## 🛡️ Security, Scope and Ethical Considerations

This project was completed for educational cybersecurity training using the authorized test PDF supplied for the exercise.

Password auditing should only be performed on documents that you own or have explicit permission to assess. Extracted hashes and recovered passwords should be handled as sensitive information. Do not use these techniques to access another person's protected documents without authorization.

The screenshots and report are included to document the learning process, not to encourage unauthorized access.

---

## 💡 Skills Developed

Through this project, I strengthened my practical understanding of:
*   PDF password security & Password hash extraction
*   John the Ripper Jumbo & Johnny graphical interface
*   Dictionary-based password attacks
*   Browser-based password-auditing tools
*   Password-strength assessment
*   Comparing local and online security tools
*   Technical documentation and evidence organization
*   Ethical and authorized security testing

---

## 🚀 Conclusion

Completing Week 3 of the Networkwalks Cybersecurity Internship provided valuable hands-on experience in PDF password security and password auditing.

By performing the exercise with both John the Ripper / Johnny and the Networkwalks online tools, I gained practical insight into how password hashes can be tested through dictionary attacks. Both approaches recovered the test password, demonstrating why strong, unique passwords are essential when protecting sensitive documents.

This project represents another step in my continuous journey toward developing practical cybersecurity skills and building a professional cybersecurity portfolio.
