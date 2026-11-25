# Reconciled Revision-Pinned Hebrew & Biblical Aramaic (MT OT) Evidence & Contextual-Review Ledger (v2.0 — Strict 5-Tier Taxonomy)

- **Date:** 2026-11-25 (Evidence & Reporting Reconciliation; **0** Bible verse-text, note, mapping, or Studio changes)
- **Adopted Source Corpus:** Saints-Hebrew-Critical-Text (Studio v10 Stage 1 `a0d022c1`, MAM Aleppo + WLC Leningrad, 39 books / 929 ch / 23,213 native MT vv)
- **Pinned Text / Mapping Commit SHA:** `f5014e214d27c15adc094bcddecda40a721c9b29`
- **Revision Chain Audited:** `71ea4f44` → `206d2445` → `57f6d108` → `915915e6` → `b3e0f2ea` → `00ff8636` → `6fe3807e` → `c659f8e6` → `c5376e6b` → `e2f4b634` → `f5014e21` (0 Bible text/note/mapping changes in evidence reconciliation)
- **Studio DB Snapshot:** `data/studio.db` (`seed_version = 10`, SHA-256 `23f39dbdcbc4599b1ed783bfce8a0b6268610e5dde6c200e114057798e64761d`)
- **Machine-Readable Ledgers:** `followup_contextual_review_ledger.json` & `scratch/followup/hebrew_contextual_ledger.jsonl` (`2,559` deduplicated citations retained after removing `0` exact duplicates)

## 1. Strict 5-Tier Evidence Totals (Each Native Reference Counted Once at Strongest Level)

> **Standard Applied Uniformly Across All Three Editions:** A passage is credited as `full_source_in_context_read` **only** where surviving evidence proves the reviewer compared its English against the adopted source in the surrounding paragraph, speech, or literary unit. Note checks, mapping checks, and isolated wording checks are classified under `targeted_evidence` (with explicit subtype counts and overlap). Batch scans, zero-change book claims, and unexpanded multi-verse issue-title ranges are strictly excluded. An earlier read supports the final revision **only** after programmatically confirming that the reviewed source text, English text, and relevant surrounding context (`±2` native verses / exact Pass 3.5 blind packet context) match final `HEAD` byte-for-byte.

| Strongest Documented Evidence Level | Distinct Native Verses | Share | Supports Final Revision (`true`) | Historical Only (`false`) | Strict Whole-Chapter Final Match |
|---|---:|---:|---:|---:|---:|
| **`full_source_in_context_read`** | **40** | **0.17%** | **37** | **3** | 36 |
| **`targeted_evidence`** *(note / mapping / isolated wording)* | **1,085** | **4.67%** | **1,053** | **32** | — |
| **`english_only_read`** *(Pass 3 standalone English)* | **949** | **4.09%** | **945** | **4** | — |
| **`automated_screening_only`** | **21,139** | **91.07%** | 21,139 | 0 | — |
| **`insufficient_evidence`** | **0** | **0.00%** | 0 | 0 | — |
| **TOTAL (`source_total` — exact partition)** | **23,213** | **100.00%** | — | — | — |

*Separate Editorial Status (NEVER merged with evidence depth): `verified` = **22,971**, `disputed` / `awaiting_human_signoff` = **242**, `unverified` = **0** (`22,971 + 242 = 23,213`).*

### Targeted Evidence Breakdown & Subtype Overlap

| Disjoint Targeted-Tier Subset | Distinct Native Verses | Share of Targeted Tier |
|---|---:|---:|
| `note_check` only | 179 | 16.50% |
| `mapping_check` only | 10 | 0.92% |
| `isolated_wording_check` only | 618 | 56.96% |
| `note_check` + `mapping_check` | 87 | 8.02% |
| `note_check` + `isolated_wording_check` | 115 | 10.60% |
| `mapping_check` + `isolated_wording_check` | 41 | 3.78% |
| `note_check` + `mapping_check` + `isolated_wording_check` | 35 | 3.23% |
| **TOTAL (`targeted_evidence` strongest tier)** | **1,085** | **100.00%** |

