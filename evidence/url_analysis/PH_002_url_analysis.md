
# PH-002 — URL Analysis

## 1. Suspicious URL

https://parcel-redelivery.example.invalid/fee?id=PH002

## 2. URL Breakdown

- Scheme: HTTPS
- Hostname: parcel-redelivery.example.invalid
- Domain ending: .invalid
- Path: /fee
- Query Parameter: id=PH002

## 3. Observations

1. The URL uses HTTPS encryption.
2. The hostname does not establish any legitimate delivery service identity.
3. The .invalid domain is reserved for testing.
4. The /fee path is consistent with the email's payment request.
5. The query parameter identifies the simulated case.

## 4. Security Assessment

The URL is suspicious in the context of the simulated
delivery notification email.

HTTPS does not establish website legitimacy.

## 5. Limitations

- No live website was accessed.
- No DNS resolution was performed.
- No redirect chain was examined.
- No external reputation check was performed.

## 6. Preliminary URL Verdict

Suspicious — simulated training evidence.
