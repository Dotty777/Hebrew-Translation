# Stage 2 Pass 2 — Independent Second Hebrew/Aramaic Source-Language Verification & Editing

- **Reviewer Role:** `heb-peer` (Independent Second Hebrew/Aramaic Source-Language Verifier & Editor)
- **Date:** 2026-11-25
- **Branch:** `review/2026-11-24-literal-smooth`
- **Base Commit (`HEB_BASE_SHA`):** `206d2445daebca44499838fa048ce3947861e67d`
- **Verified Pass 2 Corpus Commit (`HEB_PASS2_SHA`):** `57f6d10839e6029b4c33ccf8675310e1caabdf3b`
- **Pinned Critical Text (`CTS_SHA`):** `Saints-Hebrew-Critical-Text` Studio v10 Stage 1 (`a0d022c1`, MAM Aleppo + WLC Leningrad)
- **Strict Isolation Attestation:** Independently verified 100% strictly inside `Hebrew-Translation/` (`Saints-Hebrew-Critical-Text/`, `Modern-English-OT/`, `corrections/2026-11-24-modern-english-fidelity/`, legacy `<slug>/verses.json`), `review-charter.md`, and `hebrew_inventory.json`. Zero access to Greek or Latin repositories, critical texts, or translations.

---

## 1. Executive Scorecard & Source-Derived Coverage (Rules 0, 2, 4, 5)

| Metric | Count | Status |
|---|---:|---|
| Adopted MT Books / Chapters | **39** books / **929** chapters | 100% validated |
| Adopted MT Source Verses (`Saints-Hebrew-Critical-Text`) | **23,213** (WLC 23,213 / MAM 23,210) | `missing_in_studio = 0` |
| Modern English Dual-Key Coverage (`native_verses`) | **23,213** native MT verses (0 forced merges, 0 collisions) | `missing_in_native_verses = 0` |
| Modern English Saints.Bible Parallel Slots (`verses` + `unplaced`) | **22,874** placed + **293** unplaced (disambiguated with `native_ref`/`saints_ref`) | 100% site-compatible |
| Total Translator Notes (`noteCount` = `placedNoteCount + unplacedNoteCount`) | **4,308** (**4,246** placed + **62** unplaced) | 0 header drift |
| Pass 1 Proposals Independently Verified (`pass2_verdicts.jsonl`) | **78** / 78 | **48** `approved`, **25** `modified_approved`, **5** `escalate_human_editor`, **0** `rejected` |
| Pass 2 Bonus Independent Catches Applied | **2** | `Gen 47:31` (NT citation), `Exod 28:36` (nested quotes) |
| Pass 2 `verified` MT Verses | **23,008** (+102 resolved from Pass 1) | Audited & validated |
| Pass 2 `disputed` MT Verses (human editorial queue) | **205** | Kept explicitly visible |
| Pass 2 `unverified` MT Verses | **0** | `verified + disputed + unverified == 23,213` (PASS) |
| Consolidated Human Editorial Queue (`pass2_human_editor_queue.jsonl`) | **41** items | Zero silent doctrinal overrides |
| NT Citations Remaining in Hebrew OT Notes | **0** | Strict Hebrew-from-Hebrew isolation |
| Automated Full-Corpus Validation Errors (39 JSONs + 929 MDs) | **0** | 100% JSON/MD sync, even quote parity |

---

## 2. Six Major Independent Pass 2 Catches (Correcting Pass 1 Oversights)

Independent re-verification against `Saints-Hebrew-Critical-Text/` caught six substantive issues in Pass 1's proposals before any edits landed:

1. **`Daniel 9:26` Masoretic Accent Inversion (`HEB-P1-060`):** Programmatic Unicode decoding of `וְעַד֙ קֵ֣ץ מִלְחָמָ֔ה` proved that `קֵ֣ץ` carries **conjunctive *munach*** (`U+05A3`, binding `qets` directly to `milchamah`, `"until the end of the war"`), NOT a disjunctive accent as Pass 1 claimed! Corrected the Rule 4 footnote to accurately describe *munach* vs. the alternative independent syntax.
2. **Missed NT Citation in `Genesis 47:31` (`HEB-P2-BONUS-001`):** Full-corpus regex audit of all notes caught a **4th** NT citation (`Hebrews 11:21` + Septuagint in `Gen 47:31`) missed by Pass 1 alongside `Jer 38:32` (`Heb 8:9`), `Joel 3:1` (`Acts 2:17`), and `Amos 9:12` (`Acts 15:17`). All 4 were sanitized to strictly Hebrew-internal notes (`0` NT citations remaining across all 4,308 notes).
3. **Missed Nested Quote in `Exodus 28:36` (`HEB-P2-BONUS-002`, paired with `HEB-P1-076`–`077`):** Removing the premature closing `"` at `Exod 25:40` and redundant opening `"` at `Exod 30:1` places `Exod 28:36` inside the continuous double-quoted divine speech `25:2–30:10`, requiring converting `28:36`'s engraving `"Holiness to the LORD."` to single quotes `'Holiness to the LORD.'` per `STYLE.md`.
4. **Unbalanced Triple-Quote Bug in `Numbers 6:23–27` (`HEB-P1-016`–`017`):** Pass 1's proposed unmerge of MT `6:23` and `6:27` produced 3 double quotes and 3 single quotes across `6:23–27`. Fixed clean 3-level quote nesting (`"` → `'` → `"`, matching `Exod 3:16–17`) inside `native_verses` (`6` even double quotes across Numbers ch. 6).
5. **Prevented `verse-map.json` Corruption on `Leviticus 11:5–6` (`HEB-P1-020`):** Because `03-leviticus.json` ALREADY translates MT `11:5` (rock hyrax) at key `11:5` and MT `11:6` (hare) at key `11:6`, adding swapped entries to `verse-map.json` (`{english_key: [mt_keys]}`) would have pointed rock hyrax to `הָאַרְנֶבֶת` (hare)! Preserved `verse-map.json`, added a neutral reader note on `Lev 11:5`, and recorded `relation: "native_order_retained_parallel_display_inverted"` in `parallel_map`.
6. **Prevented Archive Corruption on Legacy `<slug>/verses.json` (`HEB-P1-044`):** Matching every legacy row against its **own** captured `hebrew` and `english` fields proved that ~103 of the 133 discrepancies Pass 1 flagged (including all 33 Genesis `31:55–32:32` rows, Exodus `36–38` rows, and unmerged 1 Kings / grouped Daniel 5 cards) already accurately reflect their own captured staging text. Fixed the **30 genuinely non-WLC *ta'am elyon* entries** (`exodus/verses.json` `20:14–26` [13] and `deuteronomy/verses.json` `5:17–33` [17]) cleanly to WLC/MAM `Saints-Hebrew-Critical-Text` numbering.

Also caught and refined:
- **`Joshua 19` (`HEB-P1-070`):** Expanded boundary-term harmonization from 4 verses to all **9** boundary-line verses in chapter 19 (`19:10, 11, 12, 14, 22, 29, 33, 34, 49`), preserving `"territory"` where `גְּבוּל` denotes tribal area.
- **`Song of Songs 8:3` (`HEB-P1-062`):** Noted the absence of preposition `לְ־` before `רֹאשִׁי` compared to `2:6` (`תַּחַת לְרֹאשִׁי` vs. `תַּחַת רֹאשִׁי`).

---

## 3. Applied Edits & Non-Destructive Rule 2 Dual-Key Architecture

- **Non-Destructive Dual-Key Schema (All 39 Book JSONs + `Modern-English-OT/parallel-verse-map.json`):**
  - Preserves 100% backward compatibility on `verses` (`22,874` Saints.Bible slots), `notes`, `unplaced` (`293` entries, each now explicitly tagged with `native_ref` and `saints_ref: "no-site-verse"` to disambiguate all 68 colliding keys in Exodus `36–38`, Jeremiah, and Daniel `4:4/4:5/4:32`).
  - Adds canonical `native_verses` (`23,213` individual MT verses in exact `Saints-Hebrew-Critical-Text` order, unmerging all 24 merged Saints slots cleanly across Exodus, Numbers, 1 Kings, Proverbs, Ezekiel, and Daniel, healing quote breaks in `Gen 31:51–53`, `Num 6:23–27`, `Ezek 7:2–10`, and `Mal 3:22–24`), `native_notes`, and `parallel_map`.
  - Updates `noteCount` across all 39 JSONs (`noteCount == placedNoteCount + unplacedNoteCount == 4,308`), synchronizes **96** chapter Markdown files + **25** book READMEs + **4** division READMEs + `Modern-English-OT/README.md` (`261` → `293`) + root `README.md`.
