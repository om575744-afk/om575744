# SIEM Log Analysis Lab

## Overview
[I am building a home SIEM lab to collect security logs from a Linux system and practice investigating suspicious activity. This project focuses on log ingestion, basic detection, and alert triage.nces. Example: "Built a small SIEM lab to collect security logs and investigate suspicious activity."
## Tools Used
- wazuh
- [- Linux system logs (auth.log and syslog)]
- [- Ubuntu 22.04 (virtual machine)]

## What I Did
1. [ Set up a Linux virtual machine to act as the monitored host]
2. [ Installed and configured Wazuh manager and agent]
3. [. Verified that authentication logs are being collected in the SIEM]
4. [Created a basic detection rule for repeated failed login attempts (in progress)]

## Skills Demonstrated
- SIEM implementation
- Log analysis
- Alert triage

## Screenshots
Add images here after you finish the lab. In GitHub markdown:

```markdown
![SIEM dashboard](screenshots/dashboard.png)
```

Save images in a `screenshots/` folder inside this project.

## What I Learned
- [- Correlating failed login events by source IP helps identify brute-force activity]
- [- Detection rules need tuning — too sensitive creates noise, too loose misses real attacks]

## Optional: Sample Query or Rule
```
[FILL INRule: Multiple failed SSH login attempts
- Trigger: 5+ failed authentication events from the same source IP within 300 seconds
- Log source: auth.log / SSH events
- Action: Review source IP, check for successful login after failures, block IP if malicious
: Paste a Splunk SPL search, Elastic KQL query, or Wazuh rule if you have one]
```
