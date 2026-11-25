
# PH-001 — URL Analysis

## 1. Suspicious URL

http://securebank-example.com.verify-account.invalid/login

## 2. URL Breakdown

- Scheme: HTTP
- Hostname: securebank-example.com.verify-account.invalid
- Domain ending: .invalid
- Path: /login

## 3. Observations

1. The URL uses unencrypted HTTP.
2. The hostname contains a banking-related name.
3. The actual hostname does not belong to the claimed banking domain.
4. The URL uses a misleading hostname structure.
5. The login path is consistent with the email's account verification request.

## 4. Security Assessment

The URL contains indicators of deceptive domain presentation.

The .invalid domain is reserved for testing and cannot represent a normal publicly registered website.

## 5. Limitations

- No live website was accessed.
- No DNS resolution was performed.
- No redirect chain was examined.
- No external reputation check was performed.

## 6. Preliminary URL Verdict

Suspicious URL — simulated training evidence.
