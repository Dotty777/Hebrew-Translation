# Stage 2 Pass 3 — Standalone English Clarity & Flow Review Summary (Hebrew-Based Edition)

- **Reviewer:** `@heb-flow` (Independent Standalone English Clarity & Flow Reviewer)
- **Baseline HEAD:** `23580fa3d1e52477c502152f4dfec3a9f9613a07` (branch `review/2026-11-24-literal-smooth`)
- **Isolation Guarantee:** Read **strictly** standalone English files inside `Hebrew-Translation/Modern-English-OT/` (`STYLE.md`, `glossary.json`, `README.md`, `parallel-verse-map.json`, all 39 `json/*.json`, and `markdown/*/chapter-*.md`) plus `review-charter.md`. Zero inspection of `Saints-Hebrew-Critical-Text/`, `Greek-Translation/`, `Latin-Translation/`, or prior Pass 1/2 review files.
- **Corpus Scope Audited:** **39 / 39 books**, **929 / 929 Markdown chapters**, **22,874 placed verses** (`verses`), **293 additional MT verses** (`unplaced`), **23,213 native MT verses** (`native_verses`), and translator notes.

---

## 1. Full-Corpus Programmatic Mechanics & Quotation Sweeps

All 39 books (both native MT order `native_verses` and Saints parallel order `verses`, plus `unplaced` and all 929 Markdown chapter files) were audited via automated checks:

| Check Category | Pre-Edit Findings | Disposition | Post-Edit Status |
|---|---:|---|---|
| JSON schema counts (`verseCount`, `nativeVerseCount`, `unplacedCount`, `noteCount`) | 0 errors | Clean | **0 errors** |
| JSON ↔ Markdown sync (`verses`, `unplaced`, `notes`) | 0 mismatches | Clean | **0 mismatches** |
| Double spaces, leading/trailing spaces, tabs, newlines, NBSP/ZWSP | 0 | Clean | **0** |
| Curly/smart quotes (`“”‘’`), stray Markdown/HTML, Arabic digits, non-Latin script | 0 (2 intentional `⟦ ⟧` in Josh 21:36–37) | Clean | **0 glitches** |
| Banned archaisms per `STYLE.md` / `glossary.json` | 0 | Clean | **0** |
| Archaic vocative `"O ..."` | 1 (`1 Sam 17:55` unplaced) | **Bucket A (`P3A-001`)** | **0** |
| British spellings (`-our`, `-re`, `-ll-`, etc.) | 0 | Clean | **0** |
| Orthographic inconsistencies (`ax` vs `axe`; `brickkiln` vs `brick kiln`) | 2 (`Isa 10:15`, `2 Sam 12:31`) | **Bucket A (`P3A-002`, `P3A-006`)** | **0** |
| Disallowed proper-name spellings per `glossary.json` | 1 (`Deut 4:48` Mount Sion = Hermon, explicitly noted as Hebrew-distinct `Si'on`) | Verified intentional | **0 errors** |
| Doubled consecutive words | 1 (`Hos 2:17` `"give her her vineyards"`, grammatical indirect+possessive) | Verified grammatical | **0 errors** |
| Malformed `? declares` (lowercase `declares` after `?` inside open quote) | 3 (`Jer 22:16`, `Jer 30:21`, `Ezek 21:18`) | **Bucket A (`P3A-007`–`P3A-011`)** | **0** |
| Lowercase continuation after sentence-end period (non-quoted-question) | 4 (`Ps 104:2->3`, `Esth 9:29/30->31`, `Exod 39:34->35`, `Jer 29:20->21`) | 1 **Bucket A (`P3A-005`)**, 3 **Bucket B (`P3B-006`, `P3B-007`, `P3B-010`)** | **0 Bucket A remaining** |
| 3-level stack-based quotation errors (native MT order) | 2 (`Exod 32:9`, `Jer 11:7` — both at `unplaced` seams) | **Bucket B (`P3B-001`, `P3B-002`)** | Routed to `@heb-peer` |
| Chapter breaks with open quotes (stack-based, native MT order) | 9 (`Job 13:28->14:1`, `Exod 21–23` [2], `Exod 25–30` [5], `Num 28–29` [1]) | 1 **Bucket A (`P3A-003`–`P3A-004`)**, 8 **Bucket B (`P3B-008`, `P3B-009`, `P3B-012`)** | **8** (all routed to `@heb-peer`) |
| Unquoted multi-chapter speech / speaker-boundary anomalies | 4 (`Job 30–31`, `Job 28`, `Lev 7:1–21` + nested breaks, `Deut 32:27–35`) | **Bucket B (`P3B-003`, `P3B-004`, `P3B-011`, `P3B-013`)** | Routed to `@heb-peer` |
| Unplaced Jeremiah first-person divine speech orphaned after closed `"` | 6 passages (`Jer 30:10–11, 30:22, 46:26, 48:45–47, 49:6, 51:45–48`) | **Bucket B (`P3B-014`)** | Routed to `@heb-peer` |
| Broken cross-verse English syntax (`and to prepare`) | 1 (`2 Chr 2:7–8`) | **Bucket B (`P3B-005`)** | Routed to `@heb-peer` |

