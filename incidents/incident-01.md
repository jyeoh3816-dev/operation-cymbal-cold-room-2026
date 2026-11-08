# Deceptive Click — Cybersecurity Investigation Case Study

**Operation Cymbal: Cold Room CTF 2026 | Zero Day Legend**  
**Author:** Jerry | Higher Nitec in Cyber & Network Security, ITE College West  
**Focus:** Security operations · Threat investigation · Digital forensics · Evidence validation

> **Verified scenario result:** **Scenario Pwned — 6/6 flags accepted**, 30 October 2026, 9:01 PM SGT.  
> **Overall competition result:** **736th out of 1,716 teams**, **675 points**, **6/18 challenges solved**, as recorded on my Hack The Box Certificate of Participation.  
> **Disclosure:** This is a **public, non-spoiler case study**, not a solution walkthrough. It omits challenge answers, infrastructure identifiers, exact queries, raw logs and restricted materials.

## 1. Executive summary

I completed **Deceptive Click**, an evidence-driven incident investigation scenario in **Operation Cymbal: Cold Room CTF 2026**, organised by the **Google Cloud Security Community** in partnership with **Hack The Box**. Working within the authorised **Google Security Operations (Google SecOps)** environment, I reviewed case alerts and correlated endpoint, web proxy and Windows authentication telemetry to answer six investigative questions.

The central skill I practised was moving from an alert or initial observation to a **defensible conclusion**. I checked event context, adjusted search filters when results were incomplete, compared normalised fields with original records, and differentiated what a log directly demonstrated from what still required corroboration.

**Outcome:** All six Deceptive Click flags were accepted. This reflects success in a **simulated educational challenge**, not a claim of professional incident-response employment, live-system compromise assessment or independently validated remediation.

## 2. Investigation objectives and scope

My objectives were to:

1. Establish the relevant case, time window and available evidence sources.
2. Identify useful signals from endpoint, web proxy, network and identity telemetry.
3. Test search assumptions and avoid interpreting zero matches as proof that an event did not occur.
4. Validate important attributes against source records before recording findings.
5. Communicate the investigation approach, uncertainties and learning outcomes responsibly.

**Scope:** The fictional Cymbal Investments environment and evidence sources supplied for the authorised competition. This report does not present analysis of systems outside that environment.

## 3. Tools and evidence sources

| Technology / source | How I used it | Key analytical consideration |
|---|---|---|
| **Google SecOps — Cases (SOAR)** | Reviewed case context, alert descriptions and associated evidence | Alert severity or AI-assisted assessment is not a substitute for reviewing underlying logs |
| **Google SecOps — SIEM Search** | Searched and filtered records by event period and verified context | Query scope, field choice and event taxonomy affect what is returned |
| **Windows Sysmon** | Analysed process-related and network-related records | Source and destination roles, process relationships and event semantics require care |
| **Zscaler web proxy telemetry** | Reviewed HTTP activity and original proxy records | A request destination and its referring page are different attributes |
| **Windows security logs** | Reviewed authentication and service-related security events | A recorded request or logon alone does not establish the full attacker outcome |

All entries above describe **hands-on exposure during this scenario**, not expert-level proficiency or certifications.

## 4. Investigation methodology

### Phase 1 — Initial alert triage

I began from the competition's security case, read its description and investigated the associated events. I treated the alert as a **lead to validate**, rather than automatically accepting every suggested assessment as a proven fact.

### Phase 2 — Establish a reliable search scope

I aligned the SIEM search period with the event timestamps and used corroborated identifiers to narrow the dataset. This helped separate potentially relevant activity from unrelated background events.

### Phase 3 — Correlate multiple telemetry sources

I compared information across the case queue, endpoint telemetry, web requests and authentication records. Where two sources referred to similar activity, I examined whether they described the same system, user or time period before connecting them analytically.

### Phase 4 — Validate normalised data against original records

Some details were not immediately available through the searchable, normalised event fields. I examined original event records when necessary to verify the meaning of attributes and avoid confusing a related process, host or numeric identifier with the one actually requested.

### Phase 5 — Answer with evidence, then review

For each question, I checked that the response was supported by the relevant source record before submitting it. The challenge dashboard subsequently confirmed **6/6 accepted flags**. Exact submission values and challenge-specific technical evidence are not included here.

## 5. An example of my analytical reasoning (sanitised)

One of the most useful lessons came from a search that initially returned **no matching events**. Rather than treating that as proof that the suspected activity had not occurred, I reconsidered the search's event classification and inspected the available source telemetry. A revised search located a relevant record, which I then checked against its original log format before drawing a conclusion.

| Stage | Decision or observation | Why it mattered |
|---|---|---|
| **Initial search** | An apparently relevant filter produced zero matches | No results may reflect a query limitation rather than absent activity |
| **Reassessment** | I checked the source product and how its event types appeared in Google SecOps | Different logging and normalisation schemes may describe similar activity differently |
| **Validation** | I examined the original record and verified the roles of the involved entities | Prevented me from selecting a related but incorrect field or identifier |
| **Conclusion** | I recorded only what the event directly supported | Kept the investigation evidence-based rather than assumption-driven |

