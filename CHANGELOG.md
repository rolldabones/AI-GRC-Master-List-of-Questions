# Changelog

All notable changes to this repository. Versions apply to the repository as a whole; all files version in lockstep. Prior versions are superseded, never silently overwritten.

## v1.2.5 - 2026-10-20

**Patch. Review corrections; the question set changes in wording and C2 is split.** Independent review of 20 October 2026; changes made with Claude, approved by Michael Paik. Dates are KST.

- **Questions.** C2 split into C2a (internal use) and C2b (external use); its single form asked "internally only ... as well as externally" and could not be answered yes or no (MLQ-07). C14 now asks whether you develop a general-purpose AI model, or have one developed, and place it on the market under your own name, following Article 3(3) of the EU AI Act (MLQ-04). C13 adds authorized representative and product manufacturer, the remaining operator roles in Article 3(8) (MLQ-12). No other question is renumbered.
- **Internal contradiction resolved.** The README said an unresolved C13 or C14 made the drafts fall back to deployer posture; C13 said the drafts carry a placeholder instead. The placeholder rule is kept and the fallback sentence is conformed (MLQ-01).
- **Claims the paired engine does not back, removed or qualified.** The README no longer promises C13- or C14-specific engine behavior and now says the AI GRC Copilot instructions apply only their general placeholder rule (MLQ-02). The design goal that a "No" often removes an entire section, and the claim that the answers are sufficient to draft all 30 artifacts, are dropped, and the opening sentence no longer says the answers enable the full set of 30 to be generated; the two limits are restated as two known gaps (MLQ-06). The README states that "Unknown/TBD" maps to the instructions' "[TBD]" and "Unknown/Insufficient data" (MLQ-13), and that the instructions stop for a decision on contested choices before drafting (MLQ-14).
- **Regulatory-currency note.** The EU AI Act paragraph is now a dated table of provision, date, pinpoint and as-at date (MLQ-10). The Article 50(2) transition is cited to Article 111(4), inserted by Regulation (EU) 2026/1744, Article 1, point (39)(b), with scope "providers of AI systems, including general-purpose AI systems" (MLQ-03). Chapter V (from 2 August 2025, Article 113, third paragraph, point (b)) and Article 101 fines (from 2 August 2026) are added (MLQ-05). "Korea Standard Time" spelled out at first use and the capital after a colon removed (MLQ-19). The pinpoint sentence no longer calls "Article 113(3)" wrong: the Regulation itself uses that form in Article 111(1); "Article 113, third paragraph" stays the house form (X-02).
- **Readability.** Repository-history sentences removed from the README; they are already recorded in the v1.2.0 entry below (MLQ-09). Acronyms spelled out at first use, including "governance, risk management and compliance (GRC)" (MLQ-16, MLQ-18). Process references in the v1.1.5 to v1.2.3 entries below (review sessions, report items, determinations, rulings, maintenance-list items and check classes) are replaced with plain statements of what changed and why; what those entries record is unchanged (MLQ-08).
- **Citation metadata.** The `CITATION.cff` abstract says "AI GRC Copilot instructions" instead of "Spellbook Copilot" (MLQ-11). The How to Cite block keeps the publisher, "GRC Solutions Korea", as every repository in the account does; `CITATION.cff` cannot carry it because the Citation File Format has no top-level publisher key, and that difference is a format limit, not an inconsistency (MLQ-15).
- **LICENSE.** The summary above the legal code adds the later-version and BY-NC-SA Compatible License options of Section 3(b)(1). The legal code is unchanged (MLQ-20).
- **Errata to shipped entries.** v1.2.1 cited the Article 50(2) transition to Recital 38 only; the operative provision is Article 111(4). v1.1.4 said "Article 113(3)" "is wrong and always was"; it is the Regulation's own shorthand (Article 111(1)), and "Article 113, third paragraph" is the preferred form. v1.2.0 said one LOW would remain on the `v1.1.0` in the promotion note; that token is removed in this release.
- Findings applied: MLQ-01, MLQ-02, MLQ-03, MLQ-04, MLQ-05, MLQ-06, MLQ-07, MLQ-08, MLQ-09, MLQ-10, MLQ-11, MLQ-12, MLQ-13, MLQ-14, MLQ-15, MLQ-16, MLQ-18, MLQ-19, MLQ-20, X-02.
- README masthead, How to Cite and `CITATION.cff` to v1.2.5.

