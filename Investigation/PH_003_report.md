
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


## 5. Final Investigation Verdict

Verdict: SUSPECTED BEC / PAYMENT REDIRECTION FRAUD

Confidence: High (within simulated evidence)

### Supporting Evidence

1. Supplier identity impersonation.
2. Unexpected request to change payment instructions.
3. Urgency-based financial manipulation.
4. SPF and DKIM passed for a domain different from the visible From domain.
5. DMARC alignment failure.

### Analyst Conclusion

The email demonstrates characteristics of a simulated
Business Email Compromise (BEC) payment-redirection attempt.

The sender requests a change to supplier payment instructions
without providing independently verifiable authorization.

The authentication mismatch adds suspicion but does not
independently establish malicious intent.

The request must be independently verified before
any payment instructions are changed.

All findings are based on simulated training evidence.


## 6. Investigation Limitations

The sample is simulated and does not contain
original transport headers or actual authentication results.

## 7. Recommended Mitigation

1. Do not process payment changes based solely on email.
2. Verify updated bank details through a trusted contact channel.
3. Require dual authorization for supplier payment changes.
4. Notify the finance department and security team.
5. Preserve the original email and associated evidence.
6. Review recent transactions for unauthorized transfers.
7. Establish supplier verification procedures.

