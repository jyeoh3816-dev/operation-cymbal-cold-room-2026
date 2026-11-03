Operation Cymbal: Cold Room CTF 2026
Cybersecurity Investigation Portfolio | Zero Day Legend
Google Security Operations (Google SecOps) • Incident Investigation • Threat Hunting • Digital Forensics

Verified milestone: Deceptive Click: Scenario Pwned (6/6 flags) on 30 October 2026 at 9:01 PM SGT. This repository is a professional, non-spoiler reflection on my authorised CTF participation, not a public solution guide.

At a glance
Detail	Information
Competition	Operation Cymbal: Cold Room CTF 2026
Organised by	Google Cloud Security Community in partnership with Hack The Box
Event period	30 October–2 November 2026 (Singapore time)
Format	Online, evidence-driven incident investigation
Participant	Jerry: Higher Nitec in Cyber & Network Security, ITE College West
Participation model	Individual entrant; Zero Day Legend is my portfolio identity
Main investigation platform	Google Security Operations (Google SecOps)
Verified completion	Deceptive Click: 6/6 flags accepted
Overall competition ranking	Not verified; no ranking claimed


About this portfolio
I am a Year 2 student in the three-year Higher Nitec in Cyber & Network Security programme at ITE College West, Singapore. I am building my technical foundation in cybersecurity, with a long-term interest in ethical penetration testing and security investigation.

I participated in this event to practise investigating security alerts and reconstructing incidents through evidence, rather than relying solely on a detection label or a single log entry. The scenario takes place in a fictional enterprise environment, where investigative conclusions must be supported by telemetry and sound reasoning.

This repository is intended for lecturers, cybersecurity practitioners, hiring teams, and my professional network. It showcases what I learned, how I approached analysis, and how I communicate findings while respecting the organisers' content restrictions.

Verified challenge progress
Scenario	Verified status	Public writeup
Deceptive Click	Completed — 6/6 flags; Scenario Pwned	[Non-spoiler case study](incidents/incident-01.md)
Rogue Synthesis	Outcome not documented here	[Reporting framework](incidents/incident-02.md)
OAuth Heist	Outcome not documented here	[Reporting framework](incidents/incident-03.md)


Completion evidence: My Hack The Box dashboard showed Scenario Pwned on 30 October 2026, 21:01 SGT, with all six flags accepted for Deceptive Click. I have not independently verified a final event score or overall placement and therefore do not claim either.

Deceptive Click — professional case study
Outcome: Completed the scenario's six investigative tasks using the competition's authorised environment.

The exercise involved correlating security case information, endpoint telemetry, web proxy records and identity-related events. I worked through investigation questions by narrowing the relevant time window, validating host context, examining raw records when parsed fields were incomplete, and confirming the requested evidence before making submissions.

This public account deliberately excludes flag answers, challenge-specific indicators and commands, sensitive event content and any restricted GTI documents.

[**Read the Deceptive Click case study**](incidents/incident-01.md)
Tools and skills practised
Area	Experience demonstrated
Security Operations	Navigated Google SecOps Cases and SIEM Search; reviewed case context and security alerts
Log analysis	Compared normalised event fields with source records; verified timestamps and event context
Endpoint investigation	Interpreted Windows Sysmon process and network telemetry
Network investigation	Examined network connection and Zscaler web proxy records
Identity investigation	Reviewed Windows authentication and Kerberos-related log evidence
Analytical reasoning	Tested hypotheses, refined queries when searches returned no matches, and avoided assumptions
Technical communication	Recorded defensible observations, limitations and improvement opportunities


These items describe practical exposure from one authorised challenge, not a claim of professional certification or independent employment experience.

My investigation workflow
1. Read the case and define the scope. Clarify the question, systems, accounts and permitted evidence sources.
2. Anchor the time window. Align searches with the relevant event period rather than the current date.
3. Pivot from known evidence. Use verified attributes to narrow events instead of guessing outcomes.
4. Compare evidence sources. Correlate endpoint, network and authentication telemetry.
5. Inspect original logs when needed. A missing normalised field does not necessarily mean the underlying event lacks the information.
6. Differentiate fact from inference. Check source-versus-target roles, event context and plausible legitimate activity.
7. Document responsibly. Record learning outcomes and disclosure limitations without publishing prohibited content.

Lessons learned
- Detection is not conclusion. An alert should initiate investigation, not substitute for independent validation.
- Search precision matters. Host identifiers, event taxonomy and time windows can materially change results.
- Evidence quality matters. Parsed fields are helpful, but original logs are sometimes necessary to verify a claim.
- Context matters. A single process, connection or authentication record rarely tells the complete story.
- Reporting matters. Clear explanations and appropriately stated uncertainty are as important as finding an answer.

Recommendations for defensive teams
These are general learning recommendations, not a claim that any specific control was absent in the fictional environment:
- Maintain endpoint process and network telemetry with consistent timestamps.
- Correlate identity and network activity across systems when investigating potential lateral movement.
- Retain accessible raw logs alongside normalised fields for analyst validation.
- Develop detection review processes that separate confirmed events from speculative interpretations.
- Encourage concise incident narratives that make evidence and uncertainty explicit.

Feedback and professional discussion
Constructive feedback is welcome. If you are a lecturer, cybersecurity practitioner, hiring manager, or fellow student, I would value your perspective on:
- How can I improve the clarity and defensibility of my investigation reports?
- Which security operations or digital forensics fundamentals should I prioritise next?
- What would make this portfolio more useful when assessing a junior cybersecurity candidate?

You can comment on the LinkedIn post linking to this repository, or open a GitHub Issue if issues are enabled. Please do not post challenge answers, restricted logs, access details or spoilers in public comments.

Responsible disclosure and attribution
- All investigation activity was within the authorised event environment.
- The competition allowed one participant per registration; Zero Day Legend is used as my personal CTF portfolio identity.
- I used AI-based educational assistance to understand log terminology, think through search approaches and structure my documentation. I reviewed the actual records and submitted the accepted responses through my own competition account.
- No event-specific solutions, flags, private access details, restricted raw logs, or proprietary threat-intelligence reports are reproduced here.
- Detailed challenge solutions will only be considered for publication if the relevant content is officially retired and the applicable organiser permissions allow it.
- This independent student project does not imply affiliation with or endorsement by the event organisers, ITE, CSA, GovTech, NCS or any employer.

See the [publication checklist](POST_EVENT_CHECKLIST.md) before adding any further evidence or screenshots.

Official references
- Hack The Box — Operation Cymbal: Cold Room CTF
- Google Cloud Security Community — Event announcement
- Hack The Box — Streaming, writeups and walkthrough guidelines

Last updated: 3 November 2026. This public portfolio contains only verified participation outcomes and non-spoiler educational reflections.
