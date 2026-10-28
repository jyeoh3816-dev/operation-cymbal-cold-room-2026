# Operation Cymbal: Cold Room CTF 2026

**An evidence-driven cybersecurity investigation portfolio | Zero Day Legend**

> **Status:** Preparing for competition. Investigation results and technical conclusions will be added only after participation and subject to organiser publication rules.

## Overview

This repository documents my learning and investigation methodology for **Operation Cymbal: Cold Room**, an online Capture The Flag (CTF) event hosted by the **Google Cloud Security Community** in partnership with **Hack The Box**.

The competition presents three incidents within a frozen fictional enterprise environment. Participants reconstruct what occurred by correlating telemetry spanning identity, endpoints, cloud activity, email, development/build systems and data. The emphasis is on separating malicious activity from normal operations and supporting conclusions with defensible evidence.

**Event:** 30 October 2026, 00:00 SGT – 2 November 2026, 00:00 SGT (72 hours)  
**Format:** Online, Jeopardy-style  
**Official event:** https://ctf.hackthebox.com/event/details/operation-cymbal-cold-room-3631  
**Branding:** Zero Day Legend  
**Participant:** Jerry | Higher Nitec in Cyber & Network Security, ITE College West

**Participation note:** The official event page lists a maximum of one player per team. Zero Day Legend is used here as personal portfolio branding unless an authorised team arrangement is confirmed by the organisers.

## Portfolio objectives

- Develop repeatable incident investigation and evidence-correlation workflows.
- Practise hypothesis-driven analysis and timeline reconstruction.
- Explain security findings clearly, including uncertainty and alternative explanations.
- Connect observable attacker behaviour to appropriate detection and defensive recommendations.
- Document methods, limitations, lessons learned, and personal contributions accurately.

## Investigation workflow

1. **Define the scope:** Read scenario instructions, identify relevant time windows, systems and permitted data sources.
2. **Collect and preserve evidence:** Record relevant event IDs, timestamps (including timezone), source locations and query references; do not publish secrets or raw sensitive data.
3. **Establish a baseline:** Identify expected administration, user actions and scheduled maintenance.
4. **Form and test hypotheses:** Search for corroboration and possible contradictory signals across multiple telemetry sources.
5. **Reconstruct the timeline:** Document events in chronological order, distinguish observed facts from inference, and track confidence.
6. **Assess impact:** Identify affected identities, hosts, cloud resources, data and possible incident boundaries, where evidence allows.
7. **Recommend detections and controls:** Translate validated findings into actionable defensive improvements.
8. **Review before disclosure:** Verify claims, redact sensitive material and check organiser publication permissions.

## Investigation index

| Investigation | Focus | Status | Report |
|---|---|---|---|
| Incident 01 | Initial access / marketing-click lead (scenario premise) | Not started | [Report template](incidents/incident-01.md) |
| Incident 02 | Trusted developer-tool activity (scenario premise) | Not started | [Report template](incidents/incident-02.md) |
| Incident 03 | Account / identity activity (scenario premise) | Not started | [Report template](incidents/incident-03.md) |

*The descriptions above are scenario premises from the event overview, not findings. Final challenge names, mappings and outcomes must be verified during the event.*

## Technical areas to practise

**Security operations:** alert investigation, event triage, telemetry correlation, detection validation  
**Digital forensics:** timeline reconstruction, evidence integrity, competing hypotheses  
**Identity and cloud security:** authentication events, privilege use, cloud activity  
**Incident response:** root-cause assessment, impact analysis, remediation proposals  
**Communication:** concise executive summaries and reproducible technical reporting

**Environment:** Google Security Operations is identified in the official community event description. Specific queries and capabilities will be documented only when actually used.

## Results and outcomes

| Metric | Result |
|---|---|
| Challenges solved | To be updated after the competition |
| Points earned | To be updated after the competition |
| Placement | To be updated after the competition, if available |
| Tools used | To be recorded accurately during the event |
| Key lessons | To be added after investigation |

No claims of completion, ranking, or successful exploitation are made before the event.

## Publication and ethical boundaries

- Perform investigation only in the explicitly authorised competition environment.
- Do not publish active flags, spoilers, private challenge data or operational credentials.
- Keep personal notes and evidence private during the live event.
- Publish solution details **only after the competition** and **only if the organisers permit disclosure**.
- Redact tokens, credentials, personal data and any information whose publication is restricted.
- Respect all competition rules, including participant limits and permitted assistance.
- Do not imply endorsement or affiliation with prospective employers or event partners.

## Professional development

I am a Year 2 Higher Nitec student in Cyber & Network Security at ITE College West, building practical foundations in cybersecurity investigation and ethical security testing. I use structured reports to show how I reason from evidence, validate hypotheses, communicate uncertainty, and identify defensible improvements.

## References

1. [Hack The Box — Operation Cymbal: Cold Room event](https://ctf.hackthebox.com/event/details/operation-cymbal-cold-room-3631)
2. [Google Cloud Security Community — CTF event announcement](https://security.googlecloudcommunity.com/events/community-capture-the-flag-with-hack-the-box-operation-cymbal-cold-room-141)

---

*Prepared as a pre-event portfolio framework on 28 October 2026. Future investigation sections must be updated with firsthand, verified observations.*
