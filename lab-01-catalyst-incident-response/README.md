# Lab 01 - Catalyst Incident Response

## Overview

This lab demonstrates a complete Incident Response workflow using the Catalyst Incident Response Platform.

Two separate incidents were investigated:

1. Phishing Malware
2. Brute Force Attack

The exercise included:

- installing Catalyst
- documenting incidents
- creating artifacts
- investigating Indicators of Compromise
- enriching IoCs with external intelligence
- documenting findings
- closing incidents
- writing post-incident reports

## Lab Environment

Operating System: Ubuntu Linux

Platform: Catalyst

Threat Intelligence:

- VirusTotal
- AbuseIPDB

## Objectives

Learn how SOC analysts:

- document incidents
- investigate evidence
- classify incidents
- perform post-incident reviews

## Incident Workflow

1. Create Incident
2. Add Artifacts
3. Investigate IoCs
4. Enrich Evidence
5. Document Findings
6. Close Incident
7. Lessons Learned

## Incident 1 - Phishing Malware

See phishing-postmortem.md

## Incident 2 - Brute Force + Persistence Malware

See brute-force-postmortem.md

## Troubleshooting

See troubleshooting.md

## Screenshots

The screenshots folder contains the complete investigation process, including incident creation, artifact tagging, and threat intelligence lookups.

## Lessons Learned

One of the biggest takeaways from this lab was understanding that SIEMs and Incident Response platforms serve different purposes.

A SIEM helps detect attacks. An Incident Response platform like Catalyst helps manage the investigation.

Together they provide a complete incident response workflow.
