# Follow-Up Audit — Revision-Pinned Hebrew/Aramaic Contextual-Review & Post-Edit Reread Ledger

- **Edition:** Hebrew & Biblical Aramaic (`Hebrew-Translation/Modern-English-OT/`)
- **Pinned Source Critical Text:** `Saints-Hebrew-Critical-Text` Studio v10 Stage 1 (`a0d022c1`, MAM Aleppo + WLC Leningrad)
- **Pinned English Verse-Text Revision:** `e2f4b6343783ee497a07d3ddd29b65778b7809b8` (follow-up commit makes note-attachment/README fixes only; **0** verse-text changes)
- **Machine-Readable Ledger:** `followup_contextual_review_ledger.json` and `scratch/followup/hebrew_contextual_ledger.jsonl` (**1,502** deduplicated pass-read events across **1,125** unique MT verses)

## 1. Strict Honesty Policy & Evidence vs. Editorial Status

Evidence categories (`documented_contextual_read`, `automated_screening_only`, `insufficient_evidence`) are kept **strictly separate** from editorial disposition statuses (`verified`, `disputed`, `awaiting_human_signoff`). Unattributed aggregate claims (including the unlogged `corr24` 23,167 claim and Pass 1's unlogged 269-verse Aramaic claim), batch `edition-wide` standardization replacements (`412` rows), wide speech-frame boundary scans, and standalone English-only Pass 3 reads (`@heb-flow`) are **excluded** from `documented_contextual_read` and reported explicitly below.

| Scope | Source Total | `documented_contextual_read` | `automated_screening_only` | `insufficient_evidence` | Documented % |
|---|---:|---:|---:|---:|---:|
| **Full MT Corpus (39 books / 929 chs)** | **23,213** | **1,125** | **22,088** | **0** | **4.85%** |
| **Biblical Aramaic (5 pericopes)** | **269** | **33** | **236** | **0** | **12.27%** |

**Editorial Disposition Status at `e2f4b634` (strictly separate from evidence categories):** `22,971` `verified`, `242` `disputed` (`44` items in `pass2_human_editor_queue.jsonl` awaiting human editor sign-off), `0` `unverified`.

### Ledger Contributions by Source-Checked Pass

| Pass | Reviewer | English Revision | Deduplicated Read Events | Unique MT Verses |
|---|---|---|---:|---:|
| `pre-stage2-corr24-verse-review` | `claude-2026-11-24-fidelity-review` | `71ea4f44` | 837 | 837 |
| `stage2-pass1` | `heb-fidelity` | `206d2445` | 197 | 197 |
| `stage2-pass2` | `heb-peer` | `57f6d108` | 171 | 171 |
| `stage2-pass3b-bounceback` | `heb-peer` | `b3e0f2ea` | 106 | 106 |
| `stage2-pass35-blind-ai-peer-review` | `heb-ai-peer` | `00ff8636` | 40 | 40 |
| `stage2-pass35-response` | `heb-peer` | `6fe3807e` | 38 | 38 |
| `stage2-pass4-reconciliation` | `reconciler` | `c659f8e6` | 103 | 103 |
| `stage2-pass4-bounceback` | `heb-peer` | `c5376e6b` | 10 | 10 |
| **Combined Deduplicated Total** | — | — | **1,502** | **1,125** |

## 2. Biblical Aramaic 3-Way Evidence Breakdown (269 Verses)

| Pericope | Book | Source Total | `documented_contextual_read` | `automated_screening_only` | `insufficient_evidence` |
|---|---|---:|---:|---:|---:|
| `Gen 31:47` | Genesis | 1 | 0 | 1 | 0 |
| `Ezra 4:8-6:18` | Ezra | 52 | 4 | 48 | 0 |
| `Ezra 7:12-26` | Ezra | 15 | 2 | 13 | 0 |
| `Jer 10:11` | Jeremiah | 1 | 0 | 1 | 0 |
| `Dan 2:4-7:28` | Daniel | 200 | 27 | 173 | 0 |
| **Total (5 Pericopes)** | — | **269** | **33** | **236** | **0** |

## 3. Unattributed Aggregate Claims & Non-Source-Checked / Batch Records

### A. Unattributed Aggregate Claims (NOT assigned to individual verses)

- **`UAC-HEB-01`** (`corrections/2026-11-24-modern-english-fidelity/README.md:L4,L23`): claimed **23,167** (All 23,167 English verse units (52 parallel reviewers covering ~450 verses each against MT Hebrew/Aramaic)). Only changed verses (581 verse-review rows + 88 structural rows) and named open items were logged individually; unchanged verses have no per-verse read receipt or reviewer sign-off log. *Disposition:* Individual unlogged verses remain classified as automated_screening_only.
- **`UAC-HEB-02`** (`reviews/2026-11-24-literal-smooth/pass1_summary.md:L113-L114; pass1_coverage.json:L63`): claimed **269** (All 5 Biblical Aramaic pericopes (269 verses — '100% Line-by-Line Read')). Original Pass 1 summary mis-stated pericope subtotals (Ezra 4:8-6:18 as 67 instead of 52; Dan 2:4-7:28 as 185 instead of 200) and recorded no verse-by-verse contextual read log for unmentioned Aramaic verses. *Disposition:* Only the 33 Aramaic verses with individually documented source-checked records are classified as documented_contextual_read; the remaining 236 remain automated_screening_only.
- **`UAC-HEB-03`** (`reviews/2026-11-24-literal-smooth/pass1_summary.md:L102`): claimed **118** (Low-alignment outliers (83 vv) & length-ratio outliers (35 vv) — 'All 118 manually read against MT Hebrew'). Individual verse references for the 118 outlier verses were not saved to a file. *Disposition:* Unlogged outlier verses remain automated_screening_only.
- **`UAC-HEB-04`** (`reviews/2026-11-24-literal-smooth/pass1_summary.md:L106-L109,L122`): claimed **1,417** (24 yam-suf occurrences, 8 Judges 10-11 occurrences, 932 Ketiv/Qere verses, 12 Qere-wela-Ketiv verses, 131 Psalm/Habakkuk superscriptions, 310 ancient-version notes). Reported as aggregate pattern/sweep totals; only individually named verses (e.g., 2 Sam 18:20, Ruth 3:17, Ps 16:1/45:1/60:1/74:1/78:1/69:1/80:1) have per-verse records. *Disposition:* Only explicitly named verses enter documented_contextual_read; aggregate sweep totals remain automated_screening_only.
- **`UAC-HEB-05`** (`reviews/2026-11-24-literal-smooth/pass1_coverage.json; pass2_coverage.json`): claimed **22,971** (Editorial coverage totals: Pass 1 verified=22,906; Pass 2 verified=23,008 -> 22,972 -> 22,971 (disputed=242, unverified=0)). Editorial disposition status ('verified' vs 'disputed') combined automated screening and targeted contextual review; it is NOT an individually logged verse-by-verse contextual read ledger. *Disposition:* Kept strictly separate under editorial_status_at_e2f4b634; evidence classification uses only individually documented reads.
- **`UAC-HEB-06`** (`reviews/2026-11-24-literal-smooth/pass3_bounceback_verdicts.jsonl (P3B-003, P3B-008, P3B-009, P3B-011, P3B-012, P3B-013)`): claimed **569** (Multi-chapter speech-frame quotation verification across Exod 21:1-23:33, Exod 25:1-30:10, Lev 1-3/4-5/6:17-7:21/25-26, Num 28:1-29:39, Job 28 & 30-31). Verified speaker-formula and inner-quotation boundaries across those chapters rather than verse-by-verse translation fidelity of every interior verse. *Disposition:* Only the specific boundary, inner-quote, and edited verses explicitly cited in source_verification / applied_changes are entered in documented_contextual_read.
- **`UAC-HEB-07`** (`scratch/reconciliation/pass4_summary.md`): claimed **33,776** (Cross-edition programmatic comparison across 33,776 1:1 slots, 41 OT cardinal number mismatches, and 46 OT polarity checks). Programmatic cross-edition triage; only the 99 Hebrew-bearing rows individually logged in pass4_reconciliation.jsonl (plus 8 Pass 4 bounce-backs) have documented contextual verification. *Disposition:* Only verses individually logged in pass4_reconciliation.jsonl and pass4_bounceback_verdicts.jsonl enter documented_contextual_read.

### B. Batch & Standalone English-Only Records (Excluded from source-checked `documented_contextual_read`)

- **`corr24` `edition-wide` standardization passes:** `412` rows across `380` unique MT verses (`345` not already in `documented_contextual_read`).
- **Stage 2 Pass 3 standalone English review (`@heb-flow` @ `915915e6`):** `11` Bucket A surface edits, `14` Bucket B bounce-backs, and `32` named standalone chapters (`1,010` MT verses) — zero Hebrew/Aramaic inspection.

## 4. Post-Edit Reread Audit (`71ea4f44` / `206d2445` → `e2f4b634` + Follow-Up Note Fixes)

- **Total MT verses with verse-text change (`71ea4f44..HEAD`):** **165** (0 verse-text changes in `c5376e6b`, `e2f4b634`, or follow-up commit)
  - **`text_reread_on_final_revision = true`:** **19** (independently contextually reread AFTER their final text edit commit; verse text at reread SHA is byte-identical to `e2f4b634`/HEAD)
  - **`text_reread_on_final_revision = false`:** **146** (not independently reread against Hebrew/Aramaic after their final text edit commit — breakdown by last text-edit SHA: `{'b3e0f2ea': 53, '6fe3807e': 4, '57f6d108': 78, '915915e6': 11}`)
  - *Note:* All **11** Pass 3 Bucket A verses (`915915e6`), all **4** Pass 3.5 expansion verses (`Exod 36:34, 39:33, 39:39, 40:11` in `6fe3807e`), and un-sampled Pass 2 (`57f6d108`) / Pass 3B (`b3e0f2ea`) verses have `text_reread_on_final_revision: false` until independently reread on final text.
- **Total MT verses with ANY text or note change (incl. follow-up note-attachment fixes):** **281** (incl. **75** follow-up note-attachment updates pending `@followup-verifier` verification)
  - **`reread_on_final_revision = true` (strict final state incl. notes):** **37** | **`false`:** **244**

## 5. Per-Book 3-Way Evidence Coverage (All 39 MT Books)

| # | Book | Source Total | `documented_contextual_read` | `automated_screening_only` | `insufficient_evidence` | Doc % | Editorial `verified` / `disputed` |
|---:|---|---:|---:|---:|---:|---:|---|
| 1 | Genesis | 1,533 | 45 | 1,488 | 0 | 2.94% | 1,530 / 3 |
| 2 | Exodus | 1,213 | 117 | 1,096 | 0 | 9.65% | 1,173 / 40 |
| 3 | Leviticus | 859 | 56 | 803 | 0 | 6.52% | 855 / 4 |
| 4 | Numbers | 1,289 | 54 | 1,235 | 0 | 4.19% | 1,281 / 8 |
| 5 | Deuteronomy | 959 | 51 | 908 | 0 | 5.32% | 947 / 12 |
| 6 | Joshua | 658 | 36 | 622 | 0 | 5.47% | 655 / 3 |
| 7 | Judges | 618 | 24 | 594 | 0 | 3.88% | 618 / 0 |
| 8 | Ruth | 85 | 3 | 82 | 0 | 3.53% | 85 / 0 |
| 9 | 1 Samuel | 811 | 14 | 797 | 0 | 1.73% | 810 / 1 |
| 10 | 2 Samuel | 695 | 18 | 677 | 0 | 2.59% | 695 / 0 |
| 11 | 1 Kings | 817 | 95 | 722 | 0 | 11.63% | 817 / 0 |
| 12 | 2 Kings | 719 | 17 | 702 | 0 | 2.36% | 719 / 0 |
| 13 | 1 Chronicles | 943 | 16 | 927 | 0 | 1.70% | 942 / 1 |
| 14 | 2 Chronicles | 822 | 27 | 795 | 0 | 3.28% | 822 / 0 |
| 15 | Ezra | 280 | 8 | 272 | 0 | 2.86% | 280 / 0 |
| 16 | Nehemiah | 405 | 15 | 390 | 0 | 3.70% | 405 / 0 |
| 17 | Esther | 167 | 11 | 156 | 0 | 6.59% | 165 / 2 |
| 20 | Job | 1,070 | 36 | 1,034 | 0 | 3.36% | 1,040 / 30 |
| 21 | Psalms | 2,527 | 78 | 2,449 | 0 | 3.09% | 2,516 / 11 |
| 22 | Proverbs | 915 | 33 | 882 | 0 | 3.61% | 910 / 5 |
| 23 | Ecclesiastes | 222 | 21 | 201 | 0 | 9.46% | 221 / 1 |
| 24 | Song of Songs | 117 | 7 | 110 | 0 | 5.98% | 116 / 1 |
| 25 | Lamentations | 154 | 6 | 148 | 0 | 3.90% | 154 / 0 |
| 28 | Isaiah | 1,291 | 97 | 1,194 | 0 | 7.51% | 1,257 / 34 |
| 29 | Jeremiah | 1,364 | 70 | 1,294 | 0 | 5.13% | 1,331 / 33 |
| 30 | Ezekiel | 1,273 | 56 | 1,217 | 0 | 4.40% | 1,256 / 17 |
| 31 | Daniel | 357 | 38 | 319 | 0 | 10.64% | 337 / 20 |
| 32 | Hosea | 197 | 9 | 188 | 0 | 4.57% | 197 / 0 |
| 33 | Joel | 73 | 2 | 71 | 0 | 2.74% | 73 / 0 |
| 34 | Amos | 146 | 3 | 143 | 0 | 2.05% | 146 / 0 |
| 35 | Obadiah | 21 | 0 | 21 | 0 | 0.00% | 21 / 0 |
| 36 | Jonah | 48 | 2 | 46 | 0 | 4.17% | 48 / 0 |
| 37 | Micah | 105 | 10 | 95 | 0 | 9.52% | 99 / 6 |
| 38 | Nahum | 47 | 2 | 45 | 0 | 4.26% | 47 / 0 |
| 39 | Habakkuk | 56 | 4 | 52 | 0 | 7.14% | 56 / 0 |
| 40 | Zephaniah | 53 | 2 | 51 | 0 | 3.77% | 52 / 1 |
| 41 | Haggai | 38 | 1 | 37 | 0 | 2.63% | 38 / 0 |
| 42 | Zechariah | 211 | 12 | 199 | 0 | 5.69% | 206 / 5 |
| 43 | Malachi | 55 | 29 | 26 | 0 | 52.73% | 51 / 4 |
| — | **TOTAL (39 MT Books)** | **23,213** | **1,125** | **22,088** | **0** | **4.85%** | **22,971 / 242** |
