
# PH-002 — Indicators of Compromise

## Case Information

- Case ID: PH-002
- Scenario: Delivery Notification Fraud
- Evidence Type: Simulated

## Indicators

| Type | Indicator |
|---|---|
| Sender | support@parcel-notification.example.invalid |
| Return-Path | bounce@bulk-mail.example.net |
| Hostname | parcel-redelivery.example.invalid |
| URL | https://parcel-redelivery.example.invalid/fee?id=PH002 |
| Source IP | 198.51.100.25 |
| Subject | Delivery Attempt Failed - Action Required |

## Security Notes

- The sender impersonates a parcel delivery service.
- The email requests personal information and a redelivery fee.
- DMARC authentication failed.
- The URL uses a reserved .invalid domain.
- The source IP belongs to a documentation-only range.

All indicators are simulated and must not be used
as production threat intelligence or blocklist entries.
