365 Days of Cybersecurity & Digital Forensics

Patrícia Costa | MSc Forensic Sciences (FMUP) | GitHub

🎯 Objective

Document my daily learning journey in cybersecurity and digital forensics, to work as a Digital Forensics Analyst in a cybercrime context.

I combine a solid background in Forensic Sciences (ongoing MSc at FMUP) with technical skills in information security, networking, Linux, and digital investigation, creating a specialised profile for digital forensic analysis.

📊 Current Progress

AreaStatusDays (goal)Main FocusProgressCybersecurity Fundamentals🟢 In progress16 / 180Cisco Junior Analyst + ISC2 CC2%Digital Forensics🟡 Planned0 / 180DFIR + OSINT + Autopsy0%

Commitment: 1h30/day, 6 days/week

🔒 Track 1 – Cybersecurity Foundations

Status: In progress (Day 18/180)

Objective: Master end-to-end software development to understand application architecture, database structures, and web vulnerabilities from the inside out.

Main Training & Certifications

🎓 freeCodeCamp — 🟢 In Progress (Scientific Computing with Python / Security Scripting)
🎓 Cisco Junior Cybersecurity Analyst — 🟢 In Progress (Section 1.2.4)
🎓 ISC2 Certified in Cybersecurity (CC) — ⏳ Planned


Core Technical Skills


🐍 Python Automation: Log parsing, file hashing, and data extraction
🐧 Linux Essentials & Networking: Command line fluency and TCP/IP analysis


✅ Success Criteria — mapped to active courses

The point of each course below is to build a specific, checkable skill — not just "cover" a topic. Checked once I can do it without consulting notes.

From Cisco Junior Cybersecurity Analyst (networking + SOC fundamentals):


 Explain the TCP handshake (SYN/SYN-ACK/ACK) and recognize it in a packet capture
 Identify the OSI/TCP-IP layer a given protocol operates at (DNS, HTTP, ARP, ICMP)
 Read a firewall/IDS log entry and identify source, destination, and rule triggered
 Explain the difference between IDS and IPS, and where each sits in a network


From ISC2 CC (5 domains — security principles, IR/BC/DR, access control, network security, security operations):


 State the CIA triad and give a concrete example of a control for each
 Explain the difference between incident response, business continuity, and disaster recovery
 Describe the basic incident response lifecycle (prepare → identify → contain → eradicate → recover → lessons learned) — this is the direct bridge to Track 2 forensic methodology
 Explain least privilege and give an example of it misconfigured


From freeCodeCamp (Python / Security Scripting):


 Write a script that reads a log file line by line and extracts IPs via regex
 Use a dict/Counter to tally event frequency (e.g. failed logins per IP)
 Export structured results to CSV/JSON
 Hash a file (MD5/SHA-256) and verify integrity programmatically — direct forensic use (evidence integrity)


From Linux Essentials & Networking (self-directed):


 Locate files modified in the last 24h on a system (find, stat)
 List running processes and spot a suspicious one by anomalous CPU/network activity (ps, top, lsof, ss)
 Filter relevant lines from a large log using grep/awk/sed combined


🔍 Track 2 – Digital Forensics & Digital Evidence Analysis ⭐ SPECIALIZATION

Status: In progress (Day 2/180)

Objective: Master digital forensic methodologies, chain of custody preservation, and data recovery techniques using professional DFIR tooling.

Active Study Areas


🎓 Udemy: Digital Forensics Investigation Process – The Big Picture — 🟢 In Progress (Methodology & Legal Concepts)
⚖️ Digital Evidence Fundamentals: Chain of custody and forensic reporting (FMUP alignment)
💻 File System Analysis: Artifact parsing, data carving, and timeline reconstruction using Autopsy


✅ Success Criteria — mapped to active study areas

From Udemy DFIR course (methodology & legal concepts):


 Explain chain of custody end-to-end and identify a break in it given a scenario
 List the phases of a digital forensic investigation (acquisition → preservation → analysis → reporting) and what can invalidate evidence at each phase
 Explain the difference between a forensic image and a simple file copy, and why it matters legally


From Autopsy / File System Analysis:


 Build a timeline of file creation/modification/access from a disk image
 Recover a deleted file from unallocated space in a sample image
 Extract and interpret browser history / registry artifacts relevant to a scenario


📂 Featured Projects & Labs

Project / LabDescriptionTechnologies / ToolsStatusCyberSecurity Events HubHTML page with cybersecurity eventsHTML5 / CSS3✅ CompletedPython Log AnalyzerScript developed via freeCodeCamp logic to parse security logsPython⏳ PlannedAutopsy Disk Analysis LabForensic analysis of a disk image, data carving, and timeline reportAutopsy⏳ PlannedWireshark LabNetwork traffic capture and malicious packet analysisWireshark⏳ Planned

📂 Datasets & Sources (for upcoming labs)


CFReDS (NIST) — https://cfreds.nist.gov/ — disk/memory images for the Autopsy lab
Digital Corpora — https://digitalcorpora.org/ — disk images, memory dumps, scenario data
Malware-Traffic-Analysis.net — PCAP samples with known malicious traffic, for the Wireshark lab
DFIR.training — curated practice datasets and CTF-style exercises


(To be finalized as each lab starts — exact dataset/version noted in the corresponding Progress Log entry.)

📝 Progress Log

Dated entries documenting concrete work done — not just topics covered. Keeps the % progress above honest.


Format:
[YYYY-MM-DD] — Title


Did: what was actually done (course section, exercise, script, case)
Result: outcome / what worked
Stuck on / learned: honest note on gaps or insights
Next: immediate next step




<!-- Example — replace with real entries as you go
**[2026-07-02] — Cisco Junior Analyst, Section 1.2.4**
- **Did:** Completed section on TCP/IP layer functions.
- **Result:** Passed the section quiz, no major issues.
- **Stuck on / learned:** Kept confusing session vs transport layer responsibilities — made a diagram to fix it.
- **Next:** Section 1.3, ISC2 CC Domain 1 in parallel.
-->
📅 Monthly Recap


Planned vs actual: what the 180-day tracks projected vs what really happened
Adjustment: any change to pace or course order
Confidence check: which success criteria (above) are genuinely met, not just "covered"


🧭 Target Certifications (beyond current courses)


Mid-term: GCFA or CHFI (core DFIR credentials, once Track 2 fundamentals are solid)
Long-term (optional): GNFA / GREM (network forensics / malware reverse engineering)



"Digital forensic investigation requires dual competence: rigorous forensic knowledge (MSc) + solid technical skills (cybersecurity & automation). This repository documents the building of that technical foundation."

⚠️ Disclaimer

All investigations and labs in this repository are performed on simulated, synthetic, or intentionally publicly-provided datasets, for educational purposes only. No real, private, or unauthorized data is used at any stage.
