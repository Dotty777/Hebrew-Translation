# Follow-Up Audit — Exact Biblical Aramaic Recount & Subtotals Correction

- **Source Authority:** `Saints-Hebrew-Critical-Text` (Studio v10 Stage 1 `a0d022c1`, MAM Aleppo + WLC Leningrad), cross-checked against `Saints-Critical-Text-Studio/data/studio.db` (`stream_tokens` `lang='arc'`, read-only).
- **Correction Applied:** Fixed the sole erroneous `67` / `185` subtotal entry in `reviews/2026-11-24-literal-smooth/pass1_summary.md` (line 114) with an explicit erratum. Exhaustive repository grep confirmed **0** other erroneous `67`/`185` Aramaic subtotals in `Hebrew-Translation` (`AUDIT.md:104` and `ezra/README.md:8` validly count `67` combined Ezra `[Aramaic]` legacy tags = `52 + 15`; `AUDIT.md` `185` refers to legacy archive gaps).

## 1. Exact Verified Pericope Counts (Source Inventory vs. Documented Contextual Review)

| Pericope | Book | Exact Source Count | Chapter Breakdown | Notes | `documented_contextual_read` | `automated_screening_only` |
|---|---|---:|---|---|---:|---:|
| `Gen 31:47` | Genesis | **1** | ch. 31: 1 | mixed_hebrew_aramaic_two_words | **0** | 1 |
| `Ezra 4:8-6:18` | Ezra | **52** | ch. 4: 17, ch. 5: 17, ch. 6: 18 | aramaic | **4** | 48 |
| `Ezra 7:12-26` | Ezra | **15** | ch. 7: 15 | aramaic | **2** | 13 |
| `Jer 10:11` | Jeremiah | **1** | ch. 10: 1 | aramaic | **0** | 1 |
| `Dan 2:4-7:28` | Daniel | **200** | ch. 2: 46, ch. 3: 33, ch. 4: 34, ch. 5: 30, ch. 6: 29, ch. 7: 28 | mixed_at_2_4b_then_aramaic | **27** | 173 |
| **TOTAL (5 Pericopes)** | — | **269** | `52 + 15 = 67` Ezra; `200` Dan; `1` Gen; `1` Jer | 267 wholly Aramaic + 2 mixed (`Gen 31:47`, `Dan 2:4b`) | **33** | **236** |

## 2. Source Inventory (`269`) vs. Documented Contextual Review (`33`)

- **Source inventory total:** **269** MT verses across 5 pericopes (`1 + 52 + 15 + 1 + 200 = 269`).
- **Individually documented contextual reads (from `followup_contextual_review_ledger.json`):** **33** / 269 (**12.27%**); remaining **236** verses are classified as `automated_screening_only` (`insufficient_evidence = 0`).
- **Individually documented Aramaic verses (33):** `Ezra 5:4`, `Ezra 6:4`, `Ezra 6:6`, `Ezra 6:18`, `Ezra 7:21`, `Ezra 7:25`, `Daniel 2:23`, `Daniel 2:24`, `Daniel 2:25`, `Daniel 2:41`, `Daniel 2:43`, `Daniel 3:24`, `Daniel 3:25`, `Daniel 3:31`, `Daniel 3:32`, `Daniel 3:33`, `Daniel 4:1`, `Daniel 4:4`, `Daniel 4:5`, `Daniel 4:32`, `Daniel 4:34`, `Daniel 5:7`, `Daniel 5:14`, `Daniel 5:17`, `Daniel 5:21`, `Daniel 5:25`, `Daniel 6:7`, `Daniel 6:16`, `Daniel 6:19`, `Daniel 6:25`, `Daniel 7:13`, `Daniel 7:14`, `Daniel 7:27`

## 3. Read-Only Cross-Check Against `studio.db` (`stream_tokens` `lang='arc'`)

- `studio.db` contains **4,827** `lang='arc'` tokens across **266** `versification_anchors`, expanding to **270** MT verses: all **269** canonical Biblical Aramaic verses (`Gen 31:47` has 2/9 `arc` tokens; `Dan 2:4` has 8/12 `arc` tokens switching at `2:4b`) **plus 1 read-only lexical-tagging anomaly**:
  - `Ezra 2:1` (Hebrew verse): proper name `נְבוּכַדְנֶצַּ֥ר` (`arc=1/17`) is tagged `arc` in `studio.db` `lexical_stems` (NOT an Aramaic verse).
  - Conversely, `Ezra 5:1` (`15/16 arc`) and `Ezra 6:14` (`21/22 arc`) tag proper name `עִדּוֹא` as `heb` in `studio.db`.