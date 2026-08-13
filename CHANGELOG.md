# Changelog

All notable changes to this repository. Versions apply to the repository as a whole; all files version in lockstep. Prior versions are superseded, never silently overwritten.

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
