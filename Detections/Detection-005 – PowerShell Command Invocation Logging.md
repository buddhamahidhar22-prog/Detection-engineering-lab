Behavior:

PowerShell executed a Compress-Archive operation and loaded the System.IO.Compression.FileSystem assembly.

Evidence:

Event ID: 4103 (PowerShell Module Logging)

Command:
Add-Type

Assembly:
System.IO.Compression.FileSystem

Host Application:
PowerShell.exe Compress-Archive

User:
WORKGROUP\SYSTEM

Observed Activity:

An ASUS GlideX log file was compressed into a ZIP archive.

Why It Matters:

PowerShell module logging provides visibility into commands executed within PowerShell sessions. This telemetry can help identify administrative automation, scripting activity, and potentially malicious PowerShell usage.

Investigation Questions:

Who executed the command?

What script or application initiated PowerShell?

What files were accessed or modified?

Was the PowerShell activity expected?

Assessment:

The activity appears legitimate and associated with ASUS GlideX log archival operations. No suspicious indicators were identified.
