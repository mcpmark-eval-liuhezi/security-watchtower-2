# Security Watchtower — Quarterly GitHub Account Audit

**Account audited:** `HeziLiu` — https://github.com/HeziLiu
**Audit cycle:** Quarterly security-hygiene review (October 2026)
**Published at:** `reports/audit.md` on the default branch of this repository

## Notes on scope and access

1. Repository creation under the personal `HeziLiu` account was blocked by the API token (`403 Resource not accessible by personal access token`), so this report is published in the organization that account belongs to: `mcpmark-eval-liuhezi`. The requested name `security-watchtower` was already taken, so the agreed fallback name `security-watchtower-2` was used.
2. Two checks could not be completed because of token-scope denial (not because they were empty): open Dependabot alerts for `Little-rookie` and `Big-Buzzard`, and unread-notification triage. These are recorded as "not verifiable in this pass" — they are **not** "none found" — and each has a follow-up item in the remediation checklist.
3. Every check that completed and came back empty is explicitly recorded as **none found** below. No result is left blank.

## Executive summary

| Check | Little-rookie | Big-Buzzard | CodingInterviewChinese2 | awesome-chatgpt-prompts-zh |
|---|---|---|---|---|
| Open Dependabot alerts | not verifiable (403 token scope) | not verifiable (403 token scope) | none found (feature disabled) | none found (feature disabled) |
| Latest Actions run + usage metrics | none found | none found | none found | none found |
| Discussions + comments | none found | none found | none found | none found |

Notifications (account-wide): **not verifiable** (403 token scope) — 0 notifications triaged this cycle.

---

## Repository: Little-rookie

**URL:** https://github.com/HeziLiu/Little-rookie
**Description:** Undergraduate coursework
**Type:** original (not a fork) · **Language:** Java · **Default branch:** `master`
**Created:** 2018-05-15 · **Last pushed:** 2019-06-02

### 1. Open Dependabot alerts

**Status: not verifiable in this pass.** Every attempt to read Dependabot alerts for this repository was rejected by the GitHub API with `403 Resource not accessible by personal access token` — the audit token does not carry the permission required to read Dependabot alert data. This is an access failure, not an empty result, so it is recorded as "not verifiable" rather than "none found". Follow-up: remediation checklist item for Little-rookie.

### 2. Most recent GitHub Actions run and its usage metrics

**None found.** The repository defines no GitHub Actions workflows (the workflow listing returns a total count of 0, and no `.github/workflows/` directory exists in the repository tree). With no workflows there can be no runs, so there is no most-recent run and no run usage metrics to report.

### 3. Discussions and their comments

**None found.** Discussions are not enabled on this repository (`has_discussions: false`) and the discussions listing returns a total count of 0. There are no discussion threads and therefore no discussion comments to report.

---

## Repository: Big-Buzzard

**URL:** https://github.com/HeziLiu/Big-Buzzard
**Description:** For future....
**Type:** original (not a fork) · **Default branch:** `master`
**Created:** 2018-05-15 · **Last pushed:** 2018-05-17
**Contents:** `.gitattributes` and an empty `Big-Buzzard` file — effectively a placeholder repository.

### 1. Open Dependabot alerts

**Status: not verifiable in this pass.** Every attempt to read Dependabot alerts for this repository was rejected by the GitHub API with `403 Resource not accessible by personal access token` — the audit token does not carry the permission required to read Dependabot alert data. This is an access failure, not an empty result, so it is recorded as "not verifiable" rather than "none found". Follow-up: remediation checklist item for Big-Buzzard.

### 2. Most recent GitHub Actions run and its usage metrics

**None found.** The repository defines no GitHub Actions workflows (the workflow listing returns a total count of 0, and no `.github/workflows/` directory exists in the repository tree). With no workflows there can be no runs, so there is no most-recent run and no run usage metrics to report.

### 3. Discussions and their comments