- **Targeted-tier check totals (non-disjoint across subtypes):** `note_check = 416`, `mapping_check = 173`, `isolated_wording_check = 809`, **multi-subtype overlap (`2+` subtypes) = `278`** (of which `note ∩ map = 122`).
- **Gross corpus-wide checks (including overlaps on `full_source_in_context_read` passages):** `note_check = 421` (`5` also in full), `mapping_check = 176` (`3` also in full), `isolated_wording_check = 814` (`5` also in full), `english_only_read = 1,019` (`4` also in full, `66` also in targeted).

## 2. Biblical Aramaic 5-Tier Evidence Breakdown (`269` Native MT Verses)

| Pericope | Book | `source_total` | `full_src_ctx` *(fin/hist)* | `targeted` *(fin/hist)* | `tgt_note` | `tgt_map` | `tgt_word` | `tgt_ov2+` | `eng_only` | `auto_only` | `insuff_ev` |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| `Gen 31:47` | Genesis | 1 | 0 (0/0) | 0 (0/0) | 0 | 0 | 0 | 0 | 1 | 0 | 0 |
| `Ezra 4:8–6:18` | Ezra | 52 | 1 (1/0) | 3 (3/0) | 0 | 0 | 3 | 0 | 0 | 48 | 0 |
| `Ezra 7:12–26` | Ezra | 15 | 0 (0/0) | 2 (2/0) | 0 | 0 | 2 | 0 | 0 | 13 | 0 |
| `Jer 10:11` | Jeremiah | 1 | 0 (0/0) | 0 (0/0) | 0 | 0 | 0 | 0 | 0 | 1 | 0 |
| `Dan 2:4–7:28` | Daniel | 200 | 2 (2/0) | 26 (26/0) | 18 | 10 | 20 | 15 | 25 | 147 | 0 |
| **TOTAL (5 Pericopes)** | — | **269** | **3** (3/0) | **31** (31/0) | **18** | **10** | **25** | **15** | **26** | **209** | **0** |

## 3. Reclassification Audit (Previous Follow-Up Ledger → Strict 5-Tier Ledger)

| Previous Ledger Class → Reconciled 5-Tier Class | Distinct Native Verses | Explanation |
|---|---:|---|
| `old_auto_only -> automated_screening_only` | 21,095 | Unchanged automated screening only |
| `old_auto_only -> targeted_evidence` | 53 | Newly captured from follow-up verified mapping/note audit or net-new Greek NT bracketed audit |
| `old_doc_src_ctx -> automated_screening_only` | 44 | Pruned batch scan reconstruction, zero-change prose claim, or unexpanded issue-title range |
| `old_doc_src_ctx -> english_only_read` | 10 | Pruned unverified source-check claim; retains documented Pass 3 standalone English-only read |
| `old_doc_src_ctx -> full_source_in_context_read` | 40 | Confirmed genuine full source-in-context read (Pass 3.5 blind review or recovered Greek helper range) |
| `old_doc_src_ctx -> targeted_evidence` | 1,031 | Reclassified from undifferentiated prior bucket into targeted note / mapping / isolated wording check |
| `old_p3_eng_only -> english_only_read` | 939 | Retained as Pass 3 standalone English-only read |
| `old_p3_eng_only -> targeted_evidence` | 1 | Upgraded via follow-up verified note/mapping audit |

### Pruned Batch Scans, Zero-Change Prose Claims & Issue-Title Ranges

- `corr24_readme_open_item_range_scope`: **56** rows removed from per-verse credit
- `pass35_heb_1kgs7_masger_batch_range`: **9** rows removed from per-verse credit
- `stage2-pass1_HEB-HQ-027_issue_title_range`: **9** rows removed from per-verse credit
- `stage2-pass1_HEB-HQ-028_issue_title_range`: **13** rows removed from per-verse credit
- `stage2-pass1_HEB-HQ-034_issue_title_range`: **4** rows removed from per-verse credit
- `stage2-pass2_HEB-HQ-027_issue_title_range`: **9** rows removed from per-verse credit
- `stage2-pass2_HEB-HQ-028_issue_title_range`: **13** rows removed from per-verse credit
- `stage2-pass2_HEB-HQ-034_issue_title_range`: **4** rows removed from per-verse credit

