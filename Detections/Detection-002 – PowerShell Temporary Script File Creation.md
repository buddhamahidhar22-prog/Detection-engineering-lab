Behavior:

PowerShell created a temporary script file in the user's Temp directory.

Evidence:

Event ID: 11 (File Create)

Image:
C:\WINDOWS\system32\WindowsPowerShell\v1.0\PowerShell.exe

User:
Mahi\buddh

TargetFilename:
C:\Users\buddh\AppData\Local\Temp__PSScriptPolicyTest_a2ec5btg.1bx.ps1

Why It Matters:

PowerShell is commonly used by both administrators and attackers. Monitoring files created by PowerShell can help identify script execution, payload staging, or suspicious automation activity.

Investigation Questions:

Was the PowerShell execution expected?

Was the file created in a normal temporary directory?

Does the filename indicate legitimate PowerShell behavior?

Was any additional executable or script created afterward?

Assessment:

The file appears to be a temporary PowerShell script policy test file created during normal PowerShell operation. No suspicious indicators were identified.
