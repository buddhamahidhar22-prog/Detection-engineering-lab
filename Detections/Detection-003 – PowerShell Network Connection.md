Behavior:

PowerShell initiated an outbound network connection over HTTPS.

Evidence:

Event ID: 3 (Network Connection)

Image:
C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe

Protocol:
TCP

Destination Port:
443

Destination IP:
2606:4700:10:0:0:0:6814:179a

User:
Mahi\buddh

Why It Matters:

PowerShell is frequently used by administrators and attackers. Monitoring outbound network connections from PowerShell can help identify script downloads, command-and-control traffic, or suspicious automation.

Investigation Questions:

Was the PowerShell execution expected?

Was the destination trusted?

Was the connection initiated during normal business activity?

Were any files downloaded or executed afterward?

Assessment:

The network connection was generated during a controlled lab exercise using PowerShell. The observed behavior is expected and benign.
