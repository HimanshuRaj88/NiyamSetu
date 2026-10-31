# NiyamSetu
NiyamSetu AI, our Teliport Season 4 (Tata Elxsi) solution for Case Study 4, automates medical device labeling. It finds impacted labels, drafts and validates compliant text with GenAI and vision, and keeps a full audit trail.
# LabelGuard AI

**AI that finds, writes, checks and approves medical device labels automatically.**

Submission for **Tata Elxsi Teliport Season 4**, **Case Study 4: End-to-End Labeling Automation Management for Medical Devices**.

---

## Problem

A single medical device change (for example, a new sterilization method) can require updates to 30+ labels in 20+ languages across multiple markets and packaging levels. Today this is done manually across PLM, ERP, labeling software and spreadsheets, which causes:

- Slow change cycles and delayed product launches
- Missed labels, translation errors and outdated symbols
- Regulatory findings (FDA, EU MDR), recalls and patient-safety risk

## Solution

NiyamSetu is an agentic, self-validating labeling platform. One product change goes in, and compliant, traceable, release-ready labels come out. Humans approve only the exceptions.

### Pipeline

| Step | Stage | What happens |
|---|---|---|
| 1 | **Ingest and Unify** | RPA/API connectors pull PLM, ERP, artwork and UDI data into one Label Knowledge Graph |
| 2 | **Detect and Assess** | Regulatory Intelligence Bot tracks FDA, EU MDR and ISO updates; Change Impact Engine flags affected labels, markets and actions |
| 3 | **Author** | GenAI + RAG drafts compliant text, symbols (ISO 15223-1) and UDI; AI validates translations |
| 4 | **Validate** | Computer vision redlines approved vs revised artwork; rules engine checks UDI, dates, symbols, barcode and layout |
| 5 | **Approve** | Auto change order; risk-tiered routing to Regulatory and Quality with an AI evidence pack |
| 6 | **Release and Learn** | Release to print/MES; predictive analytics learn from every error |

## Key features

- Labels that check themselves before release
- Automatic impact detection across labels, markets and languages
- Regulatory rules library (FDA, EU MDR, ISO, UDI) with source clauses
- Team of specialist AI agents with human-in-the-loop approval
- Computer-vision artwork comparison
- Translation error detection
- Evidence-backed findings linked to a rule
- Full audit trail for every label element
- Plugs into existing PLM, ERP and labeling tools

## Architecture (high level)

- **Data:** knowledge graph and vector store of regulatory texts
- **AI:** LLM + RAG, OCR/layout computer vision, deterministic rules (GS1/UDI checks)
- **Integration:** RPA and REST APIs to PLM, ERP, labeling software and MES
- **Platform:** cloud-native, with confidence scores and human review for low-confidence results

## Accuracy and traceability

- Validation with a golden label set, precision/recall on defect detection, and a shadow-mode pilot
- Every label element is linked to product data, requirement clause, source document, approval and change order
- Immutable audit log, designed to support 21 CFR Part 11 / GAMP 5 practices

## Expected impact (targets, to be validated in a pilot)

| Measure | Target |
|---|---|
| Label change cycle time | 60-70% lower |
| Manual review effort | 50% lower |
| Errors reaching the market | 80%+ lower |
| Element-level traceability | 100% |

## Regulatory references

- FDA: General Device Labeling Requirements; UDI System
- EU MDR (Regulation (EU) 2017/745); EU UDI
- ISO 15223-1 (symbols), ISO 20417 (information supplied by the manufacturer)
- IMDRF N52 (Principles of Labelling)

## Roadmap

1. **Phase 1:** AI compliance checker and artwork redlining
2. **Phase 2:** Change impact engine and GenAI authoring
3. **Phase 3:** Full multi-agent orchestration and predictive quality analytics

## Team

| Name | Technical role |
|---|---|
| [Member 1] |Full Stake Dev  |
| [Member 2] |Data Science Expert|
| [Member 3] |AI/ML Engineer (GenAI, Vision)|

## Status

Concept and solution design for the first-round submission. Impact figures are targets, not measured results.
