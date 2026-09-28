# AI Vendor Risk Assessment : AI Meeting Assistants

A third-party risk assessment of two AI meeting assistants, **Gong** and **Otter.ai**, for a fictional company, LedgerLoop, whose sales team wants to record and summarize customer calls. The project follows the TPRM workflow: intake, inherent risk tiering, an AI-specific due diligence questionnaire, vendor research, and a recommendation with conditions.

## Why I built this

My current work involves third-party due diligence and customer security audits. As AI tools spread through every business function, vendor reviews increasingly need to answer AI-specific questions: is our data used to train models, which AI providers receive it, and who is accountable when the AI changes. I built this to practice third-party AI risk assessment end to end.

## At a glance

| | |
|---|---|
| **Requesting company** | LedgerLoop, Inc. (fictional B2B SaaS) |
| **Use case** | Record, transcribe, and summarize external customer calls; sync notes to CRM |
| **Inherent risk tier** | Tier 1 (High) — driven by confidential customer data, broad system access, regulatory exposure, and fourth-party AI processing |
| **Method** | 28-question AI due diligence questionnaire answered from public vendor documentation |
| **Frameworks drawn on** | ISO/IEC 42001, NIST AI RMF, EU AI Act |

## Results

| | Gong | Otter.ai |
|---|---|---|
| Documented / Partial / Not documented | 6 / 14 / 8 | 5 / 11 / 12 |
| Favorable / Unfavorable findings | 10 / 1 | 5 / 6 |
| ISO/IEC 42001 | Certified | Not documented |
| Trains on customer content | States no training of generative models | Trains own models on de-identified data |
| Recording consent | Consent pages and notifications available | Responsibility placed on users; active class action |
| **Recommendation** | **Approve with conditions** | **Escalate** |

Key findings include the scope of a "generative models only" no-training commitment, de-identified training on confidential business conversations, stronger fourth-party AI transparency from the otherwise weaker vendor, and consent obligations that shift liability to the customer. Details in [docs/03-vendor-findings.md](docs/03-vendor-findings.md).

## Repository contents

```
├── README.md
├── docs/
│   ├── 01-inherent-risk-memo.md   Use case, six risk factors, tier, reassessment triggers
│   ├── 02-questionnaire.md        28 AI due diligence questions mapped to risk factors
│   ├── 03-vendor-findings.md      Key findings for each vendor
│   └── 04-recommendation.md       Decision, conditions, follow-up questions
└── workpapers/
    └── AI_Vendor_Risk_Assessment.xlsx
```

The workbook contains the inherent risk rating, full questionnaire responses for both vendors with evidence, summary counts, follow-up questions, and sources. GitHub can't preview `.xlsx` files — click the file, then **Download**.

## Skills demonstrated

Third-party risk management · inherent and residual risk · AI governance (ISO/IEC 42001, NIST AI RMF, EU AI Act) · fourth-party risk · adverse media screening · due diligence questionnaire design · evidence evaluation · risk-based recommendations

## Disclaimer

LedgerLoop is fictional. Vendor findings are based solely on public documentation reviewed in September 2026; vendors were not contacted, and their practices may have changed since. "Not documented" means not publicly documented, not absent. Litigation described consists of allegations, not findings of wrongdoing. This is a learning project, not legal advice or a formal vendor rating.