## 4. Unique Native Verses by Pass & Evidence Class

| Pass | Evidence Class | Unique Native Verses |
|---|---|---:|
| `followup_mapping_audit` | `targeted_evidence` | 74 |
| `followup_note_audit` | `targeted_evidence` | 75 |
| `pre-stage2-corr24-verse-review` | `targeted_evidence` | 781 |
| `stage2-pass1` | `targeted_evidence` | 171 |
| `stage2-pass2` | `targeted_evidence` | 145 |
| `stage2-pass3-standalone-flow` | `english_only_read` | 1,019 |
| `stage2-pass35-response` | `targeted_evidence` | 29 |
| `stage2-pass3b-bounceback` | `targeted_evidence` | 106 |
| `stage2-pass4-bounceback` | `targeted_evidence` | 10 |
| `stage2-pass4-reconciliation` | `targeted_evidence` | 103 |
| `stage2_pass35_blind_ai_peer_review` | `full_source_in_context_read` | 40 |

## 5. Unassigned Aggregate Claims & Batch Scans (`0` Verses Assigned)

- **`UAC-HEB-01`** (`corrections/2026-11-24-modern-english-fidelity/README.md`, claimed `23,167`): No per-verse reading log for unchanged verses; plus 412 edition-wide consistency/note batch rows (380 unique MT verses) strictly excluded.
- **`UAC-HEB-02`** (`reviews/2026-11-24-literal-smooth/pass1_summary.md:L113-L115`, claimed `269`): Unlogged aggregate claim of 100% line-by-line Aramaic read (subtotals corrected to 52+15+200+1+1=269); only individually evidenced Aramaic verses receive credit.
- **`UAC-HEB-03`** (`reviews/2026-11-24-literal-smooth/pass1_summary.md:L102`, claimed `118`): 83 alignment + 35 length outliers without saved per-verse log.
- **`UAC-HEB-04`** (`reviews/2026-11-24-literal-smooth/pass1_summary.md:L106-L109,L122`, claimed `1,417`): Aggregate pattern sweeps (yam-suf, Judges 10-11, 932 Ketiv/Qere, 12 QwK, 131 superscriptions, 310 version notes) without per-verse read logs.
- **`UAC-HEB-05`** (`pass1_coverage.json & pass2_coverage.json`, claimed `22,971`): Editorial disposition totals kept strictly separate from reading evidence.
- **`UAC-HEB-06`** (`pass3_bounceback_verdicts.jsonl (P3B-003,008,009,011,012,013)`, claimed `569`): Multi-chapter quotation-frame boundary checks; only explicitly cited/edited boundary and inner-quote verses receive targeted_evidence credit.
- **`UAC-HEB-07`** (`scratch/reconciliation/pass4_summary.md & pass35_ai_peer_review_response.jsonl`, claimed `33,776`): Programmatic cross-edition triage and Pass 3.5 batch lexical scans (21 masger* incl. unenumerated 1 Kgs 7:28-36, 18 Exodus terms); only individually verified/cited verses receive targeted_evidence credit.
- **`UAC-HEB-08`** (`corr24 README.md Open Items & pass1/2_human_editor_queue.jsonl`, claimed `95`): Unexpanded issue-title / open-item ranges (Isa 11:1-10, 42:1-4, 49:1-7, 50:4-10, 52:13-53:12, Mic 5:1-5, Exod 23:20-23, Deut 32:28-34, Num 26:15-47, Ezek 7:3-10); only specific individually cited/anchored verses receive targeted_evidence credit.

## 6. Complete Per-Book 5-Tier Evidence Breakdown (39 Books, Summing to `23,213`)

