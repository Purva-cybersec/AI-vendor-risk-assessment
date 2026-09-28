# Recommendation

| Vendor | Decision | Summary |
|---|---|---|
| Gong | **Approve with conditions** | Certified AI management system, public no-training commitment for generative models, and strong consent tooling. Residual risks are addressable through contract and configuration. |
| Otter.ai | **Escalate** | Training on customer content, consent responsibility placed on customers during active consent litigation, and no documented AI governance certification exceed what should be accepted at the analyst level. |

**Escalate** does not mean reject. It means the residual risk requires a decision by security leadership and Legal rather than the analyst.

## Conditions for Gong

1. Contract states customer data will not be used to train any models, generative or otherwise.
2. Gong confirms where AI processing occurs for EU customers' calls.
3. Calendar permissions are narrowed to the minimum required.
4. LedgerLoop enforces consent pages for all external calls.
5. Retention is set to the shortest period the business needs, below the three-year default.
6. Call owners review AI summaries before sending them to customers or logging them in the CRM.
7. LedgerLoop reviews Gong's SOC 2 Type II report for exceptions and AI-feature scope.

## What could change the Otter.ai decision

- An enterprise agreement that disables training on customer content, committed in the contract
- Clarification of the annotation subprocessor's access to customer data
- Admin controls that let LedgerLoop enforce all-party consent
- EU data residency, or Legal sign-off on transfers

## Follow-up questions

**Gong:** non-generative model training; EU AI processing location; narrower calendar permissions; SOC 2 exceptions and scope; claims and outcome of the 2023 case.

**Otter.ai:** enterprise training opt-out in contract; annotation provider's data access; consent enforcement controls and voiceprints; EU residency; plans for ISO/IEC 42001 or ISO 27001 certification.

## Ongoing monitoring

Annual reassessment, periodic adverse media screening, and immediate reassessment on any trigger in the [inherent risk memo](01-inherent-risk-memo.md).
