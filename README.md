Phishing Email Investigation
A Junior SOC Analyst portfolio project focused on analyzing simulated phishing emails using header inspection, SPF/DKIM/DMARC checks, URL and payment-lure analysis, and structured incident reporting.
Cases
￼ PH-001 — Banking Impersonation (Completed): Report · Sample · Header · URL Analysis
￼ PH-002 — Delivery Notification (Completed): Report · Sample · Header · URL Analysis · IOCs
￼ PH-003 — Business Invoice (BEC) (Completed): Report · Sample · Header · Payment Analysis · IOCs
What This Project Covers
￼ Header & Routing Analysis: Tracing ⁠From⁠, ⁠Return-Path⁠, ⁠Message-ID⁠, and ⁠Received⁠ hops for sender mismatches.
￼ Email Authentication: Evaluating ⁠SPF⁠, ⁠DKIM⁠, and ⁠DMARC⁠ results to detect domain spoofing and alignment failures.
￼ URL & BEC Triage: Breaking down deceptive domains, urgency lures, and fraudulent payment-change requests safely.
￼ SOC Reporting: Documenting IOCs, confidence levels, limitations, and remediation steps.
Workflow
1. Collect simulated ⁠.eml⁠ sample and assign a case ID.
2. Inspect raw headers and authentication results (⁠SPF⁠, ⁠DKIM⁠, ⁠DMARC⁠).
3. Analyze suspicious URLs, payment lures, and social engineering indicators.
4. Log supporting artifacts in ⁠evidence/⁠ and finalize the verdict in ⁠Investigation/⁠.
Repository Structure
￼ ⁠Investigation/⁠ — Case investigation reports (⁠PH_001_report.md⁠, ⁠PH_002_report.md⁠, ⁠PH_003_report.md⁠)
￼ ⁠Sample/⁠ — Simulated ⁠.eml⁠ email samples
￼ ⁠evidence/⁠ — Extracted headers (⁠header/⁠), URL breakdowns (⁠url_analysis/⁠), payment analysis, IOCs, and methodology
Disclaimer & Author
￼ Disclaimer: All emails, domains (⁠.invalid⁠, ⁠example.com⁠), and IPs (RFC 5737 documentation ranges) are simulated training artifacts for educational use only.
￼ Author: Neel — GitHub · LinkedIn
