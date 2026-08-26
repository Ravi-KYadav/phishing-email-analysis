# Phishing Email Analysis

Hands-on analysis of phishing emails to identify indicators of compromise (IOCs), assess sender authenticity, and document findings in analyst-style write-ups.

## 🎯 Objective

To develop the practical skill of examining a suspicious email the way a SOC analyst would when a phishing report lands in the queue — headers, authentication results, links, and attachments — and to produce clear, evidence-backed conclusions.

## 🧰 Tools Used

- Email header analyzers *<!-- e.g. MXToolbox Header Analyzer, Google Admin Toolbox Messageheader -->*
- *<!-- URL/attachment sandboxing tool used, e.g. VirusTotal, urlscan.io, any.run -->*
- Manual header inspection

## 🔧 Methodology

For each sample analyzed:

1. **Header Analysis**
   - Reviewed `Received` chain to trace the email's actual path and originating IP
   - Checked **SPF**, **DKIM**, and **DMARC** results to assess sender authenticity
   - Compared the `From` display name against the actual sending domain for spoofing
2. **Content & Link Analysis**
   - Inspected embedded URLs without clicking — hovered/extracted actual destination vs. displayed text
   - Checked URLs against reputation/sandboxing tools
   - Looked for urgency language, credential-harvesting patterns, and brand impersonation
3. **Attachment Analysis** (where applicable)
   - Identified file type and checked hash reputation
   - Noted red flags (e.g. macro-enabled documents, double extensions)
4. **IOC Extraction**
   - Documented sender IP, domain, URLs, file hashes as Indicators of Compromise
5. **Verdict & Reporting**
   - Classified as Phishing / Spear-Phishing / Spam / Legitimate, with supporting evidence

## 📋 Case Summary

| Case # | Type | Key Red Flag | Verdict |
|---|---|---|---|
| 1 | *<!-- e.g. Credential Harvesting -->* | *<!-- e.g. Spoofed domain, failed DMARC -->* | *<!-- Confirmed Phishing -->* |
| 2 | *<!-- add more -->* | | |

*<!-- Note: never upload real malicious attachments or live phishing links to a public repo. Use sanitized/defanged examples (e.g. hxxp:// instead of http://) or lab-generated samples only. -->*

## 🔍 Example Investigation Write-Up

**Subject Line:** *<!-- e.g. "Urgent: Verify Your Account" -->*
**Sender (displayed vs. actual):** *<!-- e.g. "IT Support" <it-support@company.com> vs actual: xxxx@random-domain.tk -->*
**SPF/DKIM/DMARC Result:** *<!-- pass/fail -->*
**IOCs Identified:** *<!-- IP, domain, URL, hash -->*
**Verdict:** *<!-- Phishing, with reasoning -->*
**Screenshot:** *<!-- header analysis screenshot, sanitized -->*

## 🧠 Skills Demonstrated

- Email header and authentication analysis (SPF/DKIM/DMARC)
- IOC identification and documentation
- Safe handling of malicious samples (defanging, sandboxing)
- Phishing pattern recognition (urgency, spoofing, credential harvesting)

## 📚 What I Learned

*<!-- 3-4 sentences: which authentication mechanism was most useful for catching fakes, a case that was trickier than expected, how this connects to a SOC's phishing report queue -->*

## 🔗 Related

Part of a 5-project SOC Analyst portfolio. See also: [SOC Alert Triage Practice](https://github.com/Ravi-KYadav/soc-alert-triage-practice) · [Network Traffic Analysis](https://github.com/Ravi-KYadav/network-traffic-analysis-wireshark-suricata)
