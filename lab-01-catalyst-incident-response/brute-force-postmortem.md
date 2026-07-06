# Incident Postmortem

Incident ID: IR-2023-003

## Summary

An attacker successfully performed a brute force attack against Server-001 using Hydra.

After obtaining access, persistence malware was installed. The intrusion was detected by the IDS.

## Impact

- Unauthorized access
- Persistence malware installed
- Server temporarily isolated

## Indicators of Compromise

Attacker IP: 95.181.152.9

MD5 Hash: 5a064113d8863eb34253dbee7a271974

Malicious Domain: epcdiagnostic.com

## Investigation

VirusTotal: 58 of 71 engines detected the malware. Several vendors identified it as LokiBot.

AbuseIPDB: The IP had minimal historical reports. This demonstrated that low reputation scores do not necessarily indicate a safe IP.

## Containment

- Server isolated
- Credentials reset
- Malware removed
- Server restored

## Lessons Learned

Recommendations:

- Enable MFA
- Implement account lockout policies
- Install Fail2Ban
- Monitor authentication logs
- Block unused geographic regions
- Continue IDS monitoring

## Classification

True Positive