| # | Book | Ch | `source_total` | `full_src_ctx` *(fin / hist)* | `targeted` *(fin / hist)* | `tgt_note` | `tgt_map` | `tgt_word` | `tgt_ov2+` | `eng_only` | `auto_only` | `insuff_ev` | Ed. `verified` / `disputed` *(sep.)* |
|---:|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 1 | Genesis | 50 | 1,533 | 1 (1/0) | 44 (44/0) | 19 | 5 | 32 | 9 | 100 | 1,388 | 0 | 1,530 / 3 |
| 2 | Exodus | 40 | 1,213 | 3 (2/1) | 114 (113/1) | 30 | 30 | 89 | 31 | 61 | 1,035 | 0 | 1,173 / 40 |
| 3 | Leviticus | 27 | 859 | 2 (2/0) | 54 (54/0) | 9 | 2 | 48 | 4 | 37 | 766 | 0 | 855 / 4 |
| 4 | Numbers | 36 | 1,289 | 2 (2/0) | 52 (51/1) | 19 | 13 | 38 | 16 | 41 | 1,194 | 0 | 1,281 / 8 |
| 5 | Deuteronomy | 34 | 959 | 1 (1/0) | 50 (50/0) | 19 | 4 | 40 | 13 | 66 | 842 | 0 | 947 / 12 |
| 6 | Joshua | 24 | 658 | 0 (0/0) | 36 (36/0) | 11 | 11 | 32 | 16 | 32 | 590 | 0 | 655 / 3 |
| 7 | Judges | 21 | 618 | 2 (2/0) | 22 (22/0) | 2 | 0 | 22 | 2 | 30 | 564 | 0 | 618 / 0 |
| 8 | Ruth | 4 | 85 | 0 (0/0) | 3 (3/0) | 1 | 0 | 2 | 0 | 22 | 60 | 0 | 85 / 0 |
| 9 | 1 Samuel | 31 | 811 | 0 (0/0) | 14 (13/1) | 7 | 0 | 9 | 2 | 56 | 741 | 0 | 810 / 1 |
| 10 | 2 Samuel | 24 | 695 | 2 (2/0) | 16 (16/0) | 2 | 0 | 14 | 0 | 31 | 646 | 0 | 695 / 0 |
| 11 | 1 Kings | 22 | 817 | 2 (2/0) | 87 (64/23) | 48 | 64 | 52 | 64 | 46 | 682 | 0 | 817 / 0 |
| 12 | 2 Kings | 25 | 719 | 1 (1/0) | 17 (17/0) | 3 | 1 | 13 | 0 | 0 | 701 | 0 | 719 / 0 |
| 13 | 1 Chronicles | 29 | 943 | 1 (1/0) | 15 (15/0) | 5 | 0 | 10 | 0 | 0 | 927 | 0 | 942 / 1 |
| 14 | 2 Chronicles | 36 | 822 | 1 (1/0) | 26 (26/0) | 6 | 0 | 23 | 3 | 0 | 795 | 0 | 822 / 0 |
| 15 | Ezra | 10 | 280 | 1 (1/0) | 7 (7/0) | 2 | 0 | 6 | 1 | 0 | 272 | 0 | 280 / 0 |
| 16 | Nehemiah | 13 | 405 | 2 (1/1) | 14 (14/0) | 6 | 0 | 10 | 2 | 16 | 373 | 0 | 405 / 0 |
| 17 | Esther | 10 | 167 | 0 (0/0) | 11 (11/0) | 7 | 0 | 9 | 5 | 0 | 156 | 0 | 165 / 2 |
| 18 | Job | 42 | 1,070 | 3 (3/0) | 33 (33/0) | 16 | 0 | 23 | 6 | 42 | 992 | 0 | 1,040 / 30 |
| 19 | Psalms | 150 | 2,527 | 3 (3/0) | 103 (103/0) | 61 | 3 | 48 | 9 | 21 | 2,400 | 0 | 2,516 / 11 |
| 20 | Proverbs | 31 | 915 | 1 (0/1) | 32 (27/5) | 18 | 16 | 14 | 16 | 36 | 846 | 0 | 910 / 5 |
| 21 | Ecclesiastes | 12 | 222 | 0 (0/0) | 21 (21/0) | 4 | 0 | 17 | 0 | 22 | 179 | 0 | 221 / 1 |
| 22 | Song of Songs | 8 | 117 | 1 (1/0) | 6 (6/0) | 2 | 0 | 6 | 2 | 16 | 94 | 0 | 116 / 1 |
| 23 | Lamentations | 5 | 154 | 1 (1/0) | 5 (5/0) | 1 | 0 | 5 | 1 | 65 | 83 | 0 | 154 / 0 |
| 24 | Isaiah | 66 | 1,291 | 1 (1/0) | 58 (58/0) | 14 | 1 | 53 | 10 | 11 | 1,221 | 0 | 1,257 / 34 |
| 25 | Jeremiah | 52 | 1,364 | 3 (3/0) | 86 (85/1) | 37 | 5 | 62 | 18 | 38 | 1,237 | 0 | 1,331 / 33 |
| 26 | Ezekiel | 48 | 1,273 | 2 (2/0) | 51 (51/0) | 18 | 5 | 43 | 15 | 39 | 1,181 | 0 | 1,256 / 17 |
| 27 | Daniel | 12 | 357 | 2 (2/0) | 37 (37/0) | 23 | 10 | 31 | 20 | 25 | 293 | 0 | 337 / 20 |
| 28 | Hosea | 14 | 197 | 0 (0/0) | 9 (9/0) | 4 | 0 | 5 | 0 | 24 | 164 | 0 | 197 / 0 |
| 29 | Joel | 4 | 73 | 1 (1/0) | 1 (1/0) | 1 | 0 | 1 | 1 | 0 | 71 | 0 | 73 / 0 |
| 30 | Amos | 9 | 146 | 0 (0/0) | 3 (3/0) | 1 | 0 | 3 | 1 | 27 | 116 | 0 | 146 / 0 |
| 31 | Obadiah | 1 | 21 | 0 (0/0) | 0 (0/0) | 0 | 0 | 0 | 0 | 0 | 21 | 0 | 21 / 0 |
| 32 | Jonah | 4 | 48 | 0 (0/0) | 2 (2/0) | 1 | 0 | 1 | 0 | 10 | 36 | 0 | 48 / 0 |
| 33 | Micah | 7 | 105 | 0 (0/0) | 7 (7/0) | 4 | 0 | 6 | 3 | 0 | 98 | 0 | 99 / 6 |
| 34 | Nahum | 3 | 47 | 0 (0/0) | 2 (2/0) | 1 | 0 | 1 | 0 | 0 | 45 | 0 | 47 / 0 |
| 35 | Habakkuk | 3 | 56 | 1 (1/0) | 3 (3/0) | 3 | 0 | 0 | 0 | 17 | 35 | 0 | 56 / 0 |
| 36 | Zephaniah | 3 | 53 | 0 (0/0) | 2 (2/0) | 0 | 0 | 2 | 0 | 0 | 51 | 0 | 52 / 1 |
| 37 | Haggai | 2 | 38 | 0 (0/0) | 1 (1/0) | 1 | 0 | 0 | 0 | 0 | 37 | 0 | 38 / 0 |
| 38 | Zechariah | 14 | 211 | 0 (0/0) | 12 (12/0) | 5 | 0 | 11 | 4 | 8 | 191 | 0 | 206 / 5 |
| 39 | Malachi | 3 | 55 | 0 (0/0) | 29 (29/0) | 5 | 3 | 28 | 4 | 10 | 16 | 0 | 51 / 4 |
| — | **TOTAL (39 books)** | **929** | **23,213** | **40** (37/3) | **1,085** (1,053/32) | **416** | **173** | **809** | **278** | **949** | **21,139** | **0** | **22,971 / 242** |
