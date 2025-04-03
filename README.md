# 🕵️‍♂️ Nightfall Operation – Threat Intelligence Report

Technical analysis of a real-world social engineering campaign delivering a malicious payload via the domain `night-fall.site`. This repository documents the investigation, findings, and threat indicators collected throughout the research process.

---

## 🧩 Threat Summary

- **Primary Domain:** night-fall.site
- **Secondary Domain:** arenawars.io (hosted on Google Cloud)
- **Delivery Method:** Fake download button / social engineering
- **Malicious File:** Unknown binary (pending dynamic analysis)
- **Suspected Behavior:** Downloader / RAT
- **Evasion Level:** High – likely using obfuscation and anti-analysis techniques

---

## 🔍 Repository Contents

| File | Description |
|------|-------------|
| `analysis/static_analysis.md` | Static analysis: PE headers, strings, structure, obfuscation |
| `analysis/dynamic_analysis.md` | Dynamic behavior during runtime in VM |
| `analysis/network_traffic.md` | Traffic captured with Wireshark and analysis |
| `indicators/domains.txt` | List of malicious or suspicious domains |
| `indicators/ips.txt` | Malicious IPs identified during analysis |
| `indicators/hashes.txt` | File hashes (MD5, SHA-1, SHA-256) |
| `timeline.md` | Timeline of the investigation and threat discovery |
| `conclusions.md` | Final thoughts, potential attribution, and risks |
| `tools_used.md` | Software and tools utilized for analysis |

---

## 🛡️ Responsible Reporting

The domain `arenawars.io` was discovered to be hosted on Google Cloud infrastructure and associated with the same threat actor. A formal abuse report was submitted to Google Cloud for further review and possible takedown. Ethical reporting practices were followed throughout this investigation.

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

This project is provided for educational and research purposes only.

---

Sebas is the lead analyst behind this operation. Follow his work and stay updated for deeper malware and threat research coming soon.