---

## 2. Priority Dialogue & Quotation Loci Audited

- **Genesis 31 (`31:51–53`):** Verified clean & documented. Native MT order (`31:51` open `"` → `31:53` close `"`) is 100% balanced; Saints order detaches `31:51` under `Additional Verses` and already carries explicit translator notes on `31:52` and `31:51 (additional)` explaining the speech boundary.
- **Exodus 21–23 (`21:1–23:33`):** Continuous unclosed `"` across `21:37->22:1` and `22:30->23:1` (contrasting with `20:26->21:1` close+reopen immediately prior). Routed to `@heb-peer` (`P3B-009`).
- **Exodus 25:40–30:1 (`25:2–30:10`):** Five consecutive chapter breaks leave `"` unclosed (`25:40->26:1`, `26:37->27:1`, `27:21->28:1`, `28:43->29:1`, `29:46->30:1`), so standalone `chapter-26.md`–`chapter-29.md` lack enclosing double quotes (making `28:36` `'Holiness to the LORD.'` appear top-level single-quoted in `chapter-28.md`). Routed to `@heb-peer` (`P3B-008`).
- **Leviticus (all 27 chapters):** `Lev 7:1–21` drops quotation marks entirely between `6:23` (`'"`) and `7:22` (`And the LORD spoke...`); `Lev 5:1–13` reopens `"'` across a chapter break while `Lev 2–3` and `Lev 26` reopen only `"`. Routed to `@heb-peer` (`P3B-011`).
- **Numbers 28–29 (`28:31->29:1`):** Both `"` and `'` stay unclosed across the chapter break until `29:39` (`'"`). Routed to `@heb-peer` (`P3B-012`).
- **Deuteronomy 32:28–34 (`32:27–35`):** `32:27` closes `"`, `32:28–33` stands unquoted (including Israel/Moses voice `"our Rock"` in `32:31`), and `32:34` abruptly opens `"` (`"Is it not stored away with Me..."`) with no speech-intro formula and no translator note explaining the speaker transitions/referents. Routed to `@heb-peer` (`P3B-004`).
- **Job (all 42 chapters):**
  - 10 of 11 quoted multi-chapter speeches (`4–5`, `6–7`, `9–10`, `12–13`, `16–17`, `23–24`, `32–33`, `36–37`, `38–39`, `40–41`) consistently close `"` at chapter end and reopen `"` at the next chapter.
  - **`Job 13:28 -> 14:1`** was the sole exception within Job (inside the same `12:1–14:22` speech where `12:25->13:1` closed+reopened) → fixed mechanically in **Bucket A (`P3A-003`, `P3A-004`)**.
  - **`Job 30:1–31:40`** omits outer quotes entirely after `29:25`, leaving `31:24`/`31:31` in double quotes and running `31:40a` straight into the narrator colophon `The words of Job are finished.` without a closing quote → routed to `@heb-peer` (**Bucket B `P3B-003`**).
  - **`Job 28:1–28`** stands unquoted between `27:23` and `29:1` with debated speaker attribution and no note on `28:1` → routed to `@heb-peer` (**Bucket B `P3B-013`**).
