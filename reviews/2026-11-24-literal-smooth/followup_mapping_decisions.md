# Follow-Up Audit — 39-Book Hebrew/Aramaic Mapping & Note-Attachment Regression Check

- **Scope:** All **39** Masoretic Text books (**929** chapters, **23,213** native MT verses) comparing `Saints-Hebrew-Critical-Text` vs. `Modern-English-OT` (`native_verses`, `verses`, `unplaced`, `notes`, `native_notes`, chapter MDs) vs. `Modern-English-OT/parallel-verse-map.json` vs. `Saints-Critical-Text-Studio/studio/lexica/versification.py` (read-only).
- **`versification.py` Hebrew Bugs Found:** **0** (all 42 deltas between `parallel-verse-map.json` and `versification.py` were content-verified against SHCT and `studio.db` Greek; zero edits requested to `Saints-Critical-Text-Studio`).
- **English Verse-Text Changes Made:** **0** (`hebrew_wording_proposals.jsonl`: **0** meaning-changing wording issues found).
- **Validation Result:** `validate_modern_english.py --lang heb` **929/929 PASS, 0 FAIL**; **0** JSON↔MD sync mismatches; **0** README table mismatches; **0** `unresolved` mappings.

## 1. Full-Corpus Mapping Status Breakdown (23,213 MT Verses)

| Mapping Status | MT Verses | Share | Notes |
|---|---:|---:|---|
| `mapped_verified` | **19,448** | 83.78% | 1:1 identity mappings (`native_ref == saints_ref`) |
| `reordered` | **3,402** | 14.66% | `3,400` reordered + `2` `Lev 11:5–6` (`native_order_retained_parallel_display_inverted`) |
| `split_or_merged` | **70** | 0.30% | `70` native MT verses across `24` merged Saints slots (plus `8` one-to-many `>` splits documented in `versification.py`) |
| `no_counterpart` | **293** | 1.26% | `293` standalone `unplaced` MT verses (`saints_ref: "no-site-verse"`; all `after` anchors verified) |
| `unresolved` | **0** | 0.00% | Zero unresolved verses across all 39 MT books |
| **TOTAL** | **23,213** | **100.00%** | `19,448 + 3,402 + 70 + 293 + 0 = 23,213` |

## 2. Content Verification of All 42 `parallel-verse-map.json` vs. `versification.py` Deltas

- **`32` intentional standalone `unplaced` vs. `versification.py` merged/lettered slot:** Modern-English-OT preserves these 32 MT verses as standalone Additional Verses (`no-site-verse`) while `versification.py` maps them into the containing Greek/Saints verse where Greek carries their content (including `Exod 28:24–25` inside Greek `28:29`).
- **`2` `Leviticus 11:5–6` (`native_order_retained_parallel_display_inverted`):** Greek swaps hare (`11:5`) and hyrax (`11:6`); Modern-English-OT retains native MT order with `parallel_counterpart_ref` and reader note.
- **`8` one-to-many (`>`) splits (`Exod 37:18, 38:30, 39:40; Isa 40:8; Jer 7:28, 25:13; Ezek 7:5; Prov 31:26`):** `parallel-verse-map.json` records the primary Saints target matching `versification.py`'s first target. Added missing neutral Rule 2 reader note at `Jer 7:28` (`notes['7:27']` / `native_notes['7:28']`).

## 3. Verified Note-Attachment & Metadata Bugs Fixed (Zero Verse-Text Changes)

Full-corpus programmatic audit of all **4,317** translator notes caught and repaired **75** `native_notes` attachment/cross-reference defects (**54** paired `notes` / chapter-MD updates) across **6 books** missed by Pass 4:

