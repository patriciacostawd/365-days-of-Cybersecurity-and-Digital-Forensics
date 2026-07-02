🔍 Digital Forensics & Incident Response (DFIR) Learning Journal

🎯 Objective

This repository documents my structured journey into Digital Forensics & Incident Response (DFIR), focusing on practical investigation skills, evidence handling, and technical analysis of cyber incidents.

The goal is to develop the ability to reconstruct digital incidents using real evidence, logs, disk artifacts, and network data — and to build a portfolio that demonstrates this competence to future employers.

🧭 Background

I come from a multidisciplinary background in forensic sciences and software development, and I am transitioning into cybersecurity with a strong focus on DFIR and cybercrime investigation.

Transferable skills:


Forensic sciences → chain of custody principles, evidentiary rigor, methodical documentation, courtroom-oriented reporting mindset
Software development → scripting/automation, comfort with tooling and version control, structured problem-solving, ability to read and reason about code (relevant for malware/log analysis)


🧭 Target Certifications (Roadmap)


Short-term: eJPT (foundations in networking/pentesting context)
Mid-term: GCFA or CHFI (core DFIR credentials)
Long-term (optional): GNFA / GREM (network forensics / malware reverse engineering)


🧱 Learning Structure (~120–150 Days)

Timelines below are target ranges, not deadlines. Each phase closes only when its artifact is complete — I'd rather iterate on a phase than move on with shallow coverage.

🟢 Phase 1 — Foundations (Days 1–35)

Focus:


Linux fundamentals (filesystem, permissions, processes, shell)
Networking basics (TCP/IP, DNS, HTTP/S, packet structure)
Python scripting for data analysis


Skills:


File system navigation & basic Linux forensics commands
Log parsing basics
Regex fundamentals


Artifact: Python log-parsing script (published, with its own README) that ingests raw logs and flags anomalies/IOCs — see Project 1.

✅ Success Criteria

Linux — I can, without consulting notes:


 Locate files modified in the last 24h on a system (find, stat)
 List running processes and spot a suspicious one by anomalous CPU/network activity (ps, top, lsof, ss)
 Read file permissions and identify anomalies (e.g. unexpected SUID binary)
 Filter relevant lines from a 10,000+ line log using grep/awk/sed combined
 Explain what /var/log/auth.log vs /var/log/syslog each record


Networking — I can, without consulting notes:


 Explain the TCP handshake (SYN/SYN-ACK/ACK) and recognize it in a Wireshark capture
 Distinguish normal DNS traffic from DNS-tunneling patterns
 Read an HTTP/HTTPS request in a PCAP and extract source/dest IP, ports, payload (if unencrypted)
 Explain why HTTPS hides payload but not metadata (IP, timing, size)
 Identify a port scan in a firewall log (many ports, one IP, short time window)


Python — I can, without consulting notes:


 Write a script that reads a log file line by line and extracts IPs via regex
 Use a dict/Counter to tally event frequency (e.g. failed logins per IP)
 Export structured results to CSV/JSON
 Handle large files without loading everything into memory (streaming/generators)
 Write a script that accepts CLI arguments (argparse)


🧪 Validation Exercises

ExerciseValidatesPass conditionOverTheWire "Bandit" (levels 0–15)Linux fundamentalsCompleted without googling a command every 2 minutes2–3 PCAPs from malware-traffic-analysis.net training exercisesNetworkingIdentify malicious traffic before reading the published write-upScript analyzing a simulated SSH auth logPythonCorrectly outputs: top 5 IPs by failed logins, peak activity windows, brute-force candidates (>N fails/IP in <X min)Redo the PCAP + script exercises from scratch, no reference to prior attemptRetentionFaster and more accurate than the first attempt

🗓️ Suggested Weekly Breakdown

WeekFocusDone when1–2Linux + BanditBandit 0–15 completed unaided3Networking theory + Wireshark basicsCan annotate a simple PCAP field by field4Python scriptingLog analysis script (Project 1) runs cleanly on a real log5ConsolidationRedo PCAP + script exercises from scratch — faster/cleaner than before

🟡 Phase 2 — Core DFIR, Iteration 1 (Days 36–70)

Focus:


Disk forensics (Autopsy) on a public sample image
Memory forensics fundamentals (Volatility) — moved up from "future"
Log correlation basics


Skills:


Timeline reconstruction (disk-level)
Artifact analysis (registry, browser history, deleted files)
Basic memory triage (process list, network connections in memory dump)


