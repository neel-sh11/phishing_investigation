Phishing Email Investigation
A Junior SOC Analyst portfolio project focused on analyzing simulated phishing emails using header inspection, SPF/DKIM/DMARC checks, URL analysis, and structured incident reporting.
Cases
￼ PH-001 — Banking Impersonation (Completed): Report · Sample · Header · URL Evidence
￼ PH-002 — Delivery Notification (Completed): Suspicious URLs & social engineering
￼ PH-003 — Business Invoice (Planned): Business Email Compromise (BEC) indicators
What This Project Covers
￼ Header & Routing Analysis: Tracing ⁠From⁠, ⁠Return-Path⁠, ⁠Message-ID⁠, and ⁠Received⁠ hops for sender mismatches.
￼ Email Authentication: Evaluating ⁠SPF⁠, ⁠DKIM⁠, and ⁠DMARC⁠ results to detect domain spoofing.
￼ URL & Content Triage: Breaking down deceptive domains, urgency lures, and credential-harvesting indicators safely.
￼ SOC Reporting: Documenting IOCs, confidence levels, limitations, and remediation steps.
Workflow
1. Collect simulated ⁠.eml⁠ sample and assign a case ID.
2. Inspect raw headers and authentication results (⁠SPF⁠, ⁠DKIM⁠, ⁠DMARC⁠).
3. Analyze suspicious URLs and social engineering lures.
4. Log supporting artifacts in ⁠evidence/⁠ and finalize the verdict in ⁠Investigation/⁠.
Repository Structure
￼ ⁠Investigation/⁠ — Completed case reports (⁠PH_001_report.md⁠)
￼ ⁠Sample/⁠ — Simulated ⁠.eml⁠ samples and case index
￼ ⁠evidence/⁠ — Extracted headers (⁠header/⁠), URL breakdowns (⁠url_analysis/⁠), and ⁠methodologies⁠
Disclaimer & Author
￼ Disclaimer: All emails, domains (⁠.invalid⁠, ⁠example.com⁠), and IPs (⁠203.0.113.45⁠) are simulated training artifacts for educational use only.
￼ Author: Neel — GitHub · LinkedIn