1. **53 Shifted Pre-Migration Saints Cross-References Inside `native_notes` (and unqualified in `notes`):** Repaired across **5 books** — `1 Kings` (**1**: `21:10`), `Nehemiah` (**1**: `7:68`), `Daniel` (**2**: `3:25, 4:16`), `Jeremiah` (**21**: `25:30, 28:8, 29:14, 29:21, 30:8, 31:38, 32:12, 33:5, 34:11, 34:18, 35:6, 35:14, 35:17, 36:7, 38:23, 38:28, 40:14, 46:25, 48:41, 49:1, 50:11`), and `Psalms` (**28**: `11:6, 12:8, 14:3, 16:10, 17:13, 18:27, 42:6, 43:2, 44:3, 44:20, 47:8, 62:2, 80:5, 80:16, 89:7, 90:5, 91:2, 91:14, 96:9, 98:1, 98:4, 116:12, 119:20, 119:22, 119:175, 128:1, 147:5, 148:2`). Updated `native_notes` to exact Masoretic Text references and paired Saints refs with explicit `(MT ch:v)` in `notes` and all **42** synced chapter Markdown files (matching Pass 4's `P4-HEB-03..06` convention).
2. **15 Stale Merged-Slot `native_notes` (`1 Kings` 11, `Proverbs` 4):** Rewrote `native_notes` at `1 Kings 2:35, 2:46, 5:7, 5:14, 6:1, 7:18, 9:9, 10:22, 10:26, 11:14, 12:24` and `Proverbs 15:27, 15:28, 15:29, 20:9` so native-order notes describe standalone MT order vs. Saints parallel merges rather than referring to merged sentences absent from `native_verses` (preserving `notes[saints_ref]` for Saints display).
3. **6 Misattached Secondary-Verse Lexical/Ketiv-Qere Notes:** Moved secondary-verse lexical/Ketiv-Qere notes off primary merged keys onto their exact MT verse keys in `native_notes` (`1 Kings 7:20` 'the latticework', `9:18` Tadmor/Tamar, `9:25` 'burn incense', `14:2` `atti`/`att`; `Proverbs 20:20` `be'eshun`, `20:21` `mevohelet`), recording explicit `nativeNoteCount` in `11-1-kings.json` (`118`) and `22-proverbs.json` (`158`).
4. **Missing Rule 2 Note on `Jeremiah MT 7:28` (`Saints 7:27`) & Stale Division README Table:** Added concise neutral Rule 2 note on `Jer 7:28` (`notes['7:27']` / `native_notes['7:28']` + `chapter-07.md`), bringing totals to **4,318** Saints-view translator notes (`4,255` placed + `63` unplaced) and **4,324** `native_notes`; synced **6** stale pre-Pass-2 per-book note counts in `Modern-English-OT/IV-Providence/README.md` alongside `29-jeremiah/README.md`, `Modern-English-OT/README.md`, and root `README.md`.

## 4. Priority Loci Content-Verification Summary

| Priority Locus | Status | Verification Summary |
|---|---|---|
| `Deuteronomy 5:17-18` | `reordered` | MT 5:17 (murder) -> S 5:18; MT 5:18 (adultery) -> S 5:17. Native MT order preserved in native_verses; dual-view notes accurate. |
| `Numbers 6:23-27` | `split_or_merged` | MT 6:23 & 6:27 standalone in native_verses, merged at S 6:23 (slot 6:27 unmapped). Rule 2 note accurate in both views. |
| `Exodus 20:13-15` | `reordered` | MT 20:13 (murder)->S 20:15, 20:14 (adultery)->S 20:13, 20:15 (steal)->S 20:14. Verified by Hebrew & Greek content. |
| `Exodus 21:16-17` | `reordered` | MT 21:16 (kidnapping)->S 21:17, 21:17 (cursing parents)->S 21:16. Verified by content. |
| `Exodus 36-39` | `reordered` | All 143 MT verses mapped cleanly; 5 deltas vs versification.py (2 intentional standalone unplaced 37:4, 37:22; 3 one-to-many > primary targets 37:18, 38:30, 39:40); 3 merged slots verified; Pass 4 Exod 38:19 & 39:10 note fixes intact. |
| `Leviticus 11:5-6` | `reordered` | Greek/Saints swaps hyrax & hare; Modern-English-OT retains native MT order with explicit parallel_counterpart_ref and reader note. |
| `Numbers 10:34-36` | `reordered` | MT 10:34->S 10:36, 10:35->S 10:34, 10:36->S 10:35. Verified by content & Rule 2 note. |
| `1 Kings 7` | `split_or_merged` | 0 deltas vs versification.py across all 51 MT verses; 3 merged slots (S 7:6, 7:8, 7:18) verified; moved misplaced MT 7:20 Qere note ('the latticework') from native_notes[7:18] to native_notes[7:20]. |
| `2 Kings 25:10` | `no_counterpart` | MT 25:10 absent on live Saints site; cleanly stored as standalone unplaced after 25:9 with explicit note. |
| `Proverbs 31:25-28` | `split_or_merged` | Hebrew alphabetic acrostic preserved in native_verses (Ayin 31:25, Pe 31:26, Tsade 31:27, Qoph 31:28); S 31:28 merges MT 31:26+31:28; Pass 4 note fix intact. |
| `Ezekiel 7:3-10` | `split_or_merged` | MT 7:3-5 before 7:6-9 preserved in native_verses; S 7:10 merges MT 7:5+7:10; Pass 4 note fix intact. |
| `Daniel 3-4 & 6:16` | `split_or_merged` | MT 3:31-33+4:34 unmerged in native_verses, merged at S 4:37; Dan 6:16 (absent in OG) standalone unplaced after 6:15; fixed 2 shifted cross-references in Dan 3:25 (S 3:92) & Dan 4:16 (S 4:19). |
| `Malachi 3:22-24` | `reordered` | MT 3:22->S 3:24, 3:23->S 3:22, 3:24->S 3:23. Verified by content, quotes, and Pass 4 Mal 3:1 note intact. |
| `Psalms` | `reordered` | All 2,527 MT verses mapped cleanly (0 versification.py deltas; Ps 116:14 unplaced); fixed 28 pre-migration Saints cross-references in native_notes + paired (MT) in notes/chapter MDs. |
| `Jeremiah` | `reordered` | All 1,364 MT verses mapped cleanly (68 unplaced; 2 one-to-many > primary targets 7:28, 25:13); fixed 21 pre-migration Saints cross-references + added Rule 2 note on MT 7:28 (S 7:27). |

## 5. Per-Book Mapping Breakdown (All 39 MT Books)

| # | Book | Source Total | `mapped_verified` | `reordered` | `split_or_merged` | `no_counterpart` | `unresolved` |
|---:|---|---:|---:|---:|---:|---:|---:|
| 1 | Genesis | 1,533 | 1,531 | 0 | 0 | 2 | 0 |
| 2 | Exodus | 1,213 | 1,056 | 96 | 6 | 55 | 0 |
| 3 | Leviticus | 859 | 857 | 2 | 0 | 0 | 0 |
| 4 | Numbers | 1,289 | 1,236 | 50 | 2 | 1 | 0 |
| 5 | Deuteronomy | 959 | 955 | 4 | 0 | 0 | 0 |
| 6 | Joshua | 658 | 638 | 5 | 0 | 15 | 0 |
| 7 | Judges | 618 | 618 | 0 | 0 | 0 | 0 |
| 8 | Ruth | 85 | 85 | 0 | 0 | 0 | 0 |
| 9 | 1 Samuel | 811 | 772 | 0 | 0 | 39 | 0 |
| 10 | 2 Samuel | 695 | 695 | 0 | 0 | 0 | 0 |
| 11 | 1 Kings | 817 | 617 | 124 | 43 | 33 | 0 |
| 12 | 2 Kings | 719 | 718 | 0 | 0 | 1 | 0 |
| 13 | 1 Chronicles | 943 | 930 | 0 | 0 | 13 | 0 |
| 14 | 2 Chronicles | 822 | 821 | 0 | 0 | 1 | 0 |
| 15 | Ezra | 280 | 280 | 0 | 0 | 0 | 0 |
| 16 | Nehemiah | 405 | 386 | 5 | 0 | 14 | 0 |
| 17 | Esther | 167 | 164 | 0 | 0 | 3 | 0 |
| 20 | Job | 1,070 | 1,069 | 0 | 0 | 1 | 0 |
| 21 | Psalms | 2,527 | 138 | 2,388 | 0 | 1 | 0 |
| 22 | Proverbs | 915 | 881 | 2 | 13 | 19 | 0 |
| 23 | Ecclesiastes | 222 | 222 | 0 | 0 | 0 | 0 |
| 24 | Song of Songs | 117 | 117 | 0 | 0 | 0 | 0 |
| 25 | Lamentations | 154 | 150 | 0 | 0 | 4 | 0 |
| 28 | Isaiah | 1,291 | 1,289 | 0 | 0 | 2 | 0 |
| 29 | Jeremiah | 1,364 | 614 | 682 | 0 | 68 | 0 |
| 30 | Ezekiel | 1,273 | 1,259 | 6 | 2 | 6 | 0 |
| 31 | Daniel | 357 | 303 | 35 | 4 | 15 | 0 |
| 32 | Hosea | 197 | 197 | 0 | 0 | 0 | 0 |
| 33 | Joel | 73 | 73 | 0 | 0 | 0 | 0 |
| 34 | Amos | 146 | 146 | 0 | 0 | 0 | 0 |
| 35 | Obadiah | 21 | 21 | 0 | 0 | 0 | 0 |
| 36 | Jonah | 48 | 48 | 0 | 0 | 0 | 0 |
| 37 | Micah | 105 | 105 | 0 | 0 | 0 | 0 |
| 38 | Nahum | 47 | 47 | 0 | 0 | 0 | 0 |
| 39 | Habakkuk | 56 | 56 | 0 | 0 | 0 | 0 |
| 40 | Zephaniah | 53 | 53 | 0 | 0 | 0 | 0 |
| 41 | Haggai | 38 | 38 | 0 | 0 | 0 | 0 |
| 42 | Zechariah | 211 | 211 | 0 | 0 | 0 | 0 |
| 43 | Malachi | 55 | 52 | 3 | 0 | 0 | 0 |
| — | **TOTAL (39 MT Books)** | **23,213** | **19,448** | **3,402** | **70** | **293** | **0** |