## v1.2.4 - 2026-10-20

- LICENSE: two defects against the Creative Commons legal code corrected (the space in 'ShareAlike. In'; the CC0 sentence of the closing notice). Operative terms unchanged.
- README masthead, How to Cite and `CITATION.cff` to v1.2.4.

## v1.2.3 - 2026-10-18

**Patch. Retirement residue, no change to the question set.** Found in the whole-account review of 15 October 2026. The AI GRC Spellbook Copilot custom GPT was retired on 1 October 2026 and converted to a private plug-in; three sentences still sent the reader to it as a GPT.

- ~~"enables the AI GRC Spellbook Copilot custom GPT to generate the full set"~~ **STRUCK.** Now "enables the AI GRC Copilot instructions, run on any current assistant, to generate the full set".
- ~~"the AI GRC Spellbook Copilot will draft with explicit placeholders"~~ **STRUCK.** Now "the AI GRC Copilot instructions draft with explicit placeholders".
- ~~"You can paste your answers into the AI GRC Spellbook Copilot"~~ **STRUCK.** Now points to an assistant running AI-GRC-Copilot's `instructions.md`.
- One dated sentence under the pairing paragraph states the retirement and points to the account's RETIREMENT.md.
- This repository is added to the account's list of repositories that still referred to the retired GPT; that list item is closed in this release.
- README masthead, How to Cite and `CITATION.cff` to 1.2.3 in lockstep.

## v1.2.2 - 2026-10-17

**Patch. House style, no change to the question set.** Found in the house-style pass of the whole-account review of 15 October 2026.

- `README.md`: "itemised" to "itemized" in live text. The same word in the v1.2.0 entry below is shipped history and is left as written (shipped changelog entries keep their original spelling).
- Closing line added at the end of this file.
- Masthead, How to Cite and `CITATION.cff` to 1.2.2 in lockstep. The history paragraphs and the mirror form were outside the scope of this release.

## v1.2.1 - 2026-10-15

**Patch. Legal currency, no change to the question set.** Found in the legal-currency pass of the whole-account review of 15 October 2026 (KST).

