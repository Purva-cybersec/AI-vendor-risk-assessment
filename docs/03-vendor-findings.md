# Vendor Findings

Each question was rated on two separate scales:
- **Status** (transparency): Documented / Partial / Not documented
- **Assessment** (risk): Favorable / Neutral / Unfavorable / Unknown

A clearly documented practice can still be unfavorable. Full evidence for all 28 questions is in the workbook.

| | Gong | Otter.ai |
|---|---|---|
| Documented | 6 | 5 |
| Partial | 14 | 11 |
| Not documented | 8 | 12 |
| Favorable | 10 | 5 |
| Unfavorable | 1 | 6 |

Evidence was weighted by strength: contract > independent audit or certification > help documentation > marketing pages.

## Gong

**1. The no-training commitment covers generative models only.** Gong states customer data is never used to train generative models. Gong also uses other forms of AI, so the commitment's coverage of non-generative models needs confirming, and the wording needs to move from a marketing page into the contract.

**2. AI processing location.** Gong's subprocessors operate in the USA and EU, but application AI services may use global endpoints. For EU customers' calls, the processing location needs confirming.

**3. Broad calendar permissions.** The Google Calendar add-on requests access to view events on all calendars and to run when the user is not present.

**4. Strong consent tooling that depends on the customer.** Consent pages, automated recording notifications, and the option to join without recording are available, but LedgerLoop must configure and enforce them, similar to a complementary user entity control in a SOC 2 report. Gong's 30-day post-termination deletion aligns with LedgerLoop's own 30-day deletion commitment to its customers.

**5. Adverse media.** A 2023 federal docket, Cervantes v. Gong.io Ltd., does not state its claims in the public listing; this is a follow-up item, not a finding. A patent suit filed *by* Gong against a competitor is not a customer risk.

Many "Not documented" items relate to documents in Gong's trust center that require access, which would be requested under NDA in a live review.

## Otter.ai

**1. Training on confidential business content.** Otter trains its own models on user data after proprietary de-identification. De-identification removes who spoke, but a sales call's content — deal sizes, pricing, customer financial details — remains. For confidential business conversations, the content is the sensitive part.

**2. A statement needing clarification.** Otter states training is automatic and recordings are not manually reviewed. Its subprocessor list includes a provider that annotates training and evaluation data. These may not conflict, but the data that provider receives should be confirmed.

**3. Strong fourth-party transparency.** Otter names its AI providers, states each one's role, and states they neither train on nor store customer data sent through the API. On this point Otter is more transparent than Gong.

**4. Consent placed on the customer, with active litigation.** Otter's privacy page requires users to obtain consent and indicate recording. In re Otter.AI Privacy Litigation (N.D. Cal., No. 5:25-cv-06911) consolidates class actions alleging recording, voiceprint creation, and model training without participants' consent. Secondary sources report that an August 2026 order allowed core claims to proceed. These are allegations, and Otter denies unlawful interception. Because consent responsibility sits with customers, LedgerLoop could share exposure if it used the tool without its own consent process.

**5. "Based on" is not "certified."** Otter's security policies are described as based on the ISO 27001/2 framework, which is not an independent certification. No AI management system certification is documented.

**6. No EU region documented.** Listed subprocessors are US-based.
