# Threat Detection Engineering Notes

## What Detection Engineering Is
Detection engineering is the process of identifying suspicious or malicious behavior and translating it into reliable, low-noise security detections.

The goal is not to detect every event, but to detect **meaningful behavior** that indicates a potential threat.

---

## Behavior-Based Detection
Effective detections focus on **what attackers do**, not just tools they use.

Examples:
- Scanning multiple ports across a host
- Executing encoded PowerShell commands
- Communicating over uncommon outbound ports

---

## Signal vs Noise
A good detection:
- Triggers on suspicious behavior
- Minimizes false positives
- Is easy for analysts to investigate

Noise is reduced by:
- Contextual filtering
- Understanding legitimate use cases
- Testing detections against real activity

---

## Role of Sigma
Sigma is a vendor-agnostic detection rule format that allows detections to be written once and converted to multiple SIEM platforms.

This project uses Sigma to demonstrate detection logic independent of any specific SIEM.

---

## Validation Mindset
Detections must be tested against known behavior to confirm they work as expected.

In this project, detections were validated using:
- Lab-generated activity
- Sysmon logs
- Controlled test scenarios
