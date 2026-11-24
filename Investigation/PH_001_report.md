
# PH-001: Banking Impersonation

## 1. Incident Overview

- Case ID: PH-001
- Scenario: Banking Impersonation
- Investigation Status: In Progress
- Email Type: Simulated phishing email
- Initial Assessment: Suspicious

## 2. Initial Email Analysis

- Claimed Sender: security@securebank-example.com
- Subject: Urgent: Your Account Has Been Temporarily Restricted
- Main Lure: Account restriction warning
- Requested Action: Verify account information
- Deadline: 24 hours

## 3. Initial Findings

- Urgency-based social engineering.
- Threat of permanent account suspension.
- Banking identity impersonation.
- Suspicious hostname:
  securebank-example.com.verify-account.invalid


## 4. Authentication Analysis

| Mechanism | Result | Observation |
|---|---|---|
| SPF | FAIL | Sender failed SPF evaluation |
| DKIM | NONE | No DKIM signature available |
| DMARC | FAIL | Visible From domain failed DMARC |

### Header Information

- From Domain: securebank-example.com
- Return-Path Domain: mailer-example.net
- Message-ID Domain: mailer-example.net

### Findings

1. Visible sender and Return-Path use different domains.
2. Message-ID uses mailer-example.net.
3. SPF authentication failed.
4. No DKIM signature was available.
5. DMARC authentication failed.

Note: All header results are simulated training evidence.


## 5. Preliminary Verdict

Suspicious — further investigation required.

## 6. Investigation Limitations

The sample is simulated and does not contain
original transport headers or actual authentication results.
