# Phishing Email Analysis

**SOC Analyst L1 Portfolio Project · Email Security & Phishing Investigation**

> **Status: Active / evidence library being expanded**

## Objective
Develop the practical workflow for investigating a suspicious email report: inspect headers and authentication results, evaluate links and attachments, extract IOCs, determine a verdict and document the evidence.

## Investigation Workflow

1. **Header Analysis** — review the `Received` chain and sender infrastructure.
2. **Authentication Checks** — evaluate SPF, DKIM and DMARC results.
3. **Sender Validation** — compare the display name, `From` address and sending domain.
4. **Link Analysis** — inspect the actual destination without directly visiting suspicious links.
5. **Attachment Review** — identify file type, hashes and suspicious characteristics where applicable.
6. **IOC Extraction** — record sender IPs, domains, URLs and file hashes.
7. **Verdict & Reporting** — classify the message and document the supporting evidence.

## Case Documentation Standard

| Field | Output |
|---|---|
| Subject / Sender | Message identity |
| Authentication | SPF / DKIM / DMARC results |
| URLs / Attachments | Destination and file observations |
| IOCs | IPs, domains, URLs, hashes |
| Verdict | Phishing / Spear-phishing / Spam / Legitimate |
| Rationale | Evidence supporting the decision |

## SOC Skills Demonstrated

Email-header analysis · SPF/DKIM/DMARC · URL analysis · IOC extraction · phishing pattern recognition · analyst reporting

## Evidence Roadmap

This repository is being expanded with sanitized case write-ups and screenshots. Real malicious attachments, credentials and live phishing links will not be published.

## Scope & Ethics

Educational analysis of authorized samples and simulated exercises only.