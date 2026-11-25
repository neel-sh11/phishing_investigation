
# PH-003: Business Invoice Fraud

## 1. Incident Overview

- Case ID: PH-003
- Scenario: Business Invoice Fraud
- Investigation Status: In Progress
- Email Type: Simulated BEC attempt
- Initial Assessment: Suspicious

## 2. Initial Email Analysis

- Claimed Sender: Accounts Department
- Sender Address: accounts@global-supplies.example.invalid
- Subject: Urgent: Updated Payment Details for Invoice INV-2026-1042
- Invoice Number: INV-2026-1042
- Main Lure: Updated supplier banking details
- Requested Action: Use revised payment instructions
- Deadline: 24 hours

## 3. Initial Findings

1. Business identity impersonation.
2. Payment redirection attempt.
3. Urgency-based social engineering.
4. Financial manipulation targeting the finance department.
5. Potential Business Email Compromise (BEC).


## 4. Authentication Analysis

| Mechanism | Result | Observation |
|---|---|---|
| SPF | PASS | external-mail.example.net authenticated |
| DKIM | PASS | Signature verified for external-mail.example.net |
| DMARC | FAIL | Authenticated domains do not align with visible From |

### Header Information

- From Domain: global-supplies.example.invalid
- Return-Path Domain: external-mail.example.net
- Message-ID Domain: external-mail.example.net
- SPF Domain: external-mail.example.net
- DKIM Domain: external-mail.example.net

### Findings

1. SPF authentication passed.
2. DKIM authentication passed.
3. Both authentication domains differ from the visible From domain.
4. DMARC failed due to domain alignment failure.

Note: All header information and authentication outcomes
are simulated training evidence.

## 5. Preliminary Verdict

Suspicious — further investigation required.

## 6. Investigation Limitations

The sample is simulated and does not contain
original transport headers or actual authentication results.
