# Cybersecurity Portfolio — Robert Louis Bostick

CTU Online — B.S. Computer Science, cybersecurity focus (junior, in progress)
GitHub: [@Rionangelfire](https://github.com/Rionangelfire)

I built a lightweight SOC simulation platform that streams MITRE-mapped security telemetry from a Python backend into a browser-based analyst console.

## Aegis Shield — SOC Simulation Platform
[github.com/Rionangelfire/aegis-shield](https://github.com/Rionangelfire/aegis-shield)

- **Telemetry engine** (Python): emits MITRE ATT&CK-tagged events over Server-Sent Events (`localhost:8080/stream`) — 8 threat profiles (baseline, storm, brute force, PowerShell, credential dumping, C2, lateral movement, ransomware), with tactic, technique, asset group, confidence, and event IDs.
- **SOC console** (HTML/JavaScript): consumes the stream live and renders event cards with severity styling and running counters.
- **Packet Analyzer v1.5** (Python + HTML GUI): stateful packet inspection against 5 signature rules — brute-force login attempts (T1110.001), WinRM/PowerShell remote execution (T1059.001), SMB/RDP lateral movement (T1021.002), ransomware entropy spikes (T1486), DNS tunneling (T1071.004) — with response hints (lock account, isolate host, block IP) and JSONL evidence export.

All telemetry is simulated (mock packet headers and synthetic events) for learning and demonstration. No live network capture.

## Echp — IOC Monitor & AI Simulator
[github.com/Rionangelfire/echp](https://github.com/Rionangelfire/echp)

- **IOC monitor** (Python): UDP syslog listener that matches log lines against an indicator list and writes JSON alerts, with email and SIEM alert hooks.
- **Nova Echo AI Simulator** (HTML): Gemini-powered chat terminal with tactical missions (scan, purge, isolate, decrypt, reboot). Needs a Gemini API key to run.

## Codex of Echoes — Tamper-Evident Log
[github.com/Rionangelfire/codex-of-echoes](https://github.com/Rionangelfire/codex-of-echoes)

Hash-chained log (SHA-256) with a verification script — append-only records where any edit breaks the chain. Tamper-evident, not tamper-proof.

## Skills
Python · JavaScript · HTML/CSS · SQL · JSON · GitHub

## Goal
Junior SOC analyst / technical support roles, building toward Security+.

More projects on my profile: [github.com/Rionangelfire](https://github.com/Rionangelfire)
