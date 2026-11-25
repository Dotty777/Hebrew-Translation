# Stage 2 Pass 1 — Independent Hebrew/Aramaic-Only Source-Language Fidelity Review

- **Reviewer Role:** `heb-fidelity` (Independent Hebrew/Aramaic-Only Source-Language Fidelity Reviewer)
- **Date:** 2026-11-24
- **Pinned Hebrew-Translation Revision:** branch `review/2026-11-24-literal-smooth` @ `206d2445daebca44499838fa048ce3947861e67d`
- **Pinned Critical Text Revision:** `Saints-Hebrew-Critical-Text` Studio v10 Stage 1 @ `a0d022c1` (MAM Aleppo + WLC Leningrad)
- **Strict Isolation Attestation:** Audited 100% strictly within `Hebrew-Translation/` (`Saints-Hebrew-Critical-Text/`, `Modern-English-OT/`, `corrections/2026-11-24-modern-english-fidelity/`, legacy `<slug>/verses.json`), `review-charter.md`, and `hebrew_inventory.json`. Zero access to Greek or Latin texts, repositories, or translations. Zero edits made to Modern English book JSON/MD files in Pass 1.

---

## 1. Executive Scorecard & Source-Derived Coverage (Rule 0 & Rule 5)

| Metric | Count | Status |
|---|---:|---|
| Adopted MT Books / Chapters | **39** books / **929** chapters | 100% covered |
| Adopted MT Source Verses (`Saints-Hebrew-Critical-Text`) | **23,213** (WLC 23,213 / MAM 23,210) | `missing_in_studio = 0` |
| Modern English Coverage | **22,874** placed + **293** unplaced = **23,167** units (incl. 24 merged slots) | `missing_in_english = 0`, 0 duplicates |
| Pass 1 `verified` Verses | **22,906** | Audited programmatically + contextually |
| Pass 1 `disputed` Verses (unique MT refs in proposals / human queue) | **307** | Routed to Pass 2 / Human Editor |
| Pass 1 `unverified` Verses | **0** | `verified + disputed + unverified == 23,213` |
| Total Traceable Proposals (`pass1_proposals.jsonl`) | **78** (36 flagged `needs_human_editor`) | Ready for Pass 2 verification |
| Human Editorial Queue Items (`pass1_human_queue.jsonl`) | **41** | Doctrinal / structural / witness decisions |
| Extant Non-MT Hebrew Witnesses (`no_counterpart_in_mt`) | Ben Sira (**893** vv / 46 chs / 8 TEI MSS); 11QPs-a Ps 151 (**7** vv) | Out-of-MT canon (not `missing`) |

### Proposals by Category

| Category | Count |
|---|---:|
| `rule2_native_order_mapping` | 31 |
| `lexical_and_formatting_consistency` | 12 |
| `rule4_ambiguity_ruach` | 9 |
| `fidelity_grammar_and_hebraist_notes` | 8 |
| `false_or_stale_note` | 6 |
| `rule4_ambiguity_zera` | 5 |
| `isolation_nt_citation_note` | 3 |
| `stage1_drift` | 2 |
| `qere_wela_ketiv_note` | 2 |

### Human Editorial Queue by Type

| Issue Type | Count |
|---|---:|
| `messianic_capitalization` | 18 |
| `hebraist_judgment_call` | 9 |
| `rule4_ambiguity_ruach` | 5 |
| `textual_witness_variant` | 2 |
| `rule4_ambiguity_zera` | 2 |
| `rule2_structural_policy` | 1 |
| `editorial_policy_isolation_notes` | 1 |
| `disputed_theophanic_capitalization` | 1 |
| `disputed_title_translation` | 1 |
| `disputed_capitalization` | 1 |

---

## 2. Stage 1 Critical-Text Drift Audit (`HEAD~1` vs `HEAD`, Studio v10 `a0d022c1`)

Programmatic column-level diff of all 425 updated TSV/chapter artifacts (266 TSV files changed between Nov 18 base and Studio v10 Stage 1 `a0d022c1`) found:

- **38 verses with actual column-3 `Critical_Text` changes** (all remaining TSV diffs are metadata-only: 309 `Confidence` updates, 285 `Substantive_Variants` updates):
  - **7 MAM double-vowel Unicode normalizations** (`Num 6:2, 11:32; 2 Chr 24:4; Jer 28:4; Ezek 17:7; Jonah 4:2; Nah 1:2`) — English 100% clean.
  - **15 multi-word Ketiv `_` → space normalizations** (`Jdg 16:25; 1 Sam 9:1, 20:2, 24:9; 2 Sam 5:2, 21:12; 1 Kgs 17:15; 2 Chr 34:6; Job 38:12; Lam 1:6, 4:3; Isa 9:6, 44:24; Jer 48:20; Ezek 42:9`) — English follows Qere cleanly.
  - **6 verse-ending `(ketiv)׃` → `׃ (ketiv)` normalizations** (`2 Sam 3:15, 19:32; Neh 11:17; Ps 105:28; Isa 30:32; Ezek 16:25`) — English follows Qere cleanly.
  - **8 Ketiv-wela-Qere `((...))` → `(...)` normalizations** (`Ruth 3:12; 2 Sam 13:33, 15:21; 2 Kgs 5:18; Jer 38:16, 39:12, 51:3; Ezek 48:16`) — all 8 follow Qere (omit unread particle).
  - **`Job 7:5`** (`(וג)יש` → `(וגיש)`): English already followed Qere `וְגוּשׁ`, no regression.
  - **`Jer 3:7`** (`ותראה` → `(ותראה)`): English already translates Qere `וַתֵּרֶא` once with no duplication.
- **0 meaning regressions** from the Stage 1 sync.
- **2 Pass 1 follow-up proposals raised:**
  1. **`Job 7:5`** (`HEB-P1-001`): English renders singular Qere `גּוּשׁ` (`a clod/crust`) as plural while its own note glosses singular `and a clod/crust` — propose aligning to singular.
  2. **`Jeremiah 39:12`** (`HEB-P1-002`): The only 1 of the 8 Ketiv-wela-Qere verses lacking a footnote explaining unread `(אם)`.

---

## 3. Native MT Order & Dual-Key Mapping Audit (Rule 2 — CRITICAL)

Currently, `Modern-English-OT` keys its primary `verses` dictionary by **Saints.Bible parallel display slots** rather than native MT order and exiles 293 MT verses to an `unplaced` array. This causes concrete textual, syntactic, and data-integrity defects:

1. **Priority Loci Damaged by Saints-Slot Primary Storage:**
   - **`Deuteronomy 5:17–18`** (`HEB-P1-014`, `HEB-P1-015`): Swapping MT `5:18` (`וְלֹא תִנְאָף`) into slot `5:17` and MT `5:17` (`לֹא תִרְצָח`) into slot `5:18` inverts the Hebrew syndetic `וְ` conjunction (`And ...` before the unmarked first commandment, then `And ...` again at `5:19`).
   - **`Numbers 6:23–27`** (`HEB-P1-016`, `HEB-P1-017`): Grafting MT `6:27` into the middle of slot `6:23` via an em-dash severs the blessing intro from the Aaronic Blessing (`6:24–26`), corrupts nested quotation marks, and leaves slot `6:27` empty.
   - **`Leviticus 11:5–6`** (`HEB-P1-020`): Prior pass restored native MT order (`11:5` rock hyrax, `11:6` hare) and deleted the note, **without** recording the Saints parallel swap (`MT 11:5 <-> Saints 11:6`) in `verse-map.json` or leaving a reader note.
   - **`Genesis 31:51`** (`HEB-P1-022`): Exiling MT `31:51` to `unplaced` splits Laban's speech so `unplaced:31:51` has an unclosed opening quote and placed `31:53` has an orphan closing quote.
   - **`Exodus 38:30–31` (Saints `39:9, 39:8`)** (`HEB-P1-006`): Slot reversal caused a **false note** claiming the Hebrew lacks a finite verb in v. 8 until v. 9, whereas in MT `38:30` (verb) precedes `38:31` (objects).
   - **`Daniel 3:31–33` & `4:1–34`** (`HEB-P1-038`, `HEB-P1-039`): Merging MT `3:31–33` with `4:34` in slot `4:37` moves Nebuchadnezzar's opening epistolary greeting to the END of chapter 4, leaves `4:1–3` empty, and creates **direct key collisions on `4:4`, `4:5`, and `4:32`** between placed `verses{}` (MT `4:1, 4:2, 4:29`) and `unplaced[].src` (MT `4:4, 4:5, 4:32`).
   - **`Malachi 3:22–24`** (`HEB-P1-041`–`HEB-P1-043`): Restoring native MT order (`3:22` Remember the law → `3:23` Elijah → `3:24` turn back hearts) also requires shifting the opening/closing quotation marks to `3:22` and `3:24`.
   - Also mapped with exact proposals: **`Exod 20:13–15`** (`HEB-P1-018`), **`Exod 21:16–17`** (`HEB-P1-019`), **`Num 10:34–36`** (`HEB-P1-021`), **`Exod 36–39`** (incl. undocumented merges at `38:10`, `38:24`, `38:27`: `HEB-P1-028`–`HEB-P1-031`), **`1 Kgs 7`** (incl. undocumented merges at `7:6` [MT `7:18, 7:20`], `7:8` [MT `7:19, 7:22`], `7:18` [MT `7:31–32`]: `HEB-P1-032`–`HEB-P1-034`), **`Prov 16:4` (Saints `16:9`) & `31:25–28`** (`HEB-P1-035`, `HEB-P1-036`), **`Ezek 7:3–10`** (`HEB-P1-037`), plus 5 undocumented reordered passages (**`Num 1:24–37`**, **`Num 26:15–47`**, **`Deut 23:25–26`**, **`Josh 19:47–48`**, **`Josh 24:29–31`**: `HEB-P1-023`–`HEB-P1-027`).
2. **68 `verses`-vs-`unplaced` Key Collisions Across 3 Books:**
   - **Exodus:** 32 colliding keys (`36:10–33, 37:4, 11–12, 20–21, 38:2, 6–7`) (`HEB-P1-031`)
   - **Jeremiah:** 33 colliding keys (`7:27, 25:14, 27:1/7/13/17/21, 30:10/11/15, 33:14–24, 39:4–13, 46:1, 49:6`) (`HEB-P1-040`)
   - **Daniel:** 3 colliding keys (`4:4, 4:5, 4:32`) (`HEB-P1-039`)
3. **133 Legacy `<slug>/verses.json` `masoretic_reference` Mismatches Across 9 Books:**
   - Genesis (33), Exodus (52), Numbers (3), Deuteronomy (16), 1 Kings (15), Proverbs (6), Jeremiah (2 — incl. wrong `25:20 -> 49:34`), Ezekiel (2), Daniel (4 — incl. `4:37 -> 4:34` omitting `3:31–33`) (`HEB-P1-044`).
4. **Proposed Non-Destructive Rule 2 Architecture (`HEB-HQ-001`):**
   - Store canonical Hebrew-English source data strictly in **native MT order** (`native_verses` keyed solely by MT `ch:v`, zero forced merges, zero `unplaced` key collisions) paired with an explicit **`saints_parallel_map`** mapping every native MT verse to Saints.Bible display slot(s) or `no-site-verse`, with concise neutral reader notes wherever a split/merge/reorder/unmatched verse could resemble an omission.

---

## 4. Full-Corpus Programmatic & Contextual Fidelity Audit (All 23,213 Verses)

