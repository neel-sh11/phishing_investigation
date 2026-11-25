
# PH-002: Delivery Notification Fraud

## 1. Incident Overview

- Case ID: PH-002
- Scenario: Delivery Notification Fraud
- Investigation Status: In Progress
- Email Type: Simulated phishing email
- Initial Assessment: Suspicious

## 2. Initial Email Analysis

- Claimed Sender: Parcel Delivery Support
- Sender Address: support@parcel-notification.example.invalid
- Subject: Delivery Attempt Failed - Action Required
- Main Lure: Failed parcel delivery
- Requested Action: Confirm address and pay redelivery fee
- Deadline: 12 hours

## 3. Initial Findings

1. Delivery service impersonation.
2. Urgency-based social engineering.
3. Fear of parcel return.
4. Unexpected redelivery payment request.
5. Suspicious delivery-related URL.
## 4. Authentication Analysis

| Mechanism | Result | Observation |
|---|---|---|
| SPF | PASS | bulk-mail.example.net authenticated |
| DKIM | PASS | Signature verified for bulk-mail.example.net |
| DMARC | FAIL | Authenticated domains do not align with visible From |

### Header Information

- From Domain: parcel-notification.example.invalid
- Return-Path Domain: bulk-mail.example.net
- Message-ID Domain: bulk-mail.example.net
- SPF Domain: bulk-mail.example.net
- DKIM Domain: bulk-mail.example.net

### Findings

1. SPF authentication passed.
2. DKIM authentication passed.
3. Both authenticated domains differ from the visible From domain.
4. DMARC failed due to alignment failure.

Note: All authentication results are simulated training evidence.


## 5. Preliminary Verdict

Suspicious — further investigation required.

## 6. Investigation Limitations

The sample is simulated and does not contain
original transport headers or actual authentication results.
