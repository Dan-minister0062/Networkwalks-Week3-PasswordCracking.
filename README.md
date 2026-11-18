🔐 Networkwalks Cybersecurity Internship --- Week 3
PDF Password Security Assessment | John the Ripper & Networkwalks Tools
```{=html}
<p align="center">
```
`<img src="https://img.shields.io/badge/Program-Networkwalks%20Cybersecurity%20Internship-0A66C2?style=for-the-badge" alt="Networkwalks Internship">`{=html}
`<img src="https://img.shields.io/badge/Batch-B082-6A5ACD?style=for-the-badge" alt="Batch B082">`{=html}
`<img src="https://img.shields.io/badge/Week-03-2E8B57?style=for-the-badge" alt="Week 3">`{=html}
`<img src="https://img.shields.io/badge/Focus-Cryptography%20%26%20Password%20Security-8A2BE2?style=for-the-badge" alt="Cryptography and Password Security">`{=html}
```{=html}
</p>
```
📌 Project Overview
This project documents a controlled PDF password-security exercise
completed during Week 3 of the Networkwalks Cybersecurity Internship
(Batch B082). The objective was to assess the resistance of a
password-protected PDF to dictionary-based password recovery.
The practical exercise was completed using two independent
approaches:
John the Ripper (JTR) with Johnny GUI --- a local
password-auditing workflow.
Networkwalks online tools --- the Hash Calculator and Password
Cracker.
Both methods recovered the test PDF password, `password1`, and enabled
the protected PDF to be opened and the lab flag to be captured.
> **Lab scope:** This documentation describes an authorized educational
> exercise using a test PDF. It does not describe or authorize attempts
> to access documents or accounts belonging to other people.
🎯 Objectives
Understand how password-protected PDF files can be assessed through
password-hash extraction.
Extract a PDF password hash for offline auditing.
Configure and use John the Ripper through the Johnny graphical
interface.
Perform a dictionary-based password-recovery attempt with a local
tool.
Use the Networkwalks Hash Calculator and Password Cracker as a
separate web-based workflow.
Compare the outcomes of local and web-based password-auditing
methods.
Document the process with separate evidence sets for each method.
Identify practical lessons for creating stronger passwords.
🧰 Tools and Technologies
---
Tool                                Purpose
---
John the Ripper Jumbo               Local password-hash auditing and
dictionary attack
Johnny GUI                          Graphical frontend for John the
Ripper
Networkwalks Hash Calculator        Web-based extraction/calculation of
the PDF hash
Networkwalks Password Cracker       Web-based dictionary
password-recovery exercise
Password-protected PDF              Authorized lab file used for the
exercise
🧪 Method 1 --- Local Password Auditing with John the Ripper
Evidence set: 14 screenshots (`JTR-01` to `JTR-14`).
The first workflow used John the Ripper locally, with Johnny as its
graphical frontend.
Workflow
Prepared the password-protected PDF supplied for the lab.
Extracted the PDF password hash into a format suitable for password
auditing.
Opened/configured Johnny, the graphical frontend for John the Ripper
Jumbo.
Loaded the extracted hash into the local auditing workflow.
Ran a dictionary-based password-recovery attempt.
Observed the recovered password result.
Used the recovered password to open the test PDF and continue the
lab exercise.
Result: The local John the Ripper workflow recovered the test
password `password1`.
John the Ripper evidence
---
Evidence ID             Original screenshot     Evidence
label
---
JTR-01                  W3P1                    Open
screenshot
JTR-02                  W3P2                    Open
screenshot
JTR-03                  W3P3                    Open
screenshot
JTR-04                  W3P4                    Open
screenshot
JTR-05                  W3P5                    Open
screenshot
JTR-06                  W3P6                    Open
screenshot
JTR-07                  W3P7                    Open
screenshot
JTR-08                  W3P8                    Open
screenshot
JTR-09                  W3P9                    Open
screenshot
JTR-10                  W3P10                   Open
screenshot
JTR-11                  W3P11                   Open
screenshot
JTR-12                  W3P12                   Open
screenshot
JTR-13                  W3P13                   Open
screenshot
JTR-14                  W3P14                   Open
screenshot
🌐 Method 2 --- Web-Based Password Auditing with Networkwalks Tools
Evidence set: 7 screenshots (`NW-01` to `NW-07`).
The second workflow used the Networkwalks web tools, independently of
the local John the Ripper workflow.
Workflow
Opened the Networkwalks Hash Calculator.
Used the tool to extract/calculate the hash from the
password-protected PDF.
Copied the resulting hash into the Networkwalks Password Cracker.
Ran the available dictionary-based password-recovery process.
Reviewed the recovered password result.
Used the recovered password to open the test PDF and capture the lab
flag.
Result: The Networkwalks workflow also recovered the test password
`password1`.
Networkwalks evidence
---
Evidence ID             Original screenshot     Evidence
label
---
NW-01                   W3P1                    Open
screenshot
NW-02                   W3P2                    Open
screenshot
NW-03                   W3P3                    Open
screenshot
NW-04                   W3P4                    Open
screenshot
NW-05                   W3P5                    Open
screenshot
NW-06                   W3P6                    Open
screenshot
NW-07                   W3P7                    Open
screenshot
📊 Results and Comparison
---
Assessment item         John the Ripper /       Networkwalks tools
Johnny
---
Approach                Local password auditing Web-based
password-auditing
workflow
Hash handling           Extracted PDF hash and  Used the Networkwalks
loaded it into the      Hash Calculator
local tool
Recovery method         Dictionary attack       Built-in dictionary
attack
Outcome                 Password recovered      Password recovered
Recovered lab password  `password1`             `password1`
PDF access              Test PDF opened         Test PDF opened; lab
flag captured
Both approaches reached the same result. This demonstrates that a
commonly used password can be vulnerable to dictionary-based guessing.
The result is specific to the test PDF and the wordlist/attack
conditions used in this lab; it should not be interpreted as a benchmark
of either tool's overall speed or effectiveness.
🔎 Key Learning Outcomes
A password-protected PDF stores password-verification data that can
be assessed through an extracted hash.
Password-hash extraction is distinct from decrypting the PDF itself.
Dictionary attacks test candidate passwords from a wordlist against
the extracted hash.
A weak or commonly used password may be recovered quickly if it
appears in the tested wordlist.
Local tools provide control over the auditing environment and
workflow.
Web-based tools can provide a convenient alternative, but users
should consider the privacy implications of uploading files or
hashes to third-party services.
Strong, unique passwords and password managers help reduce the risk
of dictionary-based password recovery.
🛡️ Security Recommendations
Use long, unique passwords or passphrases rather than predictable
words and number combinations.
Avoid common passwords, personal details, dictionary words, and
predictable patterns.
Use a reputable password manager to generate and store unique
credentials.
Protect sensitive PDFs with strong encryption and a robust password.
Avoid uploading confidential documents or password hashes to online
tools unless the service is trusted and its data-handling policy has
been reviewed.
Apply access controls and share protected documents only with
intended recipients.
For organizations, establish password policies and provide user
awareness training.
📁 Suggested Repository Structure
``` text
Networkwalks-Week-3/
├── README.md
├── Week3_Report.pdf
└── Screenshots/
    ├── John_the_Ripper/
    │   ├── JTR-01.png
    │   ├── JTR-02.png
    │   └── ... JTR-14.png
    └── Networkwalks_Tools/
        ├── NW-01.png
        ├── NW-02.png
        └── ... NW-07.png
```
The screenshot links above point to the GitHub-hosted images supplied
with this project. If you download the images into the repository, you
can replace each external screenshot URL with a relative path such as
`Screenshots/John_the_Ripper/JTR-01.png`.
📄 Full Technical Report
Open or download the Week 3 PDF Report
The report provides the structured methodology, results, comparison,
security observations, and separate evidence references for both tools.
⚖️ Ethical and Authorized Use
This work was conducted as an educational lab exercise on a test PDF
within the internship activity. Password auditing should only be
performed on files for which you have explicit authorization. Do not use
these techniques to attempt unauthorized access to private documents or
data.
👨‍💻 Author
Ibrahim Idris Ibrahim  
Networkwalks Cybersecurity Internship --- Batch B082  
Week 3: Cryptography and Password Security
---
```{=html}
<p align="center">
```
`<b>`{=html}Learn • Practice • Document •
Improve`</b>`{=html}`<br>`{=html} `<i>`{=html}Building practical
cybersecurity skills through responsible hands-on learning.`</i>`{=html}
```{=html}
</p>
```
