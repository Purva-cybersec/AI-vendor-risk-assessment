# AI Vendor Due Diligence Questionnaire

A focused AI supplement to standard security questionnaires (such as SIG or CAIQ). Every question traces to a factor in the [inherent risk memo](01-inherent-risk-memo.md): 1 Data sensitivity · 2 Access and integration · 3 Business criticality · 4 Regulatory exposure · 5 AI decision impact · 6 Fourth-party reliance.

## Design choices
- **Standard controls are left to the SOC 2 report.** General change management, encryption operations, and similar controls are tested in the vendor's SOC 2 report (requested in H1), so the questionnaire focuses on AI-specific gaps.
- **Business continuity is excluded.** Business criticality was rated Low, so a detailed continuity review is not required.
- **Physical data center questions are replaced by D4.** These vendors run on public cloud providers, whose physical controls are covered by those providers' own audit reports.

## A. AI governance

| ID | Question | Factor |
|---|---|---|
| A1 | Do you maintain a documented AI policy or AI management system? Is it certified to ISO/IEC 42001, and what is the certificate's scope? | All |
| A2 | Who is accountable for AI risk (a named role or committee)? | All |
| A3 | Do you perform AI risk or impact assessments before releasing new AI features? | 5 |

## B. Training data use

| ID | Question | Factor |
|---|---|---|
| B1 | Is customer content (audio, transcripts, summaries) used to train or improve any AI models, yours or third parties'? | 1, 6 |
| B2 | If yes: is it opt-in or opt-out, on which plans, and what de-identification is applied? | 1 |
| B3 | Will you commit contractually to not training on customer content? | 1 |

## C. Data handling

| ID | Question | Factor |
|---|---|---|
| C1 | What are the retention periods for recordings, transcripts, and summaries? Can customers configure them? | 1 |
| C2 | How quickly is data deleted on request and at contract termination? Do you provide confirmation of deletion? | 1 |
| C3 | Where is data stored and processed? Is an EU region available? | 1, 4 |
| C4 | Is data encrypted in transit and at rest? | 1 |
| C5 | What is your notification timeframe for incidents affecting customer data, including AI-related incidents? | 1 |

## D. Fourth parties

| ID | Question | Factor |
|---|---|---|
| D1 | Provide your subprocessor list, including all AI model providers. | 6 |
| D2 | What call data is sent to each AI provider? Do those providers retain it or train on it? | 6 |
| D3 | Do you give advance notice of new subprocessors, with a right to object? | 6 |
| D4 | Which cloud providers host customer data? How do you review those providers' security assurance reports? | 6 |

## E. Model reliability and change

| ID | Question | Factor |
|---|---|---|
| E1 | How do you test transcription and summary accuracy? Are known limitations documented? | 5 |
| E2 | Can users review and edit summaries before sharing them? Is AI-generated content labeled? | 5 |
| E3 | How are changes to AI models, including model updates or switching model providers, tested and approved before release? Are customers notified of material changes? | 5, 6 |

## F. Transparency and consent

| ID | Question | Factor |
|---|---|---|
| F1 | How are meeting participants, including external ones, notified that recording is happening? | 4 |
| F2 | Can admins prevent the tool from auto-joining certain meetings, or require host approval? | 2, 4 |
| F3 | Do you collect voiceprints or other biometric identifiers? If so, how is consent obtained? | 4 |

## G. Access and AI security

| ID | Question | Factor |
|---|---|---|
| G1 | What permissions does the tool request for calendars, email, and CRM? Can they be limited? | 2 |
| G2 | Do you support SSO, MFA, and role-based admin controls? | 2 |
| G3 | How is each customer's data kept separate from other customers' data during AI processing? | 1 |
| G4 | What protections exist against AI features leaking content, such as one user's meeting details appearing in another user's AI answers? | 1 |

## H. Assurance and regulatory

| ID | Question | Factor |
|---|---|---|
| H1 | Provide your current SOC 2 Type II report. What period does it cover, does its scope include the AI features, and were there any exceptions? | All |
| H2 | How do you classify your role and your AI system under the EU AI Act? | 4 |
| H3 | Are there pending lawsuits or regulatory actions related to recording, privacy, or AI? | 4 |
