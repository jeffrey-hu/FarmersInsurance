# FarmersInsurance Project

This project supports a lawsuit the Lu/Hu family is preparing against Farmers Insurance for their failure to pay for hail damage to the windows of their Minnesota home from the storm on **7/13/2024**. It collects the factual record, policy documents, evidence, legal research, and strategic decisions needed to build and file the case.

## Root Files

- **README.md** — Short repo intro ("FarmersInsurance — Hail Claim vs Farmers Insurance").
- **ClaimTimeline.md** — Master chronological timeline of every legally relevant event from policy inception (10/22/2014) through the latest correspondence; primary reference for sequencing the dispute.
- **DocumentIndex.md** — Catalog of policy details, coverage amounts, and annotated index of every supporting document in the project.
- **KeyDecisions.md** — Running log of strategic decisions (court venue, lawsuit strategy, negotiation choices) with rationale.
- **chatGPTLog.txt** — Raw transcript of prior ChatGPT conversations used as background research; not authoritative.

## Root Folders

- **CaseContext/** — Contains two fact references: (1) `key-facts.md`, an earlier unrefined family account of key events with legal-significance annotations; and (2) `key-facts-excluding-legal-context.md`, a more recent, phase-organized catalog of pro-family facts drawn directly from the source documents with per-fact citations and intentionally no legal framing (facts will be tied to legal arguments separately). Consult both for research, filings, argument evaluation, and strategy; prefer `key-facts-excluding-legal-context.md` when you need the sourced factual record and `key-facts.md` when you need the family's narrative framing.
- **EventDocuments/** — Primary evidence folder: Farmers' denial letters, appraisal documents, family response letters, post-appraisal email chains, the Dept. of Commerce complaint, and the family's raw `Copy of ComunicationLogs.docx.md` communication log.
- **Evidence/** — External/meteorological evidence of the 7/13/2024 storm (e.g., Minnesota wind & hail report PDF).
- **HailShapes/** — Academic papers and analysis on hail shapes/speeds and damage signatures, plus rebuttal material countering Farmers' damage-causation arguments.
- **HomePolicy/** — Original Farmers policy documents: 2014 application and policy notice, and the 2023 renewal.
- **LegalReferences/** — Legal strategy materials: case law research, argument-strength assessment, litigation bridge document, and appraisal-process research.
- **Filings/** — Documents filed with the court or served on Defendant, plus `Document_Formatting_Standard.md`, the formatting rules every such document must follow.

## Document Formatting

- **Before creating or editing any `.docx` that will be filed with the court or served on Defendant, read `Filings/Document_Formatting_Standard.md` and follow it.** It fixes page setup, list indentation (left 0.5", hanging −0.5", 8 pt after), signature blocks, the certificate-of-service form, caption blocks, numbering discipline, and how to keep a document's Markdown twin in sync. The reference document is `Filings/Discovery/discoveryPlanAndInformationalStatement/Plaintiffs_Rule_26.06_Discovery_Plan_V5.docx`.
- Two rules from that standard are easy to get wrong and expensive to fix: service goes to **counsel of record** (Kennedy Law Firm, appeared 7/28/2026), not to Defendant or its registered agent; and service by U.S. Mail **adds 3 days** to any response period under Minn. R. Civ. P. 6.01(e).

## Working Notes

- All dates are U.S. format (M/D/YYYY).
- When researching, filing, or evaluating arguments, start with `OffenseStrategies/KeyFacts/key-facts-excluding-legal-context.md` (sourced, phase-organized factual catalog) and cross-reference `CaseContext/key-facts.md`, `ClaimTimeline.md`, and `DocumentIndex.md`.
