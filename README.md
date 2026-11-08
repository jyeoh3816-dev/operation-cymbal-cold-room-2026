# Operation Cymbal: Cold Room CTF 2026

**Cybersecurity Investigation Portfolio | Zero Day Legend**  
*Google Security Operations (Google SecOps) · Incident Investigation · Threat Hunting · Digital Forensics*

> **Verified results:** **736th of 1,716 teams** · **675 points** · **6/18 challenges solved**. These figures are taken from the Hack The Box Certificate of Participation for **Zero Day Legend**. My completed scenario, **Deceptive Click**, was marked **Scenario Pwned (6/6 flags)** on 30 October 2026 at 9:01 PM SGT.
>
> This is a professional, **non-spoiler portfolio**, not a published solution guide. Challenge flags, restricted event data and detailed solutions are omitted pending applicable organiser permission.

## Competition overview

| Detail | Information |
|---|---|
| **Competition** | Operation Cymbal: Cold Room CTF 2026 |
| **Organised by** | Google Cloud Security Community in partnership with Hack The Box |
| **Format** | Online, evidence-driven cybersecurity investigation |
| **Event period (Singapore time)** | 30 October–2 November 2026 |
| **Dates printed on participation certificate** | 29 October–1 November 2026 |
| **Participant** | Jerry · Higher Nitec in Cyber & Network Security, ITE College West |
| **Team / portfolio identity** | Zero Day Legend (individual participation) |
| **Main platform** | Google Security Operations (Google SecOps) |
| **Overall team ranking** | **736th out of 1,716 teams** |
| **Total points** | **675** |
| **Challenges solved** | **6/18** |
| **Verified completed scenario** | **Deceptive Click — 6/6 flags** |

**Results verification:** The competition ranking, points, solved challenge count, team name and certificate dates are taken directly from my Hack The Box **Certificate of Participation**. The event period above is stated in Singapore time; the certificate uses its own displayed date range. No award, podium finish or distinction is claimed.

## About this portfolio

I am a Year 2 student in the three-year Higher Nitec in Cyber & Network Security programme at **ITE College West, Singapore**, building a technical foundation in security operations, digital forensics, incident response and ethical penetration testing.

I joined this CTF to practise moving from alerts to defensible conclusions: selecting relevant evidence, correlating events, testing assumptions and explaining findings clearly. The fictional enterprise setting provided opportunities to analyse endpoint, network and authentication telemetry in an authorised investigation environment.

This repository is intended for my lecturers, cybersecurity practitioners, internship interviewers and professional connections. It documents my **completed Deceptive Click case study**, investigative reasoning and learning outcomes while respecting platform and organiser publication restrictions.

## Featured completed investigation

| Incident | Verified achievement | Report |
|---|---|---|
| **Incident 01 — Deceptive Click** | **Scenario Pwned — 6/6 flags accepted** | **[Read the professional case study](incidents/incident-01.md)** |

This public repository intentionally features **one completed, evidence-based investigation**. Unfinished challenge templates have been removed so reviewers can focus on documented work.

**Completion evidence:** My Hack The Box dashboard displayed *Scenario Pwned* for Deceptive Click on **30 October 2026 at 21:01 SGT**. The participation certificate confirms a final **overall team ranking of 736th out of 1,716 teams, 675 points and 6/18 challenges solved**. The overall challenge count is presented transparently; the case study covers **Deceptive Click only**.

## Deceptive Click — professional case study

**Outcome:** Completed six investigative tasks through the competition's authorised Google SecOps environment.

The scenario involved assessing security case context and correlating endpoint telemetry, web proxy activity and identity-related events. I refined searches to the relevant event period, checked system and user context, compared structured fields with source logs when needed, and verified evidence before submitting responses.

The public case study intentionally excludes exact challenge answers, flags, sensitive infrastructure indicators, commands, screenshots of restricted evidence and proprietary threat-intelligence materials.

**[Read the Deceptive Click case study](incidents/incident-01.md)**

## Tools and technical competencies practised

| Area | Practical experience |
|---|---|
| **Security operations** | Google SecOps Cases and SIEM Search, alert context and event triage |
| **Endpoint monitoring** | Windows Sysmon process and network-event interpretation |
| **Network investigation** | Network-connection and Zscaler web proxy log review |
| **Identity investigation** | Windows authentication and Kerberos-related event analysis |
| **Log validation** | Cross-checking normalised fields and original event records |
| **Analytical reasoning** | Refining search logic, checking time windows, and distinguishing observation from inference |
| **Technical communication** | Evidence-based summaries, limitations, professional reporting and clear recommendations |