- **Regulatory-currency note.** "Article 50 transparency obligations still apply from 2 August 2026" stated the deployer position only. Since v1.2.0 C13 and C14 ask whether the organization is a provider, so the provider carve-out became material: providers of generative systems placed on the market before 2 August 2026 have until 2 December 2026 for the Article 50(2) marking duty (Recital 38, Regulation (EU) 2026/1744, [OJ L, 2026/1744](http://data.europa.eu/eli/reg/2026/1744/oj)). Added. The note heading records its amendment dates, having been headed "(15 July 2026)" over a 13 August amendment. The note links to the account's canonical [EU AI Act currency note](https://github.com/rolldabones/ai-governance-for-boards/blob/main/05-jurisdictions/eu.md#eu-ai-act-currency-note), published the same day, which governs on conflict.
- Masthead, How to Cite and `CITATION.cff` to 1.2.1 in lockstep. All other files unchanged byte for byte.

## v1.2.0 - 2026-09-08

**Minor. The minimum set changes.** A standing defect on the account's maintenance list is remediated here: the sufficiency claim in `README.md` and proposed addition R2 contradicted each other in terms, and had done since v1.1.0 on 15 July 2026.

- **The contradiction, stated before the fix.** `README.md` line 19 read that answering the questions was sufficient to draft all 30 artifacts. R2, in the proposed-additions block of the same file, read that a "Yes" on general-purpose AI model provision "pulls in GPAI provider obligations that none of the current questions surface". A set that does not surface an obligation is not sufficient to draft the artifact carrying it. Both could not hold, and the file asserted both for seven weeks.

- **STRUCK.** ~~"Answering the questions below is sufficient to draft all 30 artifacts, including:"~~ The claim is **qualified, not struck in the file**, and the reason is recorded rather than left to inference. Striking it in `README.md` would have removed the only statement of what the set covers from the section headed "What this question set covers", leaving a reader of an operative intake instrument with a hole where the coverage claim was. What was false was the unqualified form, not the coverage. The sentence now reads "…subject to the two limits stated after the list", and the two limits are stated in full immediately below the list. The account's maintenance rules place a correction of substance in the changelog, struck and itemised, so it is recorded here.

- **R1 and R2 promoted into the minimum set as C13 and C14**, with `Unknown/TBD` explicitly permitted on both, which is the answer the file has allowed on every question since v1.0.0. C13 asks role, per use case, against the C11 list. C14 asks general-purpose AI model provision. R3 stays proposed.

- **Why C13 and C14 rather than a new section R.** A new lettered section would have taken the count from 17 to 18, and "17 sections" is asserted in three places outside this repository: `rolldabones/ECOSYSTEM.md` line 33, `AI-Governance-Academy/law-firm-ai-deployment-spec.md` line 151, and this repository's own `CITATION.cff` abstract, which is that ECOSYSTEM line verbatim by the house form settled at v1.1.5. This release's scope was this repository, so two of those three could not be corrected here, and a release that knowingly puts a correct fact out of step across three repositories would create on purpose the cross-repository drift the account's maintenance rules exist to prevent. Section C is also the right home on the merits: C11 already collects each use case with its owner, user group and decision impact, and role is an attribute of that list rather than of the organization. **The section count is unchanged at 17 and no existing question is renumbered.** The mapping R1 → C13 and R2 → C14 is recorded here and in the proposed-additions block so the register entry remains traceable.

- **A pointer in section A, where the gap is.** R1's own text said geography does not capture role. The gap it named sits in section A, so section A now carries one line saying so and naming C13 and C14. No question in section A is added, renumbered or changed.

- **The heading of the proposed-additions block loses its version token.** It read "Proposed additions (v1.1.0, under consideration, not yet part of the minimum set)". `v1.1.0` shipped on 15 July 2026 and the repository has passed it five times; the token read as a plan and was a stale label. The account's automated version check reported it as a version lag on every run. That the maintenance list read the same string as forward-looking is recorded in the account's maintenance repository.

- **The automated version check will still report one LOW on this repository**, on the `v1.1.0` in the promotion note, and that is correct: the check reports version tokens and does not judge, and a history line naming the version something was proposed at is legitimate prose. It is a different line from the stale heading and it is stated here so the finding is not read as unchanged.

- **Version bumped at every occurrence:** masthead line 3, the How to Cite block, `CITATION.cff` `version` and `date-released`. `LICENSE.md` is unchanged byte for byte.

## v1.1.5 - 2026-09-06

Citation infrastructure, doctrine citation line and lockstep maintenance. Part of the September 2026 improvement pass, one patch release per repository across all 21 public repositories.

- **`CITATION.cff` added** in the account's house form: no `type` field, `version` and `date-released` in lockstep with the README, `license` as the SPDX identifier for this repository's licence, `abstract` taken from this repository's ECOSYSTEM.md role line rather than newly written.
- **How to Cite block** aligned to this release and pointing at `CITATION.cff`.
- All other files in this repository are unchanged byte for byte.

## v1.1.4 - 2026-08-13

OJ text of the amending regulation obtained; Article 5 date corrected.

**Correction, not a currency update.** The release earlier today stated that the Article 5 application date of 2 February 2025 was "settled and not affected by the Omnibus". Having now read the Official Journal text, that is **wrong in part** and is corrected here.

- **The amending act is identified.** Regulation (EU) 2026/1744 of the European Parliament and of the Council of 8 July 2026, OJ L, 2026/1744, 24.7.2026, ELI http://data.europa.eu/eli/reg/2026/1744/oj, in force 27 July 2026. Article 1, point (40) amends the third paragraph of Article 113 of Regulation (EU) 2024/1689.
- **The pinpoint question is answered.** Article 113 is structured in unnumbered paragraphs with lettered points. The correct citation form is **"Article 113, third paragraph, point (c)"**. "Article 113(3)" is wrong and always was. The prohibition on that form, adopted this morning as a precaution, is now replaced by a positive rule.
- **Article 5 carve-out.** Amended point (a) provides that Chapters I and II apply from 2 February 2025 **with the exception of Article 5(1), first subparagraph, points (ba) and (bb), and Article 5(1a) and (1b), which apply from 2 December 2026**. The general Article 5 date stands; the prohibitions the Omnibus added are deferred. The earlier unqualified statement is struck.
- **High-risk deferrals, verbatim.** Amended point (c): Chapter III, Sections 1, 2 and 3, with the exception of Article 6(5), apply from (i) 2 December 2027 for AI systems classified as high-risk pursuant to Article 6(2) and Annex III, and (ii) 2 August 2028 for those classified pursuant to Article 6(1) and Annex I.
- **New point (d).** Articles 102 to 110 apply from 27 July 2026.
- The OJ-text gap flag is removed from every file that carried it. That outstanding item is closed.

## v1.1.3 - 2026-08-13

License metadata sweep. An `SPDX-License-Identifier: CC-BY-NC-SA-4.0` line and the canonical Creative Commons legal code are now carried inside the existing license file. The filename is unchanged and the human-readable summary is retained above the legal code.

- The primary audience is automated intake and provenance tooling, which reads the SPDX tag rather than prose. Automated license detection previously reported nothing across all twenty-one repositories in this account.
- No change to the licence in force. The identifier records what was already true.

## v1.1.2 - 2026-08-13

Omnibus currency remediation. The Digital Omnibus on AI entered into force on 27 July 2026; notes describing Official Journal publication as pending are recast as operative law with dated amendment notes. The Article 5 application date of 2 February 2025 is stated as fact (Article 113, point (a)). No pinpoint to a numbered subsection of Article 113 is given: the amending regulation's Official Journal text has not been read and its renumbering is unconfirmed.

- README.md: the A4 guidance entry recast from awaiting publication to entered into force 27 July 2026, with a dated amendment note. Pairs with AI-GRC-Copilot v1.1.2, which carried the identical text.

## v1.1.1 - 2026-07-30

### Changed
- Trademark rendering corrected to the canonical closed-up form GRCnext™. The retired spaced form "GRC next" is withdrawn from repository prose. One occurrence, in the grc line of the Part of the ecosystem section.
- Version line updated in lockstep.

## v1.1.0 - 2026-07-15

- All 17 question sections (A-Q) reformatted from tab-indented bullet code blocks to standard Markdown lists; questions preserved verbatim
- "⸻" separators replaced with standard horizontal rules; en dashes in ranges normalized to hyphens for plain-text portability
- Duplicated title and intro paragraph consolidated; GPT referenced by its deployed name, AI GRC Spellbook Copilot, with a link to the paired AI-GRC-Copilot repository
- Added Proposed additions section (R1 jurisdiction role, R2 GPAI provider status, R3 non-EU/UK/US AI statutes), clearly marked as outside the minimum sufficiency set
- Added dated regulatory-currency note (ISO/IEC 42001:2023 current; NIST AI RMF 1.0 plus GenAI Profile; EU Digital Omnibus on AI adopted, awaiting OJ publication; DPIA terminology localization note)
- Added Part of the ecosystem section linking the canonical map and five nearest neighbors
- Added LICENSE (CC BY-NC-SA 4.0) and this CHANGELOG
- Tagged v1.1.0

## v1.0.0 - baseline

- Initial README: design goals, coverage statement, usage instructions and the 17 question sections (A-Q), formatted with tab-bullet code blocks and "⸻" separators. No LICENSE, CHANGELOG or tags.

---

**Final Liability rests with the Human.**
