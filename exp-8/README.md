# Experiment 8: Mapping a Defensive Incident to MITRE ATT&CK

## Aim

To map a fictional incident timeline to relevant MITRE ATT&CK tactics and techniques and identify defensive detection opportunities.

## Scenario

An organization reviews synthetic endpoint and identity logs. The records show an unusual sign-in, followed by a new process on a workstation and an outbound connection that the endpoint team later blocked. The records contain no real usernames, addresses, or credentials.

## Tools

- MITRE ATT&CK Enterprise knowledge base
- Optional: ATT&CK Navigator for visualizing a defensive coverage matrix
- The fictional timeline below

## Fictional Timeline

| Time | Synthetic observation |
|---|---|
| 09:02 | Identity service records a sign-in outside the user's usual pattern. |
| 09:07 | Endpoint telemetry records an unexpected script interpreter launch. |
| 09:09 | The endpoint agent records a blocked outbound connection. |
| 09:15 | The account is disabled and the workstation is isolated for investigation. |

## Procedure

1. Read the timeline and list the evidence actually present. Keep assumptions separate from observations.
2. Consult the MITRE ATT&CK Enterprise knowledge base and identify candidate tactics and techniques that may describe the observed behaviors.
3. For each candidate, record the ATT&CK identifier, the matching observation, confidence, and what additional defensive evidence would be needed to confirm the mapping.
4. In ATT&CK Navigator or a table, mark which events existing controls detected and which events were blocked.
5. Recommend defensive improvements, such as stronger authentication, script logging, endpoint monitoring, alert triage, and incident-response playbooks.
6. Do not reproduce the scenario as an attack or execute any techniques.

## Mapping Table

| Synthetic observation | Candidate ATT&CK tactic/technique | Evidence and confidence | Detection or prevention improvement |
|---|---|---|---|
| Unusual sign-in | | | |
| Unexpected script process | | | |
| Blocked outbound connection | | | |

## Result

The fictional events were mapped to candidate ATT&CK behaviors, with confidence and defensive coverage documented.

## Conclusion

ATT&CK provides a shared vocabulary for describing observed adversary behaviors. A mapping is a hypothesis supported by evidence, not proof that a particular actor or technique was involved.