### A. Whole-Corpus Automated Quality & Structural Sweeps (Zero Regressions)
- **Adjacent-verse swap detector (IBM-1/PMI alignment across all 23,213 vv):** **0** unmapped swaps detected.
- **Low-alignment outliers (83 vv) & length-ratio outliers (35 vv):** All 118 manually read against MT Hebrew; 0 dropped clauses or mistranslations (genealogies, architectural lists, compact poetic formulas).
- **Tetragrammaton (`יְהוָה`) count parity:** **0** drops or additions across all 23,213 vv (all 46 short-form matches are poetic `יָהּ` / `Hallelujah` / Song 8:6 `שַׁלְהֶבֶתְיָה`).
- **Negation (`לֹא`) parity:** **0** dropped negations across all 23,213 vv (20 flagged hits are affirmative oath-idiom `אִם־לֹא` [18x] and Hosea names `Lo-ruhamah`/`Lo-ammi` [2x]).
- **Style & markup hygiene:** **0** banned archaisms, **0** forbidden divine names (`YHWH`/`Yahweh`/`Jehovah`/`Tetragrammaton`), **0** Ketiv/Qere markup leaks (`(` or `_`), **0** stray brackets.
- **All 24 `יַם־סוּף` occurrences:** 24/24 consistently render `Sea of Reeds` (`0` `Red Sea`).
- **Judges 10–11:** 8/8 `בְּנֵי יִשְׂרָאֵל` occurrences already render `sons of Israel` (`0` `Israelites`).
- **All 932 Ketiv/Qere verses & 12 Qere-wela-Ketiv `[...]` verses:** Followed Qere consistently; added missing Qere-wela-Ketiv notes at `2 Sam 18:20` (`HEB-P1-003`) and `Ruth 3:17` (`HEB-P1-004`).
- **All 131 Psalm & Habakkuk superscriptions:** 100% present and faithful; proposed capitalizing `miktam`→`Miktam` (`Ps 16:1, 60:1`: `HEB-P1-071`, `HEB-P1-072`) and `maskil`→`Maskil` (`Ps 74:1, 78:1`: `HEB-P1-073`, `HEB-P1-074`) and cross-referencing `Shoshannim` (`Ps 45:1`: `HEB-P1-075`) with `Lilies` (`Ps 69:1, 80:1`).
- **Multi-chapter quote check:** Confirmed `Num 28:2–29:39` is valid; caught premature quote close/re-open across uninterrupted divine speech in `Exod 25:40–30:1` (`HEB-P1-076`, `HEB-P1-077`).
- **Syntax catch:** Fixed ungrammatical participle splice in `Lev 20:3` (`לְמַעַן טַמֵּא... וּלְחַלֵּל...`) (`HEB-P1-056`).

### B. All 5 Biblical Aramaic Pericopes (269 Verses — 100% Line-by-Line Read)
- Audited every verse of `Gen 31:47` (1 v), `Jer 10:11` (1 v), `Ezra 4:8–6:18` (67 vv), `Ezra 7:12–26` (15 vv), and `Dan 2:4–7:28` (185 vv).
- Translation fidelity to MT Aramaic is exceptionally high (including Qere forms, `Ezra 5:4` 1cp `אֲמַרְנָא`, `Ezra 6:4` `חֲדַת`, `Ezra 6:6` 3mp `כְּנָוָתְהוֹן`, `Dan 5` court formulas, `Dan 7` vision terms).
- **Findings caught:** `Dan 2:43` stale note quote (`HEB-P1-009`); `Dan 5:14` `נַהִירוּ` inconsistent with `5:11` 3 verses earlier (`HEB-P1-069`); `Dan 3:31–33` & `4:1–34` Rule 2 ordering & `4:4, 4:5, 4:32` key collisions (`HEB-P1-038`, `HEB-P1-039`); `Dan 7:13–14, 27` capitalization queued (`HEB-HQ-032`).

