# 🔐 Networkwalks Week 3 – PDF Password Security & Cryptography

<p align="center">
  <img src="https://img.shields.io/badge/Networkwalks-Cybersecurity%20Internship-blue?style=for-the-badge" alt="Networkwalks Internship"/>
  <img src="https://img.shields.io/badge/Batch-B082-success?style=for-the-badge" alt="Batch B082"/>
  <img src="https://img.shields.io/badge/Week-03-orange?style=for-the-badge" alt="Week 3"/>
  <img src="https://img.shields.io/badge/Focus-PDF%20Password%20Security-purple?style=for-the-badge" alt="PDF Password Security"/>
</p>

## 📌 Project Overview
This repository documents my Week 3 practical project for the Networkwalks Cybersecurity Internship. The objective was to assess the password strength of an authorized, password-protected PDF by extracting its hash and testing whether a dictionary attack could recover the password. 

To provide a comprehensive comparison, I completed the practical using **two distinct methodologies**: a local desktop tool (John the Ripper) and a browser-based tool (Networkwalks Web Tools).

---

## 🛠️ Tools and Technologies Used

| Tool | Environment | Purpose |
|------|-------------|---------|
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

**📸 Evidence (14 Screenshots):** 
*(View the full step-by-step in the `Screenshots/John-the-Ripper/` folder)*

<details>
<summary>👉 Click to view the JTR Screenshots</summary>

*(Paste your 14 image links here exactly as you had them in your original text)*
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

**📸 Evidence (7 Screenshots):**
*(View the full step-by-step in the `Screenshots/Networkwalks-Tools/` folder)*

<details>
<summary>👉 Click to view the Networkwalks Screenshots</summary>

*(Paste your 7 image links here exactly as you had them in your original text)*
</details>

---

## 🏁 Results and Security Analysis

Both methods successfully recovered the test password: **`password1`**.

This result perfectly demonstrates that common, predictable passwords are highly vulnerable to dictionary-based guessing, regardless of whether the attacker is using a heavy local tool or a quick web script.

**Key Takeaways & Recommendations:**
*   **Use Passphrases:** Avoid dictionary words with numbers attached (e.g., `password1`). Use long, unique passphrases instead.
*   **Password Managers:** Use a tool to generate and store complex passwords for encrypted documents.
*   **Handle with Care:** Treat extracted hashes and recovered credentials as highly sensitive information.

---

## 📁 Repository Structure

```text
Networkwalks-Week-3/
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