These describe skills practised during an authorised learning exercise, not professional employment experience or an externally awarded technical certification.

## Investigation methodology

1. **Define the investigative question.** Identify permitted data sources, relevant systems and the decision to be supported.
2. **Establish the time window.** Align search filters with actual incident timestamps, not the current date.
3. **Pivot from verified facts.** Use confirmed system, event and account context to narrow searches.
4. **Correlate evidence.** Compare endpoint, network and identity records for supporting or contradictory observations.
5. **Inspect source logs.** Validate relevant details when normalised event fields appear incomplete or ambiguous.
6. **Separate facts from hypotheses.** Explain which conclusions are evidenced and which need corroboration.
7. **Report responsibly.** Document technical learning without publishing prohibited CTF solutions or restricted content.

## Key lessons learned

- **An alert is a starting point, not a final conclusion.** Detection requires context and independent verification.
- **Precision improves investigations.** Correct host identifiers, event taxonomy and time-range selection matter.
- **Raw evidence can resolve uncertainty.** Original logs may provide detail missing from a normalised record.
- **Correlation matters.** One process, network event or login seldom proves an entire incident narrative.
- **Communication is a security skill.** A useful investigation report explains what happened, what is known and what remains uncertain.

## General defensive recommendations

These are educational observations, not claims that particular controls were absent from the scenario environment:

- Retain reliable endpoint process and network telemetry with consistent timestamps.
- Correlate identity and network activity across hosts when examining potential lateral movement.
- Preserve access to original log records alongside normalised fields for analyst validation.
- Review alert accuracy and distinguish verified findings from speculative indicators.
- Develop concise investigation summaries that clearly document confidence and limitations.

## Feedback and professional discussion

I welcome **constructive feedback** from lecturers, cybersecurity practitioners, interviewers, recruiters and fellow learners. In particular, I would appreciate suggestions on making technical investigations easier to reproduce and evaluate, choosing relevant digital forensics topics to study next, and demonstrating the skills expected of an entry-level cybersecurity candidate.

Feel free to comment on the LinkedIn post linking to this repository, or start a GitHub discussion/issue if that feature is available. **Please do not share CTF flags, unpublished solutions, restricted logs or access details in public comments.**

## Responsible disclosure and attribution

- All investigative activity was performed within the authorised competition environment.
- Zero Day Legend is my team/portfolio identity for this individual event entry.
- I used AI-based educational guidance to understand log terminology, refine investigation approaches and structure documentation. I reviewed the available records and submitted responses through my own competition account.
- No challenge-specific solutions, active flags, restricted raw logs, credentials or proprietary threat-intelligence reports are reproduced here.
- Detailed technical walkthroughs will be considered only when applicable Hack The Box retirement rules and organiser publication permissions permit them.
- This independent student portfolio does not imply endorsement or affiliation with Google, Hack The Box, ITE, CSA, GovTech, NCS or other employers.

See the [post-event publication checklist](POST_EVENT_CHECKLIST.md) before publishing more evidence or screenshots.

## Official references

- [Hack The Box — Operation Cymbal: Cold Room CTF](https://ctf.hackthebox.com/event/details/operation-cymbal-cold-room-3631)
- [Google Cloud Security Community — Event announcement](https://security.googlecloudcommunity.com/events/community-capture-the-flag-with-hack-the-box-operation-cymbal-cold-room-141)
- [Hack The Box — Streaming, Writeups and Walkthrough Guidelines](https://help.hackthebox.com/en/articles/5188925-streaming-writeups-walkthrough-guidelines)

---

*Last updated: 8 November 2026. Overall ranking and score are verified against the participation certificate; technical material is intentionally non-spoiler.*
# Operation Cymbal: Cold Room CTF 2026

**Cybersecurity Investigation Portfolio | Zero Day Legend**  
*Google Security Operations (Google SecOps) · Incident Investigation · Threat Hunting · Digital Forensics*

> **Verified results:** **736th of 1,716 teams** · **675 points** · **6/18 challenges solved**. These figures are taken from the Hack The Box Certificate of Participation for **Zero Day Legend**. My completed scenario, **Deceptive Click**, was marked **Scenario Pwned (6/6 flags)** on 30 October 2026 at 9:01 PM SGT.
>
> This is a professional, **non-spoiler portfolio**, not a published solution guide. Challenge flags, restricted event data and detailed solutions are omitted pending applicable organiser permission.

