Overview
--------

This project focuses on understanding how endpoint security solutions handle repeated benign activities without generating unnecessary alerts. 
The goal is to analyze how false positives are avoided, how alert fatigue is reduced, and how analysts make informed decisions to balance security and business continuity.

Objective
---------

To study endpoint security behavior during normal user activities and understand why repeated scans or observations do not always result in alerts, emphasizing analyst judgment over automated responses.

Environment
-----------

1) Endpoint Protection: Windows Defender

2) Operating System: Windows

3) Log Sources: Windows Security Logs, Event Viewer

Baseline Validation
-------------------

Before analysis, the system baseline was confirmed:

1) Real-time protection enabled

2) Quick scan completed with no threats detected

3) System verified as clean prior to observation

Observed Activities
-------------------

The following legitimate user actions were performed:

1) File creation and modification

2) File renaming and deletion

3) Folder creation and cleanup

These actions represent normal daily user behavior in enterprise environments.

Findings
--------

1) Endpoint protection continuously scanned files during routine activities

2) No alerts or blocks were triggered

3) Protection History showed no malicious detections

4) Event logs confirmed normal system and security activity

5) No execution, persistence, or network indicators were observed

False Positive Analysis
-----------------------

Repeated scanning behavior does not indicate malicious activity. Modern endpoint security tools rely on context, behavior, and risk assessment rather than triggering alerts for every file operation.

Common reasons repeated observations occur without alerts:

1) Legitimate business activity

2) Heuristic monitoring without execution

3) Strict but non-blocking security policies

4) Continuous background scanning for prevention

Analyst Decision
----------------

No escalation or remediation was required.
Quarantining files or isolating the endpoint would have caused unnecessary disruption without improving security posture.

The correct action was to:

1) Validate system safety

2) Document findings

3) Continue monitoring

Key Learnings
-------------

1) Repeated scans are normal and expected

2) Alerts should be driven by risk, not repetition

3) Analyst judgment is critical in preventing alert fatigue

4) False positives can negatively impact business operations

5) Documentation is a core responsibility of security analysts

Conclusion
----------

This project demonstrates that effective security operations depend not only on detection tools but also on informed analyst decisions. 
Understanding when not to act is as important as responding to real threats, helping maintain both security and operational efficiency.