- **Verified Verse-Text Edits Applied (20 verses, zero doctrinal overrides):**
  - `Job 7:5` (singular `a crust of dust`); `Lev 20:3` (`so as to defile ... and to profane`); `1 Kgs 8:65` & `Ezek 47:20` (`Lebo-hamath`); `Dan 5:14` (`illumination`); `Josh 19:10, 11, 12, 14, 22, 29, 33, 34, 49` (`boundary`/`boundaries`/`outer limits`); `Ps 15:1, 59:1, 73:1, 77:1` [MT `16:1, 60:1, 74:1, 78:1`] (`Miktam`/`Maskil`); `Exod 25:40, 28:36, 30:1` (continuous quote frame `25:2–30:10`).
- **Strictly Escalated Without Silent Main-Text Changes (`pass2_human_editor_queue.jsonl` — 41 items):**
  - `HEB-P1-052` (`Ps 51:13` `holy Spirit`), `HEB-P1-057`–`059` (`Lev 22:13`, `1 Sam 1:11`, `Dan 9:1` `seed`/`offspring`), `HEB-P1-064` (`Jer 33:15` `branch`/`Branch`), `HEB-HQ-003` (`Josh 21:36–37` `⟦ ⟧`), `HEB-HQ-004` (`Ps 24:4`), all Ezekiel/`Isa 32:15`/`Num 11:17`/`Isa 11:2` Spirit capitalizations, all 9 Hebraist judgment calls, all 18 Messianic & 3 theophanic/title capitalizations, site display-slot order policy (`HEB-HQ-001`), and ancient-version note policy (`HEB-HQ-002`).

---

## 4. Per-Book Pass 2 Coverage Table (All 39 MT Books)

| # | Book | Chs | Source Total | Placed Slots | Unplaced | Native MT | Notes | Verified | Disputed | Unverified |
|---:|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 1 | Genesis | 50 | 1,533 | 1,531 | 2 | 1,533 | 254 | 1,530 | 3 | 0 |
| 2 | Exodus | 40 | 1,213 | 1,155 | 55 | 1,213 | 184 | 1,173 | 40 | 0 |
| 3 | Leviticus | 27 | 859 | 859 | 0 | 859 | 125 | 855 | 4 | 0 |
| 4 | Numbers | 36 | 1,289 | 1,287 | 1 | 1,289 | 178 | 1,281 | 8 | 0 |
| 5 | Deuteronomy | 34 | 959 | 959 | 0 | 959 | 157 | 955 | 4 | 0 |
| 6 | Joshua | 24 | 658 | 643 | 15 | 658 | 114 | 655 | 3 | 0 |
| 7 | Judges | 21 | 618 | 618 | 0 | 618 | 96 | 618 | 0 | 0 |
| 8 | Ruth | 4 | 85 | 85 | 0 | 85 | 19 | 85 | 0 | 0 |
| 9 | 1 Samuel | 31 | 811 | 772 | 39 | 811 | 147 | 810 | 1 | 0 |
| 10 | 2 Samuel | 24 | 695 | 695 | 0 | 695 | 115 | 695 | 0 | 0 |
| 11 | 1 Kings | 22 | 817 | 754 | 33 | 817 | 114 | 817 | 0 | 0 |
| 12 | 2 Kings | 25 | 719 | 718 | 1 | 719 | 121 | 719 | 0 | 0 |
| 13 | 1 Chronicles | 29 | 943 | 930 | 13 | 943 | 141 | 942 | 1 | 0 |
| 14 | 2 Chronicles | 36 | 822 | 821 | 1 | 822 | 149 | 822 | 0 | 0 |
| 15 | Ezra | 10 | 280 | 280 | 0 | 280 | 50 | 280 | 0 | 0 |
| 16 | Nehemiah | 13 | 405 | 391 | 14 | 405 | 64 | 405 | 0 | 0 |
| 17 | Esther | 10 | 167 | 164 | 3 | 167 | 38 | 165 | 2 | 0 |
| 18 | Job | 42 | 1,070 | 1,069 | 1 | 1,070 | 191 | 1,068 | 2 | 0 |
| 19 | Psalms | 150 | 2,527 | 2,526 | 1 | 2,527 | 610 | 2,516 | 11 | 0 |
| 20 | Proverbs | 31 | 915 | 888 | 19 | 915 | 156 | 911 | 4 | 0 |
| 21 | Ecclesiastes | 12 | 222 | 222 | 0 | 222 | 52 | 221 | 1 | 0 |
| 22 | Song of Songs | 8 | 117 | 117 | 0 | 117 | 35 | 116 | 1 | 0 |
| 23 | Lamentations | 5 | 154 | 150 | 4 | 154 | 30 | 154 | 0 | 0 |
| 24 | Isaiah | 66 | 1,291 | 1,289 | 2 | 1,291 | 294 | 1,257 | 34 | 0 |
| 25 | Jeremiah | 52 | 1,364 | 1,296 | 68 | 1,364 | 259 | 1,331 | 33 | 0 |
| 26 | Ezekiel | 48 | 1,273 | 1,266 | 6 | 1,273 | 229 | 1,256 | 17 | 0 |
| 27 | Daniel | 12 | 357 | 339 | 15 | 357 | 87 | 337 | 20 | 0 |
| 28 | Hosea | 14 | 197 | 197 | 0 | 197 | 59 | 197 | 0 | 0 |
| 29 | Joel | 4 | 73 | 73 | 0 | 73 | 17 | 73 | 0 | 0 |
| 30 | Amos | 9 | 146 | 146 | 0 | 146 | 42 | 146 | 0 | 0 |
| 31 | Obadiah | 1 | 21 | 21 | 0 | 21 | 5 | 21 | 0 | 0 |
| 32 | Jonah | 4 | 48 | 48 | 0 | 48 | 17 | 48 | 0 | 0 |
| 33 | Micah | 7 | 105 | 105 | 0 | 105 | 32 | 99 | 6 | 0 |
| 34 | Nahum | 3 | 47 | 47 | 0 | 47 | 15 | 47 | 0 | 0 |
| 35 | Habakkuk | 3 | 56 | 56 | 0 | 56 | 15 | 56 | 0 | 0 |
| 36 | Zephaniah | 3 | 53 | 53 | 0 | 53 | 15 | 52 | 1 | 0 |
| 37 | Haggai | 2 | 38 | 38 | 0 | 38 | 10 | 38 | 0 | 0 |
| 38 | Zechariah | 14 | 211 | 211 | 0 | 211 | 57 | 206 | 5 | 0 |
| 39 | Malachi | 3 | 55 | 55 | 0 | 55 | 15 | 51 | 4 | 0 |
| — | **TOTAL (39 MT Books)** | **929** | **23,213** | **22,874** | **293** | **23,213** | **4,308** | **23,008** | **205** | **0** |
---