- **Song of Songs (all 8 chapters / 117 verses):** Verified clean. All 5 embedded speeches (`2:10–14`, `3:2`, `3:3`, `5:2`, `7:9`) are strictly balanced; dialogue speaker transitions remain appropriately unmarked without interpretive headings.
- **Isaiah (all 66 chapters):** Verified quote-balanced across all 66 chapters (0 stack errors). One orthographic polish (`Isa 10:15` `ax` → `axe`, `P3A-006`).
- **Jeremiah (all 52 chapters):** Fixed `? declares` punctuation in `Jer 22:16–17` and `Jer 30:21` (Bucket A); routed `Jer 11:6–8` quote-stack/addressee error (`P3B-002`), `Jer 29:15–21` unplaced capitalization seam (`P3B-007`), and 6 unplaced oracle-endpoint loci (`P3B-014`) to `@heb-peer`.
- **Ezekiel (all 48 chapters):** Verified quote-balanced across all 48 chapters (0 stack errors). Fixed `? declares` punctuation in `Ezek 21:18–19` (Bucket A).

---

## 3. Standalone Literal-Smooth Prose, Poetry & Prophecy Reading

Substantial full-chapter standalone reads were conducted across all four divisions and every major genre:
- **I. Law:** `Genesis 1, 22, 31`; `Exodus 15, 28`; `Leviticus 19`; `Numbers 22`; `Deuteronomy 6, 32`
- **II. Judgement:** `Joshua 24`; `Judges 5`; `Ruth 1`; `1 Samuel 17`; `2 Samuel 12`; `1 Kings 18`; `Nehemiah 8`; `Job 38`
- **III. Wisdom:** `Psalms 50 (MT 51)`; `Proverbs 8`; `Ecclesiastes 3`; `Song of Songs 2`; `Lamentations 3`
- **IV. Providence:** `Isaiah 53`; `Jeremiah 38 (MT 31)`; `Ezekiel 36`; `Daniel 7` (Biblical Aramaic); `Hosea 2`; `Amos 5`; `Jonah 2`; `Habakkuk 3`; `Zechariah 3`; `Malachi 3`

**Overall Clarity & Flow Assessment:** Standalone English quality is consistently high across prose, legal codes, poetry, wisdom, prophecy, and Biblical Aramaic. Literal formal equivalence is preserved without unnatural "translationese," archaisms, or paraphrastic expansion; rare/difficult idioms are smoothly integrated with clear translator notes.

---

## 4. Deliverables & Counts

- **Bucket A Applied (`pass3_surface_edits.jsonl`):** **11 verse edits** (`meaning_changed=false`, `resolves_ambiguity=false`) across **7 JSON book files** and **9 Markdown chapter files** (16 files modified, 36 insertions / 36 deletions; `verses`, `native_verses`, `unplaced`, `notes`, and `.md` chapters 100% synced, **0 schema errors**):
  - `P3A-001`: `1 Samuel 17:55` (unplaced) — archaic vocative `"O king"` → `"king"`
  - `P3A-002`: `2 Samuel 12:31` (+ note) — `"brickkiln"` → `"brick kiln"`
  - `P3A-003`–`P3A-004`: `Job 13:28`, `14:1` — mechanical chapter-break quote balance matching `Job 12:25->13:1` and all other Job chapter breaks
  - `P3A-005`: `Psalms 104:2` (`saints 103:2`) — terminal `.` → `,` before lowercase `who lays...` in `104:3` (`103:3`)
  - `P3A-006`: `Isaiah 10:15` — `"ax"` → `"axe"`
  - `P3A-007`–`P3A-008`: `Jeremiah 22:16–17` — `? declares the LORD.` → `?" declares the LORD.` + reopened `"`
  - `P3A-009`: `Jeremiah 30:21` (`saints 37:21`) — `? declares the LORD."` → `?" declares the LORD.`
  - `P3A-010`–`P3A-011`: `Ezekiel 21:18–19` — `? declares the Lord GOD.` → `?" declares the Lord GOD.` + reopened `"`
- **Bucket B Routed to `@heb-peer` (`pass3_bounceback.jsonl`):** **14 structured bounce-back items** (`7 high`, `7 medium`; `meaning_changed=true` or `resolves_ambiguity=true`) — NOT applied by `@heb-flow`; routed to `@heb-peer` for independent verification against `Saints-Hebrew-Critical-Text/`.