### C. Notes Audit (All 4,270 Notes: 4,210 Placed + 60 Unplaced)
- **2 Critical False Notes Caught:** `Joshua 10:14` (falsely claims MT `10:15` & `10:43` are absent from the critical Hebrew text, `HEB-P1-005`) and `Exodus 38:31` / Saints `39:8` (falsely blames Hebrew order for Saints slot inversion, `HEB-P1-006`).
- **1 Inaccurate Witness Provenance Note:** `Joshua 21:36` (`⟦ ⟧`) — corrected to exact Studio provenance (`MAM Aleppo` / B19A original body / `Letteris 1852` vs. `WLC [L]` / `Ben Chayyim 1525`, `HEB-P1-007`, `HEB-HQ-003`).
- **2 Stale Note Quotes Across All 4,270 Notes:** `Genesis 8:21` (`HEB-P1-008`) and `Daniel 2:43` (`HEB-P1-009`).
- **3 OT Notes Citing NT Passages (Strict Isolation Flag):** `Jeremiah 31:32` (Saints `38:32`, cites Heb 8:9), `Joel 3:1` (cites Acts 2:17), `Amos 9:12` (cites Acts 15:17) (`HEB-P1-011`–`HEB-P1-013`, `HEB-HQ-002`). Additionally documented **310 notes** mentioning ancient versions (Septuagint/Vulgate/Syriac/Targum) for human editorial policy review.
- **Metadata drift:** 17 book JSONs omit the 60 `unplaced[].note` entries from `noteCount` (4,210 vs. 4,270 actual), and `Modern-English-OT/README.md` still cites stale `261` instead of `293` unplaced verses (`HEB-P1-078`).

### D. Within-Hebrew Lexical Variation Inventory (Pass 2/3 Awareness)
- **Targeted harmonization proposals raised:** `Lebo-hamath` (`1 Kgs 8:65`, `Ezek 47:20` — `HEB-P1-067`, `HEB-P1-068`); `Joshua 19` boundary terms seam (`19:14, 22, 29, 33` — `HEB-P1-070`); `Dan 5:14` `נַהִירוּ` (`HEB-P1-069`).
- **Context-sensitive variation documented (not force-flattened in Pass 1):** `גֵּר` (`resident alien` 33 / `sojourner` 31 / `foreign resident` 3 / `stranger` 1), `נָשִׂיא` (`leader` 62 / `prince` 34 / `chieftain` 2 / `ruler` 1), `קָדֵשׁ` (`male cult prostitute` 3 / `male shrine prostitute` 2 / `shrine prostitute` 3), `פָּדָה` (`redeem` 24 / `ransom` 9), `מַצֵּבָה` (`pillar` 22 / `standing stone` 8 / `sacred pillar` 2), `טָמֵא` (`unclean` 130 / `impure` 3), `אֲהָהּ` (`Alas` 9 / `Ah` 6), `דֶּבֶר` (`pestilence` 26 / `plague` 6+).

---

## 5. Rule 4 Ambiguity Preservation & Human Editorial Queue

1. **Bare `רוּחַ` & `Spirit` Capitalization (`HEB-P1-045`–`HEB-P1-053`, `HEB-HQ-005`–`HEB-HQ-009`):**
   - All 8 anarthrous visionary Ezekiel loci (`2:2, 3:12, 14, 24; 8:3; 11:1, 24; 43:5`) and `Isa 32:15` read lowercase `a spirit`. Added missing Rule 4 footnotes on `Ezek 8:3, 11:1, 11:24, 43:5` and `Isa 32:15`, and updated `Ezek 2:2` cross-references.
   - Added Rule 4 footnotes / editorial flags on articular `הָרוּחַ` (`Num 11:17, 25, 26`), appositional `רוּחַ` (`Isa 11:2`), and internal inconsistency `Ps 51:13` (`Your holy Spirit`) vs. `Isa 63:10–11` (`His Holy Spirit`).
2. **Contextual `זֶרַע` (`seed` vs. `offspring`) (`HEB-P1-054`–`HEB-P1-059`, `HEB-HQ-010`–`HEB-HQ-011`):**
   - Restored balanced collective/individual ambiguity wording in `Gen 3:15` footnote (`HEB-P1-054`) and added singular-echo note at `Gen 22:17` (`HEB-P1-055`).
   - Preserves `seed` in all covenantal/wordplay loci (`Gen 3:15`, Abrahamic/Davidic promises, `Lev 18:21` echo of `18:20`, `Isa 6:13, 53:10`, `Mal 2:15`, `Dan 2:43`) while flagging biologically/idiomatically jarring non-echo contexts (`Lev 20:2–4`, `Lev 22:13`, `1 Sam 1:11`, `Dan 9:1`) for human editor decision.
