# Email Investigation Standard

1. Preserve the message and record its source.
2. Review sender, display name and sending domain.
3. Validate SPF, DKIM and DMARC where available.
4. Inspect URLs and actual destinations without blindly opening suspicious links.
5. Review attachments by type and hash where applicable.
6. Extract IOCs: domains, URLs, IPs and hashes.
7. Correlate indicators with available context.
8. Assign a verdict and severity, then document the recommended action.

The objective is an evidence-backed decision, not simply a suspicious-looking email classification.
