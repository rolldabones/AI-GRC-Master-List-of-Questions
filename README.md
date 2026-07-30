# AI GRC Master List of Minimum Questions

**Version 1.1.1 · 30 July 2026**

This is a Master List of Minimum Questions that, if answered, enables the [AI GRC Spellbook Copilot](https://github.com/rolldabones/AI-GRC-Copilot) custom GPT to generate the full set of 30 canonical AI GRC artifact drafts (policy, charters, registers, SOPs, protocols, monitoring, incident, vendor, audit, training, ISO roadmap, regulatory playbook, continuous improvement).

This repository and [AI-GRC-Copilot](https://github.com/rolldabones/AI-GRC-Copilot) are a pair: that repo holds the drafting engine, this repo holds the minimum input set that feeds it.

## Design goals

- Binary yes/no wherever possible
- Only a small number of non-binary fields for names, lists and numeric thresholds
- Questions are structured so a "No" often removes an entire section of multiple documents

If you cannot answer something, you can respond "Unknown/TBD" and the AI GRC Spellbook Copilot will draft with explicit placeholders and an open-items list.

## What this question set covers

Answering the questions below is sufficient to draft all 30 artifacts, including:

- AI policy, governance charter, code of conduct, RACI
- Risk framework, risk register, compliance register, audit plan
- Inventory and classification register, lifecycle SOPs, change management
- Model Risk Management (MRM) policy, bias and fairness protocol, explainability standards, human-in-the-loop (HITL) guidelines
- Data policy for AI, DPIA process, provenance and lineage docs
- Incident response plan, vendor risk policy, monitoring plan
- Model cards, decision log, stakeholder feedback record, tracker
- Training framework, awareness plan, ISO/IEC 42001 roadmap, regulatory engagement playbook, continuous improvement plan

Of course, these drafts then need to be reviewed, augmented, approved and activated for your GRC system. Final Liability rests with the Human.

## Fastest way to use these questions

You can answer in a compact format like:

- "A4: Yes, A5: No, ..."
- Names and systems in plain text
- Everything else Yes/No

You can paste your answers into the AI GRC Spellbook Copilot, along with the questions for context, and then ask it to generate the full 30-document artifact pack set with:

- Owner and accountable approver
- Control objective and steps
- Evidence and system of record
- Review cadence and KPIs
- Exceptions process
- Links to dependent artifacts
- An open-items list for any "Unknown/TBD" responses

---

## A. Identity, scope, jurisdictions (non-binary where necessary)

- A1 (Text): Organization legal name for documents
- A2 (Text): Primary business sector / industry
- A3 (List): Operating countries and jurisdictions (top 5 is fine)
- A4 (Y/N): Do you operate in the EU or serve EU residents?
- A5 (Y/N): Do you operate in the UK or serve UK residents?
- A6 (Y/N): Do you operate in the US or serve US residents?
- A7 (Y/N): Is the organization regulated by a sector regulator (financial, health, telecom, etc.)?
- A8 (Text): If yes, name the regulator(s)
- A9 (Y/N): Do you want the artifacts to be written as a global baseline with local addenda?

---

## B. Executive accountability, owners, escalation (mostly non-binary for names)

- B1 (Text): Accountable executive for AI governance (single name and title)
- B2 (Y/N): Is there an existing risk owner role (CRO or equivalent)?
- B3 (Text): Head of Legal name/title (or external counsel contact)
- B4 (Text): Privacy officer / DPO name/title (or "None")
- B5 (Text): Security lead name/title (CISO or equivalent)
- B6 (Text): Engineering lead name/title responsible for AI delivery
- B7 (Text): Internal Audit lead name/title (or "No Internal Audit")
- B8 (Y/N): Do you already have an enterprise risk committee that can take AI oversight?
- B9 (Y/N): Do you want a dedicated AI Governance Committee chartered?
- B10 (Y/N): Do you require Legal review and sign-off before any AI system goes live?
- B11 (Y/N): Do you require Risk review and sign-off before any AI system goes live?
- B12 (Y/N): Do you require Privacy review and sign-off before any AI system goes live?
- B13 (Y/N): Do you require Security review and sign-off before any AI system goes live?
- B14 (Y/N): Do you require an executive approver for "High risk" AI releases?
- B15 (Non-binary): Escalation path for AI incidents (role chain, not individuals if preferred)

---

## C. AI system landscape, use cases, impact (minimum to populate inventory, classification, model cards)

- C1 (Y/N): Do you currently use AI in production?
- C2 (Y/N): Do you use AI internally only (employee-facing) as well as externally (customer/public-facing)?
- C3 (Y/N): Do any AI outputs influence decisions about people (employment, credit, eligibility, access, pricing, safety)?
- C4 (Y/N): Do any AI systems operate in real time (sub-second decisions)?
- C5 (Y/N): Do you use generative AI (LLMs, image generation, code generation) in any business process?
- C6 (Y/N): Do you deploy any custom-trained models (not only vendor APIs)?
- C7 (Y/N): Do you fine-tune vendor foundation models on your data?
- C8 (Y/N): Do you use open-source models in production?
- C9 (Y/N): Do you use AI agents or tool-using workflows that can take actions (not just generate text)?
- C10 (Y/N): Do you use AI for safety critical functions (health, transportation, industrial control, security operations)?
- C11 (List): Top 5 AI use cases, each with: name, business owner role, user group (internal/external), decision impact (advisory vs automated)
- C12 (Y/N): Do you need an appeals or contestability process for affected users?

---

## D. Data types, privacy, rights, provenance (drives DPIA, data policy, lineage)

- D1 (Y/N): Do any AI systems process personal data?
- D2 (Y/N): Do any AI systems process sensitive personal data (health, biometrics, children, precise location, etc.)?
- D3 (Y/N): Do you process data about minors?
- D4 (Y/N): Do you use customer content or user-generated content as training or evaluation data?
- D5 (Y/N): Do you use employee data for training or evaluation?
- D6 (Y/N): Do you use third-party licensed datasets?
- D7 (Y/N): Do you scrape public web data for training or evaluation?
- D8 (Y/N): Do you have documented lawful basis and notices for AI-related processing (where applicable)?
- D9 (Y/N): Do you have a data retention schedule that covers AI training, prompts, logs, outputs?
- D10 (Y/N): Do you have a process to honor data subject rights (access, deletion, correction) that includes model-related data?
- D11 (Y/N): Do you require dataset provenance documentation for every model?
- D12 (Y/N): Do you require training data to be reproducible (same inputs can be reassembled later)?
- D13 (Y/N): Do you require content filtering or PII redaction before training?

---

## E. Risk appetite, unacceptable failures, thresholds (feeds risk register, controls, stop rules)

- E1 (Y/N): Do you have an existing enterprise risk appetite statement that AI should inherit?
- E2 (Y/N): Do you want to define AI-specific "unacceptable outcomes" explicitly?
- E3 (Y/N): Is harm to individuals (financial, reputational, discrimination) treated as a top-tier risk category?
- E4 (Y/N): Is regulatory non-compliance treated as a top-tier risk category?
- E5 (Y/N): Is security misuse (prompt injection, data exfiltration, jailbreaks) treated as a top-tier risk category?
- E6 (Y/N): Do you require human-in-the-loop for any high-impact decision about individuals?
- E7 (Y/N): Do you allow fully automated decisions about individuals without human review?
- E8 (Y/N): Do you require pre-launch fairness testing when a model affects people?
- E9 (Y/N): Do you require explainability artifacts for any customer-facing AI?
- E10 (Non-binary numeric): What is your risk rating scale (eg 1-5 likelihood x impact), or "Use a standard 1-5"?
- E11 (Non-binary): Define what counts as "High risk" in plain terms (one paragraph is enough)
- E12 (Y/N): Do you want explicit stop-ship criteria for AI releases?

---

## F. Governance structure, decision rights, records (feeds charter, RACI, decision log)

- F1 (Y/N): Do you want one central AI Governance Committee?
- F2 (Y/N): Do you want a separate Model Risk function (MRM) distinct from engineering?
- F3 (Y/N): Do you want a single accountable owner per AI system (Model Owner concept)?
- F4 (Y/N): Do you want a single accountable owner per dataset used for AI (Data Owner concept)?
- F5 (Y/N): Do you require documented approval gates at each lifecycle stage (intake, design, test, deploy, monitor, retire)?
- F6 (Y/N): Do you require a formal exception process with time-bound remediation?
- F7 (Y/N): Do you require a decision log for material AI decisions?
- F8 (Y/N): Do you require stakeholder feedback capture for customer-facing AI?

---

## G. Tooling and system of record (evidence-first foundations)

- G1 (Non-binary): Primary ticketing system (Jira, ServiceNow, other)
- G2 (Non-binary): Primary document repository (Confluence, SharePoint, Google Drive, other)
- G3 (Non-binary): Source control (GitHub, GitLab, other)
- G4 (Y/N): Do you have a model registry today?
- G5 (Y/N): Do you have experiment tracking today (MLflow or equivalent)?
- G6 (Y/N): Do you have centralized logging for AI prompts, outputs, errors?
- G7 (Y/N): Do you have monitoring dashboards for AI performance and drift?
- G8 (Y/N): Do you have an incident management platform with on-call?
- G9 (Y/N): Do you have an internal audit evidence repository or GRC tool?
- G10 (Non-binary): Where will the AI System Inventory live as system of record?
- G11 (Non-binary): Evidence retention requirement (eg 1 year, 3 years), or "TBD"

---

## H. AI lifecycle controls (feeds lifecycle SOPs, change management, monitoring)

- H1 (Y/N): Do you require an intake form before any AI work begins?
- H2 (Y/N): Do you require threat modeling for AI systems?
- H3 (Y/N): Do you require pre-deployment validation and sign-off?
- H4 (Y/N): Do you require post-deployment monitoring with defined SLAs?
- H5 (Y/N): Do you allow shadow deployments or dark launches?
- H6 (Y/N): Do you allow continuous deployment for models without manual approval?
- H7 (Y/N): Do you require rollback plans for model changes?
- H8 (Y/N): Do you require periodic recertification of models (eg every 6 or 12 months)?
- H9 (Y/N): Do you require retirement criteria and decommission steps for models?

---

## I. Model risk management specifics (feeds MRM policy, testing protocols, model cards)

- I1 (Y/N): Do you want an explicit Model Risk Management Policy document?
- I2 (Y/N): Do you require model cards for every deployed AI system?
- I3 (Y/N): Do you require documented evaluation datasets and sampling plans?
- I4 (Y/N): Do you require reproducible evaluation runs (versioned code, data, parameters)?
- I5 (Y/N): Do you require robustness testing (adversarial prompts, stress tests)?
- I6 (Y/N): Do you require calibration and confidence reporting where applicable?
- I7 (Y/N): Do you require red teaming for generative AI?
- I8 (Y/N): Do you require periodic bias regression tests after updates?

---

## J. Fairness, explainability, transparency, human oversight (feeds 4 separate standards)

- J1 (Y/N): Do any models produce outcomes that could create disparate impact across protected groups?
- J2 (Y/N): Do you have access to demographic attributes to measure fairness?
- J3 (Y/N): If you do not have demographics, do you want proxy or qualitative fairness methods?
- J4 (Y/N): Do you require user-facing disclosures when AI is used (eg "AI-assisted" labeling)?
- J5 (Y/N): Do you require explanations to end users for adverse outcomes?
- J6 (Y/N): Do you require a human review path for adverse decisions?
- J7 (Y/N): Do you require a documented appeals workflow with timelines?

---

## K. Security, abuse, safety controls (feeds monitoring plan, incident plan, vendor clauses)

- K1 (Y/N): Do you require secure-by-default prompt and output handling (no secrets in prompts)?
- K2 (Y/N): Do you require prompt injection testing for any tool-using or RAG system?
- K3 (Y/N): Do you require data loss prevention controls for AI tooling?
- K4 (Y/N): Do you restrict use of public AI tools for confidential data?
- K5 (Y/N): Do you require vulnerability management to include model and pipeline components?
- K6 (Y/N): Do you require abuse monitoring (toxic outputs, policy violations, self-harm content, fraud enablement)?

---

## L. Vendor and third-party AI (feeds vendor policy, due diligence checklist, contract minimums)

- L1 (Y/N): Do you use any third-party AI vendors in production?
- L2 (Y/N): Do vendors process your customer personal data?
- L3 (Y/N): Do you require vendors to support audit rights (SOC 2 reports, pen tests, assurance)?
- L4 (Y/N): Do you require contract clauses for data ownership, training restrictions, deletion, breach notice?
- L5 (Y/N): Do you require vendors to disclose sub-processors and model changes?
- L6 (Y/N): Do you require an offboarding plan for vendor AI (data return, deletion, continuity)?
- L7 (Y/N): Do you require ongoing vendor performance monitoring, not only initial due diligence?

---

## M. Incident response and escalation (feeds AI incident plan plus regulator playbook hooks)

- M1 (Y/N): Do you want a dedicated AI incident severity taxonomy (Sev 1-4) distinct from general incidents?
- M2 (Y/N): Do you require reporting of certain AI incidents to Legal within 24 hours?
- M3 (Y/N): Do you require customer notification workflows for AI-caused harm or data exposure?
- M4 (Y/N): Do you require regulator notification decisioning to be led by Legal?
- M5 (Y/N): Do you require post-incident root cause analysis and CAPA for all Sev 1-2 AI incidents?
- M6 (Y/N): Do you require an incident evidence bundle (logs, prompts, outputs, model version, approvals)?

---

## N. Audit, assurance, compliance mapping (feeds audit plan, compliance register, ISO roadmap)

- N1 (Y/N): Do you want explicit alignment to ISO/IEC 42001?
- N2 (Y/N): Do you want explicit alignment to NIST AI RMF?
- N3 (Y/N): Do you want to map to any internal control framework (ISO 27001, SOC 2, COSO)?
- N4 (Y/N): Do you require an annual AI audit plan with defined test procedures?
- N5 (Y/N): Do you want independent validation for high-risk models (separate team or external)?
- N6 (Y/N): Do you need a compliance register that tracks obligations per jurisdiction and use case?

---

## O. Training, communications, adoption (feeds training framework and awareness plan)

- O1 (Y/N): Do you require mandatory AI training for all employees?
- O2 (Y/N): Do you require role-based training for engineers, product, support, legal, risk?
- O3 (Y/N): Do you require attestations (employees confirm understanding)?
- O4 (Y/N): Do you require periodic refresh training (eg annual)?
- O5 (Y/N): Do you want an AI acceptable use policy for employee tooling?
- O6 (Y/N): Do you require a communications plan for external disclosures about AI use?

---

## P. Operating cadence, KPIs, continuous improvement (feeds KPIs, review gates, CI plan)

- P1 (Y/N): Do you want monthly governance reporting?
- P2 (Y/N): Do you want quarterly governance reporting?
- P3 (Y/N): Do you want standard KPIs across all AI systems (inventory completeness, review SLA, incident rate, exceptions aging)?
- P4 (Y/N): Do you require periodic control effectiveness reviews (eg semi-annual)?
- P5 (Y/N): Do you require a formal continuous improvement backlog for AI GRC?
- P6 (Y/N): Do you require a documented exceptions process with metrics (count, age, overdue)?

---

## Q. Document style and enforcement (keeps drafts consistent across the 30 artifacts)

- Q1 (Y/N): Do you want all documents written as policy-like (shall/required) rather than guidance-like (should)?
- Q2 (Y/N): Do you want a single global policy plus SOP annexes, not 30 standalone policies?
- Q3 (Y/N): Do you want every control to specify evidence, system of record, owner, review cadence?
- Q4 (Y/N): Do you want enforcement language (consequences for non-compliance) included?
- Q5 (Y/N): Do you want templates embedded in each artifact (forms, checklists), not just referenced?

---

## Proposed additions (v1.1.0, under consideration, not yet part of the minimum set)

Answering these sharpens the compliance register, vendor policy and regulatory playbook. They are not required for the sufficiency claim above.

- R1 (Per use case): For each AI system in scope, does the organization act as provider, deployer, importer or distributor? Obligations under the EU AI Act and comparable regimes differ sharply by role, and geography (A3-A6) does not capture role.
- R2 (Y/N): Do you develop or place general-purpose AI models on the market (as opposed to only building on top of them)? A "Yes" pulls in GPAI provider obligations that none of the current questions surface.
- R3 (Y/N): Do you operate in or serve residents of jurisdictions with dedicated AI statutes beyond the EU, UK and US (eg Korea's AI Framework Act)? A3 collects the country list but nothing flags AI-specific local law as a drafting trigger.

---

## Regulatory-currency note (15 July 2026)

- ISO/IEC 42001:2023 remains the current edition of the AI management system standard (N1). EN ISO/IEC 42001:2026 is the CEN European adoption of the same 2023 text, not a revision. The companion impact assessment methodology is ISO/IEC 42005:2025.
- NIST AI RMF (N2) refers to version 1.0 (January 2023) together with the Generative AI Profile (NIST AI 600-1, July 2024).
- For organizations answering "Yes" to A4: the EU Digital Omnibus on AI was adopted by the European Parliament on 16 June 2026 and the Council on 29 June 2026 and awaits publication in the Official Journal as of this note. On entry into force it defers Annex III high-risk obligations to 2 December 2027 and Annex I embedded high-risk obligations to 2 August 2028. Until publication, 2 August 2026 remains the legally operative date.
- DPIA and data subject rights questions (Section D) use GDPR terminology. Equivalent triggers exist under other regimes (UK GDPR, US state privacy laws, Korea's PIPA); the drafts should localize per A3.
- These questions name alignment targets for drafting purposes. They are not conformity claims. Verify current status before relying on any of them.

## Part of the ecosystem

This repository is part of the [rolldabones governance ecosystem](https://github.com/rolldabones/rolldabones/blob/main/ECOSYSTEM.md). Nearest neighbors:

- [AI-GRC-Copilot](https://github.com/rolldabones/AI-GRC-Copilot) - the paired drafting engine these questions feed
- [AI-Impact-Assessment-Tool](https://github.com/rolldabones/AI-Impact-Assessment-Tool) - the per-system assessment whose findings populate several answers here
- [grc-workbook](https://github.com/rolldabones/grc-workbook) - the module-by-module instrument for building the GRC capability the 30 artifacts document
- [RedCap-01](https://github.com/rolldabones/RedCap-01) - the diagnostic testing whether the resulting ERM actually improves decisions
- [grc](https://github.com/rolldabones/grc) - the GRCnext™ framework supplying the primitives behind the question design

## License

[CC BY-NC-SA 4.0](LICENSE.md). Attribution required, non-commercial use, share alike.

---

Final Liability rests with the Human.
