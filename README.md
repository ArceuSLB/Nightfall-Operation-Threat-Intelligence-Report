# 🕵️‍♂️ Nightfall Operation – Threat Intelligence Report

This repository documents the threat research and technical analysis of a real-world social engineering campaign involving the domains `night-fall.site` and `arenawars.io`. The goal of this project is to analyze the tactics used by the threat actor, document indicators of compromise (IoCs), and provide defensive recommendations.

---

## 🧩 Threat Summary

- **Primary Domain:** night-fall.site
- **Secondary Domain:** arenawars.io (hosted on Google Cloud)
- **Delivery Method:** Fake download button (social engineering)
- **Payload Behavior:** Downloader / RAT (Pending dynamic confirmation)
- **Evasion Tactics:** Likely obfuscation, anti-analysis behavior, cloud-based hosting

---

## 🔍 Repository Contents

| File | Description |
|------|-------------|
| `analysis/static_analysis.md` | PE headers, strings, section analysis |
| `analysis/dynamic_analysis.md` | Runtime behavior in controlled VM |
| `analysis/network_traffic.md` | Network indicators, command & control |
| `indicators/domains.txt` | Related domains |
| `indicators/ips.txt` | IP addresses observed |
| `indicators/hashes.txt` | File hashes (MD5, SHA1, SHA256) |
| `timeline.md` | Chronological record of research process |
| `conclusions.md` | Summary, risks, and potential attribution |
| `tools_used.md` | Tools and techniques used in this research |

---

## 🛡️ Responsible Reporting

The domain `arenawars.io` was found to be hosted on Google Cloud and associated with the threat infrastructure. A formal abuse report was submitted to Google Cloud. All analysis was conducted in isolated virtual environments using ethical practices.

---

## ⚔️ Tools Used

- Ghidra
- Wireshark
- PEStudio
- Procmon
- VirusTotal / VTGraph
- Any.Run
- Fakenet-NG

---

## 🔗 License

This repository is intended for educational and research purposes only.