This example is intentionally generalised to **demonstrate reasoning without revealing a challenge solution**.

## 6. Evidence-quality principles applied

| Evidence question | How I assessed it | Reporting principle |
|---|---|---|
| **Is the alert significant?** | Reviewed case context and underlying security telemetry | A detection is a hypothesis to investigate |
| **Does the event involve the relevant system?** | Checked system and account context alongside event time | Correlation requires matching identities and timelines |
| **Is a network event conclusive?** | Considered source, destination and event meaning | A connection does not alone prove successful access or compromise |
| **Is an identity event conclusive?** | Considered the authentication record in its operational context | An observed request is not equivalent to proving every subsequent action |
| **Can the original record clarify an ambiguous field?** | Compared parsed and source views where relevant | Original evidence can resolve normalisation gaps |

**Limitation:** This public document is not a complete incident timeline or forensic evidence package. The exact chronology, identifiers, logs and answer-level proof remain excluded for disclosure reasons.

## 7. Skills demonstrated and development areas

**Skills practised:** case-based triage, SIEM time-window selection, structured event searches, raw-log interpretation, endpoint/network/identity correlation, evidence verification, documentation and clear communication of uncertainty.

**Areas I plan to strengthen:** Windows event internals, Kerberos and Active Directory fundamentals, process trees and endpoint forensics, detection-engineering basics, incident timeline visualisation and writing more concise evidence-to-conclusion summaries.

I am especially interested in developing these foundations further for **security operations, digital forensics and ethical penetration testing** roles.

## 8. Defensive improvement opportunities

These are **general educational recommendations**, not confirmed weaknesses in the simulated organisation.

| Improvement | Defensive value |
|---|---|
| Maintain consistent endpoint, network and authentication logging | Improves investigation visibility and timeline correlation |
| Retain original event records alongside normalised SIEM data | Enables analysts to confirm attributes when mappings are incomplete |
| Correlate activity across endpoints and identities | Reduces the risk of interpreting isolated events out of context |
| Review detection confidence with supporting evidence | Helps prevent overstatement of suspicious or malicious activity |
| Use a consistent investigation-reporting format | Improves handovers, technical review and auditability |

## 9. Verified results and reporting limitations

| Metric | Verified outcome |
|---|---|
| **Deceptive Click** | **Scenario Pwned — 6/6 flags accepted** |
| **Scenario completion** | **30 October 2026, 9:01 PM SGT** |
| **Overall competition ranking** | **736th of 1,716 teams** |
| **Competition score** | **675 points** |
| **Challenges solved across the event** | **6/18** |
| **Verification sources** | Hack The Box challenge dashboard and Certificate of Participation |

**Important distinction:** The six accepted flags represent completion of **Deceptive Click**. The 6/18 figure represents my **overall competition challenge count**; I do not claim completion of other scenarios or an award placement.

This report does not publish flag answers, exact searches, command lines, identifiers, screenshots containing restricted material, original proprietary logs or full incident reconstruction steps. It also does not claim that I performed live remediation or proved a real-world incident's full business impact.

## 10. Reflection and invitation for feedback

This exercise reinforced three principles for me: **verify before concluding**, **correlate before attributing**, and **state uncertainty clearly**. I learned that a useful security investigation is not just about finding an answer; it is about understanding which evidence supports it and recognising the limits of that evidence.

I welcome constructive feedback from lecturers, fellow students, security analysts, incident responders and cybersecurity recruiters, particularly on:

- How can I make the reasoning in this non-spoiler case study clearer and more concise?
- Which technical foundations would make me better prepared for an entry-level cybersecurity internship?
- What is the most useful next step in improving my incident-reporting skills?

Feedback is welcome via the LinkedIn post linking to this portfolio or an appropriate GitHub discussion. **Please avoid posting restricted challenge solutions or private evidence in public comments.**

## 11. Authorship, assistance and responsible disclosure

I participated individually under the **Zero Day Legend** portfolio identity. I used **AI-based educational guidance** for concepts, search planning and document structure, while inspecting source records and submitting my competition answers through my own account. This distinction is included for transparency.

I appreciate the opportunity provided by the **Google Cloud Security Community** and **Hack The Box**. This independent student report does not imply affiliation with or endorsement by the organisers, **ITE College West**, **CSA**, **GovTech**, **NCS** or other prospective employers. Publication of any future technical walkthrough is subject to applicable organiser and Hack The Box rules.

---

[Back to competition portfolio](../README.md) · [Publication checklist](../POST_EVENT_CHECKLIST.md) · [Official CTF event](https://ctf.hackthebox.com/event/details/operation-cymbal-cold-room-3631)

*Last updated: 8 November 2026. Public non-spoiler edition.*
