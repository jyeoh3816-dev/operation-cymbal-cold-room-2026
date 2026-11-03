# Deceptive Click — Cybersecurity Investigation Case Study

**Operation Cymbal: Cold Room CTF 2026 | Zero Day Legend**

> **Result:** Scenario Pwned — **6/6 flags accepted** on **30 October 2026 at 9:01 PM SGT**.  
> **Disclosure classification:** Public, **non-spoiler professional case study**. This is not a flag-by-flag walkthrough.

## Executive summary

I completed **Deceptive Click**, an evidence-driven security investigation scenario in Operation Cymbal: Cold Room CTF 2026. Working in the competition's authorised Google SecOps environment, I investigated a simulated incident using security case data, endpoint events, web proxy records and authentication telemetry.

The practical challenge was to move from an initial alert to well-supported findings while distinguishing observed activity from assumptions. I verified my submissions against security records and completed all six investigative tasks. This case study records my **approach and learning outcomes** without disclosing the solutions or proprietary challenge data.

## My objectives

- Understand the case scope and select appropriate telemetry sources.
- Practise accurate security-event interpretation across multiple logging technologies.
- Refine SIEM searches and validate important fields with source records.
- Connect relevant observations into a coherent incident assessment.
- Present conclusions clearly and acknowledge the limits of the available evidence.

## Environment and data sources used

| Source | What I practised | Analytical consideration |
|---|---|---|
| **Google SecOps Cases** | Examined case context, alerts and related events | An AI-assisted or rule-based label still requires evidence review |
| **Google SecOps SIEM Search** | Filtered and correlated security telemetry | Date ranges and event schemas affect the quality of results |
| **Windows Sysmon** | Reviewed process-related and network-related events | Source and target process roles must not be confused |
| **Zscaler web proxy records** | Analysed web request context and original logs | Not all useful HTTP details appear as searchable normalised fields |
| **Windows security events** | Examined authentication-related evidence | A ticket request or login event needs situational context |

## Investigation methodology

### 1. Case triage

I began by reading the scenario objective and reviewing the associated security case. Instead of treating the alert title as a complete finding, I considered which underlying event information could validate the case's significance.

### 2. Search scope and time alignment

I aligned the SIEM time range with the event period, then worked from verified identifiers. This reduced unrelated activity and helped clarify which records belonged to the simulated investigation.

### 3. Cross-source correlation

I compared endpoint, network and authentication telemetry. When one log gave only partial context, I considered which authorised source might corroborate or qualify the observation. I did not assume that a suspicious process or network connection alone proved a particular attacker outcome.

### 4. Original record validation

I encountered cases in which a relevant attribute was not obvious in a normalised field view. Examining the underlying event record helped distinguish a missing search result from an actually absent fact. I also learned to verify field roles and event semantics rather than selecting an unrelated numerical identifier.

### 5. Evidence-based submission and review

For each investigative question, I checked that the proposed answer corresponded to an observed value in the authorised evidence. All six submissions were accepted. The exact findings, host identifiers, commands, filenames and flag values remain intentionally unpublished.

## Observed professional competencies

| Competency | Practical reflection |
|---|---|
| Investigation discipline | Progressed from an alert toward relevant corroborating telemetry |
| Query troubleshooting | Revised search strategy when a broad or mismatched event filter produced no results |
| Source validation | Inspected raw logs to confirm field meaning and avoid misreading normalised output |
| Security fundamentals | Applied knowledge of endpoint monitoring, network traffic and Windows authentication |
| Communication | Organised findings into a concise, auditable narrative without overstating conclusions |

## General defensive improvement opportunities

The following recommendations are generalised from the skills practised and **are not claims about actual deficiencies in the fictional environment**.

1. **Improve visibility:** Maintain reliable endpoint process, network and authentication logs with synchronised timestamps.
2. **Prioritise correlation:** Make it easier to pivot between endpoint activity, network traffic and authentication events.
3. **Preserve original context:** Keep raw records available when normalised parsing leaves gaps.
4. **Increase detection confidence:** Require corroboration before labelling a case as confirmed malicious activity.
5. **Strengthen reporting:** Clearly separate observed facts, analytical hypotheses and impact claims.

## Learning reflection

The most valuable part of this exercise was learning to be precise. A query returning no results does not automatically refute a hypothesis; it may indicate the wrong field, scope or event classification. Conversely, one apparently suspicious log entry does not automatically establish compromise. Effective investigation involves testing the available evidence, understanding the limits of each source and communicating the result responsibly.

Completing Deceptive Click has strengthened my foundation in security operations and digital forensics, which complements my longer-term interest in ethical penetration testing.

## Outcome and limitations

- **Verified achievement:** Deceptive Click completed, **6/6 flags accepted**.
- **Verified completion time:** 30 October 2026 at 9:01 PM SGT, according to the competition dashboard.
- **Not claimed:** Overall leaderboard placement, final cumulative points, professional certification or completion of the other two scenarios.
- **Disclosure limitation:** No answers, challenge-specific indicators, original logs, screenshots containing restricted data or detailed reconstruction instructions are included in this public document.

## Acknowledgement and responsible sharing

I completed this exercise as an individual competitor using **Zero Day Legend** as my portfolio identity. I used AI-based educational guidance during the investigation for terminology, query planning and report structure; I inspected the source records and submitted the accepted answers using my account. I thank the **Google Cloud Security Community** and **Hack The Box** for providing the learning opportunity.

**Feedback welcome:** I would value comments from lecturers, fellow students and cybersecurity professionals on ways to improve my investigative reasoning, technical writing and next learning priorities. Please do not post restricted challenge solutions in public discussions.

[Back to repository overview](../README.md) · [Publication checklist](../POST_EVENT_CHECKLIST.md)