3. **Messianic & Disputed Capitalization Queue (`HEB-HQ-021`–`HEB-HQ-041`):**
   - Audited and queued all requested Messianic/disputed loci: `Ps 2:2,7,12`; `Ps 16:10`; `Ps 45:7–8`; `Ps 110:1,5,7`; `Isa 4:2, 7:14, 9:5–6, 11:1–10, 52:13–53:12, 61:1`; `Jer 23:5` vs. `Jer 33:15` (internal `Branch`/`branch` capitalization mismatch: `HEB-P1-064`, `HEB-HQ-030`!); `Dan 7:13–14, 27`, `Dan 9:25–26`; `Mic 5:1–5`; `Zech 3:8, 6:12, 9:9, 12:10`; `Mal 3:1` (lowercase `messenger of the covenant` paired with capitalized `He is coming`); plus `Gen 48:16, 49:24`, `Exod 23:20–21`, `Deut 18:15,18`, `Josh 5:14`, `Job 1:6` / `1 Chr 21:1` vs. `Zech 3:1`, `Job 19:25`, `Eccl 12:11`.
4. **All 7 Hebraist Judgment Calls + `Esth 2:9,17` & `Dan 1:9` (`HEB-HQ-012`–`HEB-HQ-020`):**
   - Verified all 7 (`Dan 9:26`, `Dan 9:27`, `Ezek 41:6`, `Zeph 1:5`, `Isa 40:6`, `Mic 6:8`, `Song 8:3`, `Exod 12:42`) plus `Esth 2:9,17` and `Dan 1:9`; added missing Rule 4 notes for `Dan 9:26`, `Dan 9:27`, `Song 8:3`, `Mic 6:8`, `Esth 2:9`, `Dan 1:9` (`HEB-P1-060`–`HEB-P1-066`).

---

## 6. Per-Book Pass 1 Coverage Table (All 39 MT Books)

| # | Book | Chs | Source Total | Placed | Unplaced | Verified | Disputed | Unverified |
|---:|---|---:|---:|---:|---:|---:|---:|---:|
| 1 | Genesis | 50 | 1,533 | 1,531 | 2 | 1,525 | 8 | 0 |
| 2 | Exodus | 40 | 1,213 | 1,155 | 55 | 1,163 | 50 | 0 |
| 3 | Leviticus | 27 | 859 | 859 | 0 | 853 | 6 | 0 |
| 4 | Numbers | 36 | 1,289 | 1,287 | 1 | 1,234 | 55 | 0 |
| 5 | Deuteronomy | 34 | 959 | 959 | 0 | 953 | 6 | 0 |
| 6 | Joshua | 24 | 658 | 643 | 15 | 643 | 15 | 0 |
| 7 | Judges | 21 | 618 | 618 | 0 | 618 | 0 | 0 |
| 8 | Ruth | 4 | 85 | 85 | 0 | 84 | 1 | 0 |
| 9 | 1 Samuel | 31 | 811 | 772 | 39 | 810 | 1 | 0 |
| 10 | 2 Samuel | 24 | 695 | 695 | 0 | 694 | 1 | 0 |
| 11 | 1 Kings | 22 | 817 | 754 | 33 | 810 | 7 | 0 |
| 12 | 2 Kings | 25 | 719 | 718 | 1 | 719 | 0 | 0 |
| 13 | 1 Chronicles | 29 | 943 | 930 | 13 | 942 | 1 | 0 |
| 14 | 2 Chronicles | 36 | 822 | 821 | 1 | 822 | 0 | 0 |
| 15 | Ezra | 10 | 280 | 280 | 0 | 280 | 0 | 0 |
| 16 | Nehemiah | 13 | 405 | 391 | 14 | 405 | 0 | 0 |
| 17 | Esther | 10 | 167 | 164 | 3 | 165 | 2 | 0 |
| 18 | Job | 42 | 1,070 | 1,069 | 1 | 1,067 | 3 | 0 |
| 19 | Psalms | 150 | 2,527 | 2,526 | 1 | 2,511 | 16 | 0 |
| 20 | Proverbs | 31 | 915 | 888 | 19 | 910 | 5 | 0 |
| 21 | Ecclesiastes | 12 | 222 | 222 | 0 | 221 | 1 | 0 |
| 22 | Song of Songs | 8 | 117 | 117 | 0 | 116 | 1 | 0 |
| 23 | Lamentations | 5 | 154 | 150 | 4 | 154 | 0 | 0 |
| 24 | Isaiah | 66 | 1,291 | 1,289 | 2 | 1,257 | 34 | 0 |
| 25 | Jeremiah | 52 | 1,364 | 1,296 | 68 | 1,328 | 36 | 0 |
| 26 | Ezekiel | 48 | 1,273 | 1,266 | 6 | 1,255 | 18 | 0 |
| 27 | Daniel | 12 | 357 | 339 | 15 | 335 | 22 | 0 |
| 28 | Hosea | 14 | 197 | 197 | 0 | 197 | 0 | 0 |
| 29 | Joel | 4 | 73 | 73 | 0 | 72 | 1 | 0 |
| 30 | Amos | 9 | 146 | 146 | 0 | 145 | 1 | 0 |
| 31 | Obadiah | 1 | 21 | 21 | 0 | 21 | 0 | 0 |
| 32 | Jonah | 4 | 48 | 48 | 0 | 48 | 0 | 0 |
| 33 | Micah | 7 | 105 | 105 | 0 | 99 | 6 | 0 |
| 34 | Nahum | 3 | 47 | 47 | 0 | 47 | 0 | 0 |
| 35 | Habakkuk | 3 | 56 | 56 | 0 | 56 | 0 | 0 |
| 36 | Zephaniah | 3 | 53 | 53 | 0 | 52 | 1 | 0 |
| 37 | Haggai | 2 | 38 | 38 | 0 | 38 | 0 | 0 |
| 38 | Zechariah | 14 | 211 | 211 | 0 | 206 | 5 | 0 |
| 39 | Malachi | 3 | 55 | 55 | 0 | 51 | 4 | 0 |
| — | **TOTAL (39 MT Books)** | **929** | **23,213** | **22,874** | **293** | **22,906** | **307** | **0** |