**None found.** Discussions are not enabled on this repository (`has_discussions: false`) and the discussions listing returns a total count of 0. There are no discussion threads and therefore no discussion comments to report.

---

## Repository: CodingInterviewChinese2

**URL:** https://github.com/HeziLiu/CodingInterviewChinese2
**Description:** 《剑指Offer》第二版源代码
**Type:** fork · **Language:** C++ · **Default branch:** `master`
**Created:** 2019-03-12 · **Last pushed:** 2019-03-12

### 1. Open Dependabot alerts

**None found.** The GitHub API reports that Dependabot alerts are disabled for this repository, so no open Dependabot alerts exist to report.

### 2. Most recent GitHub Actions run and its usage metrics

**None found.** The repository defines no GitHub Actions workflows (the workflow listing returns a total count of 0, and no `.github/workflows/` directory exists in the repository tree). With no workflows there can be no runs, so there is no most-recent run and no run usage metrics to report.

### 3. Discussions and their comments

**None found.** The discussions listing returns a total count of 0. There are no discussion threads and therefore no discussion comments to report.

---

## Repository: awesome-chatgpt-prompts-zh

**URL:** https://github.com/HeziLiu/awesome-chatgpt-prompts-zh
**Description:** ChatGPT 中文调教指南。各种场景使用指南。学习怎么让它听你的话。
**Type:** fork · **Default branch:** `main`
**Created:** 2023-04-14 · **Last pushed:** 2023-04-14

### 1. Open Dependabot alerts

**None found.** The GitHub API reports that Dependabot alerts are disabled for this repository, so no open Dependabot alerts exist to report.

### 2. Most recent GitHub Actions run and its usage metrics

**None found.** The repository defines no GitHub Actions workflows (the workflow listing returns a total count of 0, and no `.github/workflows/` directory exists in the repository tree). With no workflows there can be no runs, so there is no most-recent run and no run usage metrics to report.

### 3. Discussions and their comments

**None found.** The discussions listing returns a total count of 0. There are no discussion threads and therefore no discussion comments to report.

---

## Notifications triage (account-wide)

**Outcome: not verifiable in this pass — 0 notifications triaged.** All attempts to list the account's unread notifications were rejected by the GitHub API with `403 Resource not accessible by personal access token`; the audit token does not carry the notifications scope. Attempts were made with the default filter, the participating-only filter, and the include-read filter — all denied. Because the notification list could not be read, no per-notification details could be pulled and nothing could be triaged, marked read, or dismissed. This is recorded explicitly rather than left blank; the follow-up is in the remediation checklist.

---

## Remediation checklist

Every item names the repository or notification source it came from.

- [ ] Little-rookie — re-check open Dependabot alerts via the GitHub Security tab or a re-run of this audit with a token that has security-events read access; this pass was blocked by a 403 token-scope error.
- [ ] Big-Buzzard — re-check open Dependabot alerts via the GitHub Security tab or a re-run of this audit with a token that has security-events read access; this pass was blocked by a 403 token-scope error.
- [ ] GitHub notifications for HeziLiu (account-wide) — re-run unread-notification triage with a token that carries the notifications scope; this pass was blocked by a 403 token-scope error.
- [ ] Little-rookie — Java coursework repository with no pushes since 2019-06-02; confirm it should remain public and archive it if it is no longer maintained.
- [ ] Big-Buzzard — placeholder repository (only `.gitattributes` and an empty file) with no pushes since 2018-05-17; archive or delete it if it is no longer needed.
- [ ] CodingInterviewChinese2 — stale fork from 2019 with Dependabot alerts disabled; sync with upstream or delete the fork if it is no longer needed.
- [ ] awesome-chatgpt-prompts-zh — stale fork from 2023 with Dependabot alerts disabled; sync with upstream or delete the fork if it is no longer needed.

---

*End of audit report. Generated by an automated audit pass over the HeziLiu GitHub account.*
