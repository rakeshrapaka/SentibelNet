SentinelNet is designed to monitor network traffic in real time and detect suspicious or malicious activity using machine learning.
It learns from past data (like NSL-KDD) to classify behavior as normal or attack and raises alerts when anomalies are detected.

In real-world enterprise networks, systems like this are how companies prevent intrusions, DDoS attacks, and data breaches — it’s the AI layer that helps security teams identify threats early.


Think of SentinelNet as the AI security camera inside a company’s network:
the firewall stops known threats, while SentinelNet intelligently spots abnormal behavior that traditional tools might miss — and sends an alert to the security dashboard.

What’s happening here:

Internet Traffic → Firewall:
The firewall acts as the first gatekeeper — blocking known malicious IPs, ports, or basic rule violations.
But many unknown or stealth attacks still pass through.

Firewall → SentinelNet:
SentinelNet is the next layer of defense.
It analyzes live traffic at a deeper level — not just headers, but patterns of behavior.

SentinelNet (ML Model):

Extracts network flow features

Classifies each flow as normal or attack

Uses learned patterns from datasets like NSL-KDD or CICIDS2017

SentinelNet → Alert Logs:
When an anomaly or attack signature is detected, SentinelNet:

Generates a log entry

Flags it in an alert dashboard

Optionally sends a signal to the security team (or a SIEM system like Splunk)

SOC Team (Security Operations Center):
Security analysts review these alerts in real time and respond — blocking IPs, quarantining systems, or investigating incidents.
