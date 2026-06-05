# Detection Engineering Lab

## Overview

This project was created to understand endpoint telemetry, Windows event logging, and detection engineering concepts using Sysmon and PowerShell logging.

The objective was to generate controlled activities, observe resulting telemetry, investigate events, and understand visibility gaps within logging configurations.

---

## Lab Environment

- Windows 11
- Sysmon
- PowerShell Logging
- Event Viewer

---

## Detection Use Cases

1. Local Account Creation Detection
2. PowerShell File Creation Detection
3. PowerShell Network Activity Detection
4. Parent-Child Process Analysis
5. PowerShell Command Execution Logging
6. PowerShell Download Activity
7. Telemetry Gap Analysis

---

## Key Skills Demonstrated

- Detection Engineering Fundamentals
- Security Monitoring
- Log Analysis
- Windows Security Logging
- PowerShell Logging
- Incident Investigation
- Root Cause Analysis
- Endpoint Telemetry Analysis

---

## Key Finding

A PowerShell download successfully created a file, but the expected Sysmon FileCreate event was not observed.

Investigation revealed that Sysmon FileCreate monitoring relied on include-based filtering and did not monitor the file location used during testing.

This demonstrated how telemetry gaps can impact detection coverage.

---

## Status

Project Completed
Documentation Uploaded
