# Phishing Email Analysis

**SOC Analyst L1 Lab · Email Security · Phishing Investigation**

> 🟢 **Status: Active — case library is being expanded**

### 🧰 Stack
<img src="https://img.shields.io/badge/Email-Analysis-555555" alt="Email Analysis"> <img src="https://img.shields.io/badge/URL-Analysis-555555" alt="URL Analysis"> <img src="https://img.shields.io/badge/IOC-Analysis-555555" alt="IOC Analysis">

## 🎯 Objective
Practise the workflow behind a real suspicious-email report: preserve the message, validate the sender and authentication, examine links and attachments, extract IOCs, reach a verdict and explain the evidence.

## 🗺️ Repository map

| Path | Purpose |
|---|---|
| [`docs/01-investigation-standard.md`](docs/01-investigation-standard.md) | Repeatable email-analysis workflow |
| [`cases/`](cases/) | Individual investigations and reusable case template |
| [`evidence/`](evidence/) | Evidence quality and sanitisation rules |

## 🔎 Investigation workflow

1. **Preserve** the message and record its source.
2. **Validate** sender identity and SPF/DKIM/DMARC where available.
3. **Inspect** URLs, destinations and attachments safely.
4. **Extract** domains, URLs, IPs and hashes.
5. **Correlate** indicators with available context.
6. **Classify** the message and assess severity.
7. **Report** the evidence, rationale and recommended action.

## 🧠 Skills being practised
**Email-header analysis • SPF/DKIM/DMARC • URL analysis • IOC extraction • phishing recognition • analyst reporting**

## Scope & ethics
Educational analysis of authorised samples and simulated exercises only. Real credentials, live malicious attachments and operational phishing links are not published.
