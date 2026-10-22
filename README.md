# Sergey Boyko (Boiko in official documents)

**Researcher in AI evaluation and verification · background in fraud and security investigations**
Almaty, Kazakhstan · Fellow, [Ronin Institute for Independent Scholarship 2.0](https://ronininstitute.org/scholars/) (independent affiliation) · [ORCID](https://orcid.org/0009-0009-2178-5701) · [LinkedIn](https://linkedin.com/in/sergey-boyko-researcher)

For 20+ years I investigated fraud and prepared evidence for legal decisions: police investigator, then security and anti-fraud lead in finance and fintech (Director of Internal and Economic Security at Solva Group, seven legal entities, until September 2026). I now apply the same discipline to AI-generated results and scientific claims: test them against independent evidence, controls and counterexamples, and state where the result stops holding.

## Research

- **AIAS+ 2026:** the paper *Kill Before You Commit: A Falsification-First Loop for AI-Assisted Scientific Discovery* is accepted for a poster presentation (5–7 November 2026). It remains under second-round review for the conference proceedings and is not yet accepted for publication.
- **Method:** falsification first. A separate AI agent tries to break an initial analysis; verified findings are kept apart from inferences and open claims.
- **Own result downgraded after self-audit.** [ARCHCODE](https://github.com/sergeeey/ARCHCODE) reported a pooled AUC of 0.977 on 353 ClinVar HBB variants. The audit in its README shows that the figure follows variant-category composition: with a position-only control the AUC is 0.551, and the median within-category AUC across 25 category-locus combinations is 0.52, both close to chance. The caveat is at the top of that README, next to the number.

## Projects

| Project | What it does | Status and limits |
|---|---|---|
| [Skeptic Engine](https://github.com/sergeeey/Skeptic-Engine-2026-) | Adversarial checks for scientific data integrity: statistical artifacts and structural inconsistencies in genomics, proteomics and biomedical data. 360 unit tests (they check code behaviour, not detection accuracy). | Research toolkit. Finds anomalies, not misconduct. Results on simulated fabrication and on real fraud labels are reported separately; some experiments have n=59–99 with wide confidence intervals. |
| [ScannerGap](https://github.com/sergeeey/scannergap) | Maps where static analysis stops seeing. Gold subset: 23 annotated real CVEs scored HIT / PARTIAL / MISS against Semgrep and Bandit. Exploratory run: 83 of 135 CVEs (61.5%) missed by both. | Research prototype. The 135-CVE set is author-selected and its manifest is not frozen; reproducibility is not complete. CodeQL is a separate exploratory subset. Not a benchmark result. |
| [mcp-bouncer](https://github.com/sergeeey/mcp-bouncer) | Prompt-injection pre-filter for MCP servers and AI agents that read external content. Python standard library only, eight attack classes, MIT. | Heuristic pre-filter, not an LLM guardrail; a determined attacker can bypass it. |
| [methodology-router](https://github.com/sergeeey/A---6-methodology-router) | Local CLI that freezes research claims, routes them to methods through explicit gates and keeps a hash-chained evidence ledger. No PASS without a run receipt. | MVP. |
| [Claude-cod-top-2026](https://github.com/sergeeey/Claude-cod-top-2026) | Methodology for Claude Code: evidence markers, audit gates, anti-hallucination rules, validation-theater checks. MIT. | Used in my own projects. |

## Earlier work

Computational genomics (ARCHCODE, chromatin loop extrusion for regulatory variant interpretation) and spectral toy-model research ([N-7-GeoSpectra-Lab](https://github.com/sergeeey/N-7-GeoSpectra-Lab), with explicit non-claims). Both publish controls and negative results next to the headline.

## Tools

Python 3.11+ · pytest · GitHub Actions · Semgrep rules · CVE analysis (NVD) · reproducible experiment design with controls · LLM and AI-agent workflows.

Open to research collaboration and roles in AI evaluation, AI safety and fraud/abuse investigations.