## 5. Stage 2 Pass 3 Bounce-Back Verification (`P3B-001`–`P3B-014`)

- **Pass 3 Standalone Surface Commit (`HEB_PASS3_SHA`):** `915915e68d270ba12d710522550c464c3b519041` (`@heb-flow`, 11 Bucket A edits)
- **Verified Pass 3 Bounce-Back Corpus Commit (`HEB_PASS3B_SHA`):** `b3e0f2ea87923eea52517398b65c7c8b4daf4cd3` (`@heb-peer`)
- **Deliverable:** `pass3_bounceback_verdicts.jsonl` (**14 / 14** items independently verified against `Saints-Hebrew-Critical-Text/`):
  - **`approved` (9):** `P3B-001` (`Exod 32:7–10`), `P3B-002` (`Jer 11:6–8`), `P3B-003` (`Job 30:1–31:40`), `P3B-008` (`Exod 25:40–30:10`), `P3B-009` (`Exod 21:1–23:33`), `P3B-010` (`Exod 39:34, 39:41`), `P3B-011` (`Lev 1–3, 4–5, 6:18–7:21, 25–26`), `P3B-012` (`Num 28:31–29:39`), `P3B-014` (`Jer 30:10–11, 30:22, 46:26, 48:45–47, 49:6, 51:45–48`)
  - **`modified_approved` (3):** `P3B-005` (`2 Chr 2:7–8`, smoothed LBH *waw* + infinitive + note), `P3B-006` (`Esth 9:29–31`, dual-view comma on `verses['9:29']` & `native_verses['9:30']`, terminal `.` kept on standalone `unplaced['9:30']` + note), `P3B-007` (`Jer 29:15–21`, em-dash at `native_verses['29:15']`, capitalized `native_verses['29:21']`, Rule 2 note on `36:15`/`29:15`)
  - **`escalate_human_editor` (2):** `P3B-004` (`Deut 32:27–35` → `HEB-HQ-042`, Rule 4 notes added on `32:28` and `32:34`), `P3B-013` (`Job 28:1–28` → `HEB-HQ-043`, kept unquoted + Rule 4 note added on `28:1`)
  - **`rejected` (0)**
