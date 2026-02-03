# Detection Validation

## Network Scan Detection
- Tool Used: nmap
- Expected Result: Multiple Sysmon Event ID 3 entries
- Detection Triggered: Yes

## PowerShell Detection
- Command Used: powershell -enc
- Expected Result: Sysmon Event ID 1 with encoded flag
- Detection Triggered: Yes

## Outbound Port Detection
- Port Tested: 4444
- Expected Result: Sysmon Event ID 3
- Detection Triggered: Yes

