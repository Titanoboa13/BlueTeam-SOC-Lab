### Alert 001 – Initial Triage
Evidence: 
<img width="1785" height="166" alt="alert-001-overview" src="https://github.com/user-attachments/assets/5c4f2b9b-0b6f-4524-b41b-50f9b1e63342" />

## Alert Information

Alert name: windows_lab

Rule ID: 60106

Severity level: 3

Timestamp: Dec 22, 2025 09:56:37.401

Source host: 001

Data source: Windows Security

## Observed Activity
The alert indicates a successful Windows logon event on host 001, associated with the agent name "windows_lab".

## Initial Analyst Assessment
The alert reports a successful Windows logon event without evidence of failed authentication attempts, abnormal logon types, or suspicious source information. Successful logons are common operational events and, in isolation, do not indicate malicious activity. Additional contextual indicators would be required to suggest misuse of valid credentials.

## Preliminary Classification
False Positive

## MITRE ATT&CK Mapping

Tactic: N/A

Technique: N/A

Justification: Although the rule references T1078 (Valid Accounts), the observed activity does not demonstrate adversarial use of credentials. No anomalous login behavior, suspicious source, or privilege abuse indicators are present.

## Next Action
Close

## Reason:
The event represents a routine successful authentication without indicators of compromise. No escalation or further investigation is required at Level-1.


### Alert 002
Evidence:
<img width="1837" height="54" alt="alert-002-overview" src="https://github.com/user-attachments/assets/9f759351-7baa-4628-9939-b7345ac44068" />

## Alert Information

Alert name: Service startup type was changed

Rule ID: 61104

Severity level: 3

Timestamp: Dec 22, 2025 14:04:10

Source host: windows_lab

Data source: Windows System (Service Control Manager)

## Observed Activity
The Windows Background Intelligent Transfer Service (BITS) startup type was changed from Manual to Automatic. The change was logged by the Service Control Manager (Event ID 7040) and is informational in nature, with no associated user or process details.

## Preliminary Classification
Informational

## MITRE ATT&CK Mapping

Tactic: N/A

Technique: N/A

Justification: The observed service configuration change lacks evidence of adversarial intent or follow-on malicious activity. MITRE ATT&CK mapping requires additional context that is not present in this event.

## Next Action

Close

## Reason:
The service startup type change for BITS appears consistent with normal system or update-related behavior. No indicators of compromise, suspicious processes, or repeated changes were observed. No escalation or further monitoring is required at Level-1.
