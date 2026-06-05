Behavior:

PowerShell executed the Get-Process command and recorded the script block content through Event ID 4104.

Evidence:

Event ID: 4104 (PowerShell Script Block Logging)

User:
MAHI\buddh

Script Block Content:
Get-Process

Why It Matters:

Script Block Logging provides visibility into PowerShell commands executed within a session. Unlike process creation logs, it captures command content and can help identify administrative actions, automation, or malicious PowerShell activity.

Investigation Questions:

Who executed the command?

What command was executed?

Was the command expected?

Did the command result in further process creation, file creation, or network activity?

Assessment:

The activity was generated during a controlled lab exercise. The observed PowerShell command was legitimate and expected.
