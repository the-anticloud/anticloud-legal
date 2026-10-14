# LEGAL

![license](https://img.shields.io/badge/license-license-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-legal_tech-lightgrey)

> Anticloud-hardened packaging of the upstream project `LEGAL` in category **LEGAL TECH**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** LEGAL TECH · **Upstream:** https://github.com/anthropics/claude-for-legal · **Upstream pin:** `4a6c651889c97cc9140580363c73e0eb17379c2b` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

# Claude for Legal

Reference agents, skills, and data connectors for the legal workflows we see most — in-house commercial, privacy, product, corporate, employment, litigation, regulatory, AI governance, IP, and the learning side of the practice (law school clinics and students).

> **New here?** Start with [QUICKSTART.md](QUICKSTART.md) — install in 60 seconds. This README is the full reference.

Everything here is available **two ways from one source**: install it as a [Claude Cowork](https://claude.com/product/cowork) or [Claude Code](https://claude.com/product/claude-code) plugin, or deploy it through the [Claude Managed Agents API](https://docs.claude.com/en/api/managed-agents) behind your own workflow engine. Same system prompt, same skills — you choose where it runs.

## Getting started in Cowork
- [Install Claude Desktop](https://claude.com/download)
- Get access to Claude Cowork
- Follow the instructions in the video below:

https://github.com/user-attachments/assets/51394f0a-5277-4fe2-b81c-5c5e9ac876b5

> [!IMPORTANT]
> **Every output from these plugins is a draft for attorney review — not legal advice, not a legal conclusion, not a substitute for a lawyer.** They are built with guardrails that reflect that: source attribution on every citation, conservative defaults on privilege and subjective legal calls, jurisdiction assumptions surfaced, and explicit gates before anything is filed, sent, or relied on. A lawyer reviews, verifies, and takes professional responsibility for anything that leaves the building. These plugins make that review faster; they do not replace it.
>
> **These plugins do not represent Anthropic's legal positions.** They are tools that help lawyers analyze issues. Where a skill includes a checklist item, a suggested framework, a risk flag, or a characterization of case law or regulatory guidance, that is an aid to the reviewing attorney's own analysis, not a statement of Anthropic's view of the law. The law in many of these areas is unsettled and evolving. The attorney using the plugin — not the plugin, and not Anthropic — is responsible for the legal positions taken in their work product.

What's in the project:

- **Practice-area plugins** covering in-house, firm, and academic legal work — each one built around a cold-start interview that learns your playbook and a `CLAUDE.md` practice profile that every skill reads from.
- **Managed-agent cookbooks** for the scheduled, eyes-on-the-feed workflows (renewal watcher, docket watcher, regulatory feed monitor, diligence grid, launch radar).
- **MCP connectors** across general productivity (Slack, Google Drive, Box) and legal-specific systems (Ironclad, DocuSign, iManage, Everlaw, CourtListener, and more).
- **[Named agents](#agents)** — end-to-end workflow agents (Vendor Agreement Reviewer, DSAR Responder, Termination Reviewer, Claim Chart Builder, …) with job-style names and a single command to run each one.

## Agents

Each agent is named for the workflow it runs. They're the most common surface — start with the ones that match your work, then tune the underlying skill, the practice profile, and the connectors to how your team does it.

| Agent | What it does | Plugin | Command |
|---|---|---|---|
| **Vendor Agreement Reviewer** | Reviews a vendor MSA against your playbook and produces a redline memo | `commercial-legal` | `/commercial-legal:review` |
| **NDA Triager** | GREEN/YELLOW/RED triage of inbound NDAs so only the hard ones hit a lawyer's desk | `commercial-legal` | `/commercial-legal:review` |
| **Amendment Tracer** | Traces how a contract has changed across its base agreement and every amendment | `commercial-legal` | `/commercial-legal:amendment-history` |
| **Renewal Watcher** | Scans the contract register for cancel-by and renewal deadlines | `commercial-legal` | scheduled agent |
| **Deal Debrief** | Weekly sweep of signed agreements with playbook deviations — prompts the attorney to log context while memory is fresh | `commercial-legal` | scheduled agent |
| **Playbook Monitor** | Watches the deviation log and proposes playbook updates when a clause has drifted | `commercial-legal` | scheduled agent |
| **Escalation Router** | Routes contract issues to the right approver and drafts the ask | `commercial-legal` | `/commercial-legal:escalation-flagger` |
| **Tabular Diligence Review** | Tabular review over a data room with one row per document and every cell cited | `corporate-legal` | `/corporate-legal:tabular-review` |
| **Issue Extractor** | Reads VDR documents and extracts issues per house categories and materiality thresholds | `corporate-legal` | `/corporate-legal:diligence-issue-extraction` |
| **Board Consent Drafter** | Drafts unanimous written consents in house format with precedent search | `corporate-legal` | `/corporate-legal:written-consent` |
| **Material Contracts Schedule Builder** | Builds the disclosure schedule from diligence findings against the purchase-agreement threshold | `corporate-legal` | `/corporate-legal:material-contract-schedule` |
| **Entity Compliance Tracker** | Computes filing deadlines across jurisdictions and entity types, runs health audits | `corporate-legal` | `/corporate-legal:entity-compliance` |
| **Closing Checklist Driver** | Tracks every condition, consent, document, and filing blocking close | `corporate-legal` | `/corporate-legal:closing-checklist` |
| **Integration Runbook** | Phased post-closing integration plan with consent tracking and weekly status | `corporate-legal` | `/corporate-legal:integration-management` |
| **Data Room Watcher** | Monitors the VDR for new uploads and posts closing checklist status on schedule | `corporate-legal` | scheduled agent |
| **Termination Reviewer** | Runs a proposed termination against jurisdiction-specific risk flags | `employment-legal` | `/employment-legal:termination-review` |
| **Hire Reviewer** | Reviews offer letters and restrictive covenants with a jurisdiction check | `employment-legal` | `/employment-

*(excerpt; full text in `UPSTREAM_CLONE/`)*

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Unknown (no standard manifest detected)** (manifests: none detected; scanned in UPSTREAM_CLONE)
- Top-level source layout: `ai-governance-legal/`, `commercial-legal/`, `corporate-legal/`, `employment-legal/`, `external_plugins/`, `ip-legal/`, `law-student/`, `legal-builder-hub/`, `legal-clinic/`, `litigation-legal/`, `managed-agent-cookbooks/`, `privacy-legal/`
- Snapshot size: **300 files**, **745 lines of code** (measured; see Benchmarks)
- Primary languages: `.md` (221), `.yaml` (29), `.json` (28), `(none)` (17), `.py` (3), `.sh` (2)
- Upstream commit pinned for this packaging: `4a6c651889c97cc9140580363c73e0eb17379c2b`

---

## Installation

Everything here is available **two ways from one source**: install it as a [Claude Cowork](https://claude.com/product/cowork) or [Claude Code](https://claude.com/product/claude-code) plugin, or deploy it through the [Claude Managed Agents API](https://docs.claude.com/en/api/managed-agents) behind your own workflow engine. Same system prompt, same skills — you choose where it runs.

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

> **New here?** Start with [QUICKSTART.md](QUICKSTART.md) — install in 60 seconds. This README is the full reference.

Everything here is available **two ways from one source**: install it as a [Claude Cowork](https://claude.com/product/cowork) or [Claude Code](https://claude.com/product/claude-code) plugin, or deploy it through the [Claude Managed Agents API](https://docs.claude.com/en/api/managed-agents) behind your own workflow engine. Same system prompt, same skills — you choose where it runs.

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

> **New here?** Start with [QUICKSTART.md](QUICKSTART.md) — install in 60 seconds. This README is the full reference.

Everything here is available **two ways from one source**: install it as a [Claude Cowork](https://claude.com/product/cowork) or [Claude Code](https://claude.com/product/claude-code) plugin, or deploy it through the [Claude Managed Agents API](https://docs.claude.com/en/api/managed-agents) behind your own workflow engine. Same system prompt, same skills — you choose where it runs.

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Unknown (no standard manifest detected) |
| Manifests detected | none |
| Files in snapshot | 300 |
| Lines of code | 745 |
| Dependency references | 0 |
| Upstream license | Apache-2.0 |
| Overlay license | Anticommons 0.1.0 |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

| **Subpoena Triage** | Classifies, scopes, and plans compliance with a new subpoena | `litigation-legal` | `/litigation-legal:subpoena-triage` |
| **Chronology Builder** | Builds or updates a chronology from declared sources and uploads | `litigation-legal` | `/litigation-legal:chronology` |
| **Deposition Prep** | Builds a deposition outline tied to case theory with docs and impeachment | `litigation-legal` | `/litigation-legal:deposition-prep` |
| **Brief Section Drafter** | Drafts a brief section in house style, consistent with case theory | `litigation-legal` | `/litigation-legal:brief-section-drafter` |
| **Privilege Log Reviewer** | First-pass privilege log review — obvious calls + flags for attorney review | `litigation-legal` | `/litigation-legal:privilege-log-review` |
| **Legal Hold** | Issue, refresh, release, or report on legal holds | `litigation-legal` | `/litigation-legal:legal-hold` |
| **Matter Intake** | Uniform intake for a new matter — writes matter.md, history.md, appends to log | `litigation-legal` | `/litigation-legal:matter-intake` |
| **Matter Briefing** | Deep briefing on one matter — ready for a GC or outside counsel call | `litigation-legal` | `/litigation-legal:matter-briefing` |
| **Portfolio Status** | Risk distribution, upcoming deadlines, stale matters | `litigation-legal` | `/litigation-legal:portfolio-status` |
| **Outside Counsel Status** | Generates weekly status-request drafts across the active portfolio | `litigation-legal` | `/litigation-legal:oc-status` |
| **Clinic Intake** | Structured client intake with cross-area issue spotting and conflict flags | `legal-clinic` | `/legal-clinic:client-intake` |
| **Case Memo Scaffold** | IRAC-scaffolded case analysis memo with research gaps flagged | `legal-clinic` | `/legal-clinic:memo` |
| **Research Roadmap** | Statutes to check, case law areas, Westlaw search terms — leads, not cites | `legal-clinic` | `/legal-clinic:research-start` |
| **Clinic Deadline Tracker** | Add, report, update, and close case deadlines with malpractice-aware warnings | `legal-clinic` | `/legal-clinic:deadlines` |
| **Case Status Summarizer** | Case status by audience — client, professor, or court-ready | `legal-clinic` | `/legal-clinic:status` |
| **Client Letter Drafter** | Routine client correspondence — appointment confirms, doc requests, updates | `legal-clinic` | `/legal-clinic:client-letter` |
| **Student Ramp** | Semester onboarding — clinic procedures, tool walkthrough, practice exercises | `legal-clinic` | `/legal-clinic:ramp` |
| **Semester Handoff** | End-of-semester case handoff memos — the mirror of ramp | `legal-clinic` | `/legal-clinic:semester-handoff` |
| **Supervisor Review Queue** | Professor's review queue (when formal review supervision is configured) | `legal-clinic` | `/legal-clinic:supervisor-review-queue` |
| **Bar Prep Coach** | Jurisdiction-aware MBE and essay practice targeted at weak subjects | `law-student` | `/law-student:bar-prep-questions` |
| **Socratic Drill Sergeant** | It asks, you answer, it pushes back — does not give you the answer | `law-student` | `/law-student:socratic-drill` |
| **IRAC Grader** | Grades your IRAC essay on structure, issue-spotting, rules, analysis | `law-student` | `/law-student:irac-practice` |
| **Case Briefer** | Brief a case in your preferred format | `law-student` | `/law-student:case-brief` |
| **Outline Builder** | Build or extend an outline in your format from class notes and casebook | `law-student` | `/law-student:outline-builder` |
| **Cold Call Prep** | Predicts professor's questions and drills them before class | `law-student` | `/law-student:cold-call-prep` |
| **Exam Forecaster** | Analyze past exams from the same professor; forecast likely emphases | `law-student` | `/law-student:exam-forecast` |
| **Legal Writing Critic** | Structural feedback on a draft — never rewrites | `law-student` | `/law-student:legal-writing` |
| **Flashcard Drillmaster** | Generate or drill flashcards — Leitner-style buckets | `law-student` | `/law-student:flashcards` |
| **Study Planner** | Long-term study plan with scheduled sessions, adaptive to session history | `law-student` | `/law-student:study-plan` |
| **Skill Registry Browser** | Search watched registries for community legal skills | `legal-builder-hub` | `/legal-builder-hub:registry-browser` |
| **Skill Installer** | Install a community skill with trust checks and skills-QA | `legal-builder-hub` | `/legal-builder-hub:skill-installer` |
| **Skill QA** | Evaluate a skill against the Legal Skill Design Framework | `legal-builder-hub` | `/legal-builder-hub:skills-qa` |
| **Community Skill Recommender** | Suggest community skills based on recent activity in other plugins | `legal-builder-hub` | `/legal-builder-hub:related-skills-surfacer` |
| **Community Skill Updater** | Check for updates to installed community skills | `legal-builder-hub` | `/legal-builder-hub:auto-updater` |
| **Registry Sync** | Periodic check of watched registries for new and updated skills | `legal-builder-hub` | scheduled agent |

For Managed Agent deployment — `agent.yaml`, leaf-worker subagents, steering-event examples, and per-agent security notes — see **[managed-agent-cookbooks/](./managed-agent-cookbooks)**.

*Section quoted from the upstream readme.*
Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

# Contributing to Claude for Legal

Notes for anyone writing or editing a plugin in this project. Keep this short — the
design principles that matter most for the quality of the output, not a style
guide.

## Before your first PR

Sign the CLA. The first time you open a pull request, the CLA Assistant bot will
comment with a link to the [CLA](CLA.md) and ask you to confirm. Reply with
`I have read the CLA Document and I hereby sign the CLA` and the check will pass.
You only need to do this once.

## Design principle: SKILL.md encodes the right behavior; CLAUDE.md guardrails
are the net

Every plugin in this project ships with two layers of instruction:

1. **`<plugin>/skills/<skill>/SKILL.md`** — what this specific skill does, step by
   step. The narrow, task-specific scaffold.
2. **`<plugin>/CLAUDE.md`** — the shared guardrails and the practice profile.
   "Scaffolding, not blinders," source-tag discipline, "verify user-stated legal
   facts," premise verification, destination check, cross-skill severity floor,
   pre-flight citation banner. The wide, plugin-level safety net.

**If a skill's correct output depends on a CLAUDE.md guardrail catching a
mistake the SKILL.md would have made, that's a design smell.** The SKILL.md
should tell the model what to do directly; the guardrails should catch what the
SKILL.md missed. Every time a guardrail has to rescue a skill, we're relying on
the guardrail firing consistently — and on a bad run, a weaker model, a terser
prompt, or a future editor who reads only the skill text, the rescue doesn't
happen.

**Rule of thumb: if a QA test passes only because a guardrail fired, add the
behavior to the SKILL.md directly.** The guardrail stays (belt and suspenders),
but the skill now carries the knowledge it needs on its own.

Examples of this rule in practice:

- A design patent question should not pass an infringement triage only because
  "Scaffolding, not blinders" lets the model override the utility-patent
  workflow. The skill should branch on the D-prefix itself and route to the
  ordinary-observer test.
- A renewal cancel-by date that falls on a Sunday should not land on the user's
  calendar correctly only because the user thought to ask about weekdays. The
  register schema and the Mode 2 output should carry the business-day roll-back
  themselves.
- An FLSA back-pay computation should not get the regular-rate formula right
  only because the model happens to remember §207(e). The skill should have a
  §207(e) checklist

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: Apache-2.0** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text

                                 Apache License
                           Version 2.0, January 2004
                        http://www.apache.org/licenses/

   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION

   1. Definitions.

      "License" shall mean the terms and conditions for use, reproduction,
      and distribution as defined by Sections 1 through 9 of this document.

      "Licensor" shall mean the copyright owner or entity authorized by
      the copyright owner that is granting the License.

      "Legal Entity" shall mean the union of the acting entity and all
      other entities that control, are controlled by, or are under common
      control with that entity. For the purposes of this definition,
      "control" means (i) the power, direct or indirect, to cause the
      direction or management of such entity, whether by contract or
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original Apache-2.0 terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `Apache-2.0` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `LEGAL` (category: LEGAL TECH)
- **Upstream URL:** https://github.com/anthropics/claude-for-legal
- **Pinned commit (SHA):** `4a6c651889c97cc9140580363c73e0eb17379c2b`
- **Branch:** main
- **Pin provenance:** GitHub API commits/main. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`68c681e3d3736a948ed89ccfad3403ec1e187247608b9bc5681229211bb28dfb`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

