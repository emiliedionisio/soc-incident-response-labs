# Incident Postmortem

Incident ID: IR-2023-001

## Summary

A phishing email containing a malicious attachment was delivered to user Jane Smith.

The attachment executed after being opened. The infected workstation (PC-001) was isolated from the network and restored after malware removal.

## Impact

- One workstation affected
- Potential ransomware execution
- No evidence of lateral movement

## Indicators of Compromise

IP Address: 45.142.166.228

MD5 Hash: 44d88612fea8a8f36de82e1278abb02f

## Investigation

VirusTotal confirmed:

- Malicious IP reputation
- Association with phishing infrastructure

The MD5 hash was detected by 64 of 67 antivirus engines. The sample was identified as the EICAR test file.

## Containment

- User notified
- Workstation disconnected
- Malware removed
- System restored

## Lessons Learned

Recommendations:

- Improve email filtering
- User awareness training
- Maintain offline backups
- Patch systems regularly
- Improve endpoint detection

## Classification

True Positive
