# Phishing Email Analysis

**SOC Analyst L1 Lab · Email Security · Phishing Investigation**

> 🟢 **Status: Active — evidence library is being expanded**

### 🧰 Stack
<img src="https://img.shields.io/badge/Email-Analysis-555555" alt="Email Analysis"> <img src="https://img.shields.io/badge/URL-Analysis-555555" alt="URL Analysis"> <img src="https://img.shields.io/badge/IOC-Analysis-555555" alt="IOC Analysis">

## 🎯 Why I built this lab
I want to practise the workflow behind a real suspicious-email report: inspect the message, validate the sender and authentication, examine links/attachments, extract IOCs, make a verdict and explain the evidence.

## 🔎 Investigation workflow

1. **Header analysis** — `Received` chain and sender infrastructure.
2. **Authentication checks** — SPF, DKIM and DMARC.
3. **Sender validation** — display name, `From` address and sending domain.
4. **Link analysis** — inspect the actual destination without directly visiting suspicious links.
5. **Attachment review** — file type, hashes and suspicious characteristics where applicable.
6. **IOC extraction** — sender IPs, domains, URLs and file hashes.
7. **Verdict & reporting** — classify the message and document the supporting evidence.

## 🗂️ Case standard

| Field | Output |
|---|---|
| Subject / Sender | Message identity |
| Authentication | SPF / DKIM / DMARC results |
| URLs / Attachments | Destination and file observations |
| IOCs | IPs, domains, URLs, hashes |
| Verdict | Phishing / Spear-phishing / Spam / Legitimate |
| Rationale | Evidence supporting the decision |

## 🧠 What I'm practising
**Email-header analysis • SPF/DKIM/DMARC • URL analysis • IOC extraction • phishing pattern recognition • analyst reporting**

## 📌 Evidence roadmap

This repository is being expanded with sanitised case write-ups and screenshots. Real malicious attachments, credentials and live phishing links will not be published.

## Scope & ethics
Educational analysis of authorised samples and simulated exercises only.