Artifact: Written case walk-up using a public CFReDS or Digital Corpora image — see Project 2.

🟡 Phase 2 — Core DFIR, Iteration 2 (Days 71–100)

Focus:


Network forensics (Wireshark) on public PCAP samples
Correlating disk + memory + network artifacts for a single scenario


Skills:


PCAP triage and suspicious-flow identification
Cross-source timeline correlation
IOC extraction and structuring (CSV/STIX-like format)


Artifact: PCAP analysis write-up — see Project 3.

🔴 Phase 3 — Incident Simulation (Days 101–130+)

Focus:


End-to-end incident investigation combining disk, memory, network, and log evidence
Professional forensic report writing
Evidence correlation across sources into a single coherent timeline


Skills:


Full case analysis
IOC extraction and threat-actor behavior mapping
Professional forensic reporting (executive summary + technical appendix)


Artifact: Full DFIR case study with anonymized PDF report — see Project 4.

🧪 Projects

🔍 Project 1 — Log Analysis (Python)

Description: Analysis of system logs to detect anomalies and extract indicators of compromise (IOCs).

Tools: Python, Regex, CSV/JSON parsing

Dataset: Synthetic/sample logs (source TBD — e.g. sample Apache/auth logs)

Deliverable: Script + README explaining detection logic and sample findings

Status: In progress

💾 Project 2 — Disk Forensics Case (Autopsy)

Description: Forensic analysis of a disk image including file recovery, timeline analysis, and artifact extraction.

Tools: Autopsy, Timeline analysis

Dataset: Public sample image (CFReDS or Digital Corpora — to be selected)

Deliverable: Written case walk-through (methodology, findings, screenshots, conclusions)

Status: Planned

🌐 Project 3 — Network Traffic Analysis

Description: Analysis of PCAP files to identify suspicious network activity and reconstruct events.

Tools: Wireshark

Dataset: Public PCAP sample (e.g. malware-traffic-analysis.net)

Deliverable: Traffic analysis report with identified IOCs and reconstructed event sequence

Status: Planned

🧠 Project 4 — Full DFIR Case Study

Description: End-to-end investigation combining disk, network, and log evidence.

Tools: Autopsy, Wireshark, Volatility, Python

Dataset: Combination of public samples assembled into a single scenario

Outcome:


Full forensic report (executive summary + technical detail)
IOC extraction
Incident timeline


Status: Planned

📂 Datasets & Sources

Public, legally usable datasets used throughout this journal:


CFReDS (NIST) — https://cfreds.nist.gov/ — standard disk/memory images for training
Digital Corpora — https://digitalcorpora.org/ — disk images, memory dumps, scenario data
Malware-Traffic-Analysis.net — PCAP samples with known malicious traffic
DFIR.training — curated list of practice datasets and CTF-style exercises
Volatility Foundation sample memory images — for memory forensics practice


(List will be updated with exact dataset names/versions as each project starts.)

🛠️ Tools & Technologies


Linux (Ubuntu / Kali basics)
Python
Wireshark
Autopsy
Volatility
Sysinternals
Regex
JSON / CSV analysis


📊 Progress Tracking

AreaStatusLinux🟡 In progressNetworking🟡 In progressPython🟡 In progressDisk Forensics⏳ Not startedMemory Forensics⏳ Not startedNetwork Forensics⏳ Not startedIncident Response⏳ Not started

📝 Progress Log

Dated entries documenting concrete work done — not just topics studied. Each entry should answer: what did I do, what did I learn/get stuck on, what's next.


Format suggestion per entry:
[YYYY-MM-DD] — Title


Did: what was actually done (exercise, script, case)
Result: outcome / what worked
Stuck on / learned: honest note on gaps or insights
Next: immediate next step


<!-- Example entry — replace with real ones as you go
**[2026-07-02] — Bandit levels 0–5**
- **Did:** Completed OverTheWire Bandit levels 0–5.
- **Result:** All passed unaided except level 4 (needed a hint on `file` command usage).
- **Stuck on / learned:** Forgot `find -perm` syntax, had to look it up — added to personal cheat sheet.
- **Next:** Levels 6–10.
-->
📌 Philosophy

"Digital forensics is not about tools. It is about reconstructing truth from fragmented digital evidence."

⚠️ Disclaimer

All investigations in this repository are performed on simulated, synthetic, or intentionally publicly-provided datasets, for educational purposes only. No real, private, or unauthorized data is used at any stage.