---

## 7. Pass 2 Handoff Checklist

- Every entry in `pass1_proposals.jsonl` carries all 13 required traceability fields (`id`, `book`, `native_ref`, `saints_ref`, `source_phrase`, `source_edition`, `current_english`, `proposed_english`, `current_note`, `proposed_note`, `reason`, `category`, `needs_human_editor`).
- **Immediate high-confidence fixes ready for Pass 2 verification:** false notes (`Josh 10:14`, `Exod 38:31`), stale note quotes (`Gen 8:21`, `Dan 2:43`), Stage 1 drift follow-ups (`Job 7:5`, `Jer 39:12`), Qere-wela-Ketiv notes (`2 Sam 18:20`, `Ruth 3:17`), `Lev 20:3` grammar splice, `Lev 11:5–6` missed `verse-map.json` entry, Rule 4 bare `רוּחַ` notes (`Ezek 2:2, 8:3, 11:1, 11:24, 43:5`), `Gen 22:17` `זֶרַע` note, `Lebo-hamath` (`1 Kgs 8:65`, `Ezek 47:20`), `Dan 5:14` `נַהִירוּ`, `Ps 16:1/60:1/74:1/78:1` superscription capitals, `Exod 25:40–30:1` quote frame, and JSON `noteCount` / `README.md` metadata.
- **Escalate to qualified human editor before edits:** Rule 2 dual-key schema adoption (`HEB-HQ-001`), OT-note NT/non-MT citation policy (`HEB-HQ-002`), `Josh 21:36–37` `⟦ ⟧` & `Ps 24:4` witness decisions (`HEB-HQ-003`–`HEB-HQ-004`), `Isa 32:15` / `Ps 51:13` / `Isa 11:2` / `Num 11:17` Spirit capitalization (`HEB-HQ-006`–`HEB-HQ-009`), `Gen 3:15` & contextual `זֶרַע` (`HEB-HQ-010`–`HEB-HQ-011`), Hebraist judgment calls (`HEB-HQ-012`–`HEB-HQ-020`), and Messianic/disputed capitalization (`HEB-HQ-021`–`HEB-HQ-041`).