- **Post-Pass-3B Updated Corpus Totals (`HEB_PASS3B_SHA`):**
  - **Source MT Coverage:** `23,213` total (`22,972` `verified` + `241` `disputed` + `0` `unverified` == `23,213` PASS)
  - **Translator Notes:** `4,314` total (`4,251` placed + `63` unplaced; `+6` new notes, `2` notes expanded; `0` NT citations)
  - **Consolidated Human Editorial Queue (`pass2_human_editor_queue.jsonl`):** `43` items (`HEB-HQ-001`–`HEB-HQ-043`)
  - **Full-Corpus 3-Level Quotation & Mechanics Validation (39 JSONs + 929 Chapter MDs):** `0` native 3-level quote-stack errors, `0` native open chapter breaks, `0` native lowercase-after-period anomalies, `0` schema/sync/hygiene errors.
---

## 6. Stage 2 Pass 3.5 AI Peer Review Verification & Pattern Expansion

- **Blind Sample Result (`00ff8636`):** `37/40` `verified_faithful`, `3` `flagged` (`HEB-P35-20` `Prov 14:32`, `HEB-P35-32` `Neh 4:7`, `HEB-P35-33` `Exod 37:14`), `0` `unverified`, `1` recurring pattern (cross-verse coreference/referent disruption).
- **Verified Post-Pass-3.5 Corpus Commit (`HEB_POST_P35_SHA`):** `6fe3807ef4969a2184fe85f960c007b6f83c7a2e` (`@heb-peer`)
- **Deliverable:** `pass35_ai_peer_review_response.jsonl` (**5** records: **3** blind flags verified + **2** pattern-expansion catches applied):
  1. **`HEB-P35-20` (`Prov 14:32`, `modified_approved_and_escalated` → `HEB-HQ-044`):** Replaced forced English object syntax with temporal MT rendering (`in his death a righteous man has a refuge`), expanded the Rule 4 footnote on `choseh bemoto` + `bera'ato`, and logged `HEB-HQ-044` for final human editorial confirmation.
  2. **`HEB-P35-32` (`Neh 4:7`, `approved`):** Eliminated the inserted pronoun collision with v. 6 by naming `"the people"` (`אֶת־הָעָם`) on the first `וָאַעֲמִיד` and `"them"` on the resumptive verb, plus added a brief resumptive-syntax note; verified all other repeated 1cs wayyiqtol verses in Nehemiah (`2:15, 7:5, 13:19`) are clean.
  3. **`HEB-P35-33` (`Exod 37:14` / Saints `38:10`, `approved`):** Harmonized definite `הַמִּסְגֶּרֶת` from `"the rim"` to `"the frame"` (matching `Exod 25:25, 25:27, 37:12`); audited all 21 `מסגר*` verses across MT (`1 Kgs 7:28–36`, `2 Kgs 16:17`, etc., all internally consistent).
  4. **`HEB-P35-EXP-01` (`Exod 36:34` / Saints `38:18` & `Exod 39:33` / Saints `39:13`, `approved`):** Tabernacle architectural expansion across 18 terms in `Exod 25–40` caught `בְּרִיחַ` switching from `"crossbars"` (`26:26–29, 35:11, 36:31–33, 40:18`) to `"bars"` in `36:34` (2x) and `39:33`; harmonized all 11 verses to `"crossbar(s)"`.
  5. **`HEB-P35-EXP-02` (`Exod 39:39` & `40:11` unplaced, `approved`):** Tabernacle architectural expansion caught `הַכִּיּוֹר וְאֶת־כַּנּוֹ` switching from `"the basin and its stand"` (`30:18, 30:28, 31:9, 35:16, 38:8`) to `"the basin and its base"` in `39:39` and `40:11` (colliding with `אֶדֶן` `"bases"`); harmonized all 7 verses to `"the basin and its stand"`.
- **Post-Pass-3.5 Final Totals (`HEB_POST_P35_SHA`):** `23,213` source MT verses (`22,971` `verified` + `242` `disputed` + `0` `unverified` == `23,213` PASS), `4,314` notes (`4,251` placed + `63` unplaced, `0` NT citations), `44` human-editor queue items (`HEB-HQ-001`–`HEB-HQ-044`), `0` schema/sync/quote-stack/open-chapter-break errors across all 39 books & 929 chapter MDs.
