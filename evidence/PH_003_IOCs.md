
# PH-003 — Indicators of Compromise

## Case Information

- Case ID: PH-003
- Scenario: Business Invoice Fraud
- Evidence Type: Simulated BEC attempt

## Indicators

| Type | Indicator |
|---|---|
| Sender | accounts@global-supplies.example.invalid |
| Return-Path | bounce@external-mail.example.net |
| Message-ID Domain | external-mail.example.net |
| Source IP | 192.0.2.80 |
| Invoice Reference | INV-2026-1042 |
| Subject | Urgent: Updated Payment Details for Invoice INV-2026-1042 |

## Business Fraud Indicators

- Unexpected supplier payment-detail change.
- Urgency surrounding an outstanding invoice.
- Request to use revised payment instructions.
- Sender identity does not align with authenticated domains.

## Security Notes

All evidence is simulated.
The source IP is reserved for documentation.
The invoice reference is fictional.

No actual bank account or payment destination was provided.
