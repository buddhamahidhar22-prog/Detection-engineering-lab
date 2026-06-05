Behavior:

PowerShell executed an Invoke-WebRequest command to download content from example.com and save it locally as example.html.

Evidence:

PowerShell Script Block Logging (Event ID 4104):

Invoke-WebRequest https://example.com -OutFile "$env:TEMP\example.html"

User:
MAHI\buddh

Verification:

The file example.html was successfully created in the Temp directory.

Investigation Findings:

Expected telemetry included:

* PowerShell Script Block Logging (4104)
* Sysmon Network Connection (Event ID 3)
* Sysmon File Creation (Event ID 11)

Observed telemetry:

* Event ID 4104 present
* File successfully created
* No corresponding Event ID 11 observed

Assessment:

The activity executed successfully; however, the expected file creation telemetry was not recorded. This indicates a telemetry gap or Sysmon configuration limitation affecting visibility into this specific file creation event.

Detection Engineering Lesson:

Successful activity does not guarantee complete telemetry coverage. Logging configurations should be validated against expected behaviors to identify visibility gaps.
