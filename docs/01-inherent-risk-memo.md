# Inherent Risk Assessment — AI Meeting Assistant

**Requesting team:** Sales and Customer Success
**Intended use:** Record, transcribe, and summarize external customer calls; sync meeting notes to the CRM.
**Vendors under consideration:** Gong, Otter.ai
**Assessment basis:** This rating reflects the risk of the intended use, before any vendor-specific review. It applies to whichever vendor is selected.

**Data involved:** Call audio and video, transcripts, and AI-generated summaries, containing customers' confidential financial information and the names, email addresses, and voices of LedgerLoop employees and customer participants.

| Factor | Rating | Rationale |
|---|---|---|
| Data sensitivity | High | Calls contain customer financial information classified as confidential, plus personal data including participants' names and voices. |
| Access and integration | High | The tool reads employee calendars, including attendee details and meeting titles, joins meetings automatically, and may sync notes to the CRM. |
| Business criticality | Low | If the tool is unavailable, Sales and Customer Success can continue customer calls and take notes manually, so an outage causes inconvenience rather than business disruption. The tool supports core processes but does not run them. |
| Regulatory exposure | High | Recording requires consent from all participants in several US states, voice data may fall under biometric privacy law, and EU participants' data is subject to GDPR, including cross-border transfer rules. Provisional rating, to be confirmed by Legal. |
| AI decision impact | Medium | Summaries may inform customer follow-ups and CRM records, so errors could misstate customer commitments. However, a LedgerLoop employee attends every call and can correct errors, and the tool makes no decisions about individuals. |
| Fourth-party reliance | High | The vendor may send call content to third-party AI model providers with which LedgerLoop has no contract. LedgerLoop's protection depends entirely on the vendor's agreements with those providers. |

## Inherent risk tier: Tier 1 (High)

The tier is driven by the highest-risk factors, not an average. Confidential customer data, broad system access, regulatory exposure, and fourth-party AI processing each independently warrant Tier 1.

## Required due diligence for Tier 1

- Full AI vendor due diligence questionnaire
- Review of the SOC 2 Type II report and ISO certifications, including ISO/IEC 42001 where held
- Identification of fourth-party AI model providers and their data retention and training terms
- Adverse media screening
- Legal and privacy review of recording consent and cross-border data transfers
- Contract terms: no training on customer data, deletion on termination, advance notice of new subprocessors
- Annual reassessment

**Reduced scope:** Given Low business criticality, a detailed review of the vendor's business continuity and disaster recovery plans is not required.

**Reassessment triggers:** Use of the tool expands beyond Sales and Customer Success; recordings or summaries become the official record of customer commitments; or the vendor changes its AI model providers.
