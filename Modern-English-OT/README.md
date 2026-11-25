# Saints Modern English — Old Testament (Hebrew & Biblical Aramaic)

> **Status:** `draft: true` — **100.00% Complete & Post-Audit Polished**  
> **Coverage:** **ALL 39/39 Hebrew & Aramaic Bible books** (929 chapters, **22,874** placed verses + **293** additional `no-site-verse` MT verses = **23,167 total verses**, **4,314** translator notes [4,251 verse + 63 additional]).  
> **Validation:** `validate_modern_english.py --corpus full --lang heb --include-missing` **929/929 PASS, 0 FAIL**; 0 hard/soft archaisms, 0 `"Thus says"`, 0 ketiv/qere leaks, 0 Arabic digits.

## Overview

This directory contains the complete **Saints Modern English** translation of the Hebrew Bible (Masoretic Hebrew & Biblical Aramaic), translated fresh from `Saints-Hebrew-Critical-Text` under the locked style policy ([`STYLE.md`](STYLE.md)) and shared term glossary ([`glossary.json`](glossary.json)).

- **Method:** Formal-equivalent (literal) Modern English smoothed for natural reading, with zero archaisms, own-source Masoretic fidelity (`יהוה` → `the LORD`, `אֲדֹנָי יֱהֹוִה` → `the Lord GOD`, *qere* rendered cleanly), and original wording.
- **Additional MT verses (`unplaced`):** All **293 `no-site-verse` MT verses** (across 17 books / 75 chapters, incl. Lam 3:22–24/29, Prov 4:7/16:3/22:6, Isa 2:22, Ps 116:14, 1 Sam 13:1, Jer 33:14–26, Dan 4–6 Aramaic) are included in book `json/*.json` (`unplaced` + `unplacedCount`) and chapter Markdown (`## Additional Verses (Not in Saints Numbering)`).
- **Related directory:** Original reviewed 6-passage Hebrew/Aramaic pilot in [`../Modern-English-Pilot/`](../Modern-English-Pilot/README.md).

## Divisions

| Division | Status | Books | Chapters | Verses | Additional | Notes | Directory |
|---|---|---:|---:|---:|---:|---:|---|
| **I. Law (Pentateuch / Torah)** | **Complete** | 5 / 5 | 187 | 5,791 | 58 | 902 | [`I-Law/`](I-Law/README.md) |
| **II. Judgement (Historical Books & Job)** | **Complete** | 13 / 13 | 291 | 7,940 | 120 | 1,360 | [`II-Judgement/`](II-Judgement/README.md) |
| **III. Wisdom (Wisdom & Poetry)** | **Complete** | 5 / 5 | 206 | 3,903 | 24 | 883 | [`III-Wisdom/`](III-Wisdom/README.md) |
| **IV. Providence (Prophets)** | **Complete** | 16 / 16 | 245 | 5,240 | 91 | 1,169 | [`IV-Providence/`](IV-Providence/README.md) |

## Division I. Law (5 / 5 Complete)

| # | Book | Chapters | Verses | Additional | Notes | Reading Edition | Book JSON |
|---:|---|---:|---:|---:|---:|---|---|
| 1 | Genesis | 50 | 1,531 | 2 | 254 | [`I-Law/markdown/01-genesis/`](I-Law/markdown/01-genesis/README.md) | [`01-genesis.json`](I-Law/json/01-genesis.json) |
| 2 | Exodus | 40 | 1,155 | 55 | 186 | [`I-Law/markdown/02-exodus/`](I-Law/markdown/02-exodus/README.md) | [`02-exodus.json`](I-Law/json/02-exodus.json) |
| 3 | Leviticus | 27 | 859 | — | 125 | [`I-Law/markdown/03-leviticus/`](I-Law/markdown/03-leviticus/README.md) | [`03-leviticus.json`](I-Law/json/03-leviticus.json) |
| 4 | Numbers | 36 | 1,287 | 1 | 178 | [`I-Law/markdown/04-numbers/`](I-Law/markdown/04-numbers/README.md) | [`04-numbers.json`](I-Law/json/04-numbers.json) |
| 5 | Deuteronomy | 34 | 959 | — | 159 | [`I-Law/markdown/05-deuteronomy/`](I-Law/markdown/05-deuteronomy/README.md) | [`05-deuteronomy.json`](I-Law/json/05-deuteronomy.json) |

## Division II. Judgement (13 / 13 Complete)

| # | Book | Chapters | Verses | Additional | Notes | Reading Edition | Book JSON |
|---:|---|---:|---:|---:|---:|---|---|
| 6 | Joshua | 24 | 643 | 15 | 114 | [`II-Judgement/markdown/06-joshua/`](II-Judgement/markdown/06-joshua/README.md) | [`06-joshua.json`](II-Judgement/json/06-joshua.json) |
| 7 | Judges | 21 | 618 | — | 96 | [`II-Judgement/markdown/07-judges/`](II-Judgement/markdown/07-judges/README.md) | [`07-judges.json`](II-Judgement/json/07-judges.json) |
| 8 | Ruth | 4 | 85 | — | 19 | [`II-Judgement/markdown/08-ruth/`](II-Judgement/markdown/08-ruth/README.md) | [`08-ruth.json`](II-Judgement/json/08-ruth.json) |
| 9 | 1 Samuel | 31 | 772 | 39 | 147 | [`II-Judgement/markdown/09-1-samuel/`](II-Judgement/markdown/09-1-samuel/README.md) | [`09-1-samuel.json`](II-Judgement/json/09-1-samuel.json) |
| 10 | 2 Samuel | 24 | 695 | — | 115 | [`II-Judgement/markdown/10-2-samuel/`](II-Judgement/markdown/10-2-samuel/README.md) | [`10-2-samuel.json`](II-Judgement/json/10-2-samuel.json) |
| 11 | 1 Kings | 22 | 754 | 33 | 114 | [`II-Judgement/markdown/11-1-kings/`](II-Judgement/markdown/11-1-kings/README.md) | [`11-1-kings.json`](II-Judgement/json/11-1-kings.json) |
| 12 | 2 Kings | 25 | 718 | 1 | 121 | [`II-Judgement/markdown/12-2-kings/`](II-Judgement/markdown/12-2-kings/README.md) | [`12-2-kings.json`](II-Judgement/json/12-2-kings.json) |
| 13 | 1 Chronicles | 29 | 930 | 13 | 141 | [`II-Judgement/markdown/13-1-chronicles/`](II-Judgement/markdown/13-1-chronicles/README.md) | [`13-1-chronicles.json`](II-Judgement/json/13-1-chronicles.json) |
| 14 | 2 Chronicles | 36 | 821 | 1 | 149 | [`II-Judgement/markdown/14-2-chronicles/`](II-Judgement/markdown/14-2-chronicles/README.md) | [`14-2-chronicles.json`](II-Judgement/json/14-2-chronicles.json) |
| 15 | Ezra | 10 | 280 | — | 50 | [`II-Judgement/markdown/15-ezra/`](II-Judgement/markdown/15-ezra/README.md) | [`15-ezra.json`](II-Judgement/json/15-ezra.json) |
| 16 | Nehemiah | 13 | 391 | 14 | 64 | [`II-Judgement/markdown/16-nehemiah/`](II-Judgement/markdown/16-nehemiah/README.md) | [`16-nehemiah.json`](II-Judgement/json/16-nehemiah.json) |
| 17 | Esther | 10 | 164 | 3 | 38 | [`II-Judgement/markdown/17-esther/`](II-Judgement/markdown/17-esther/README.md) | [`17-esther.json`](II-Judgement/json/17-esther.json) |
| 20 | Job | 42 | 1,069 | 1 | 192 | [`II-Judgement/markdown/20-job/`](II-Judgement/markdown/20-job/README.md) | [`20-job.json`](II-Judgement/json/20-job.json) |

## Division III. Wisdom (5 / 5 Complete)

| # | Book | Chapters | Verses | Additional | Notes | Reading Edition | Book JSON |
|---:|---|---:|---:|---:|---:|---|---|
| 21 | Psalms | 150 | 2,526 | 1 | 610 | [`III-Wisdom/markdown/21-psalms/`](III-Wisdom/markdown/21-psalms/README.md) | [`21-psalms.json`](III-Wisdom/json/21-psalms.json) |
| 22 | Proverbs | 31 | 888 | 19 | 156 | [`III-Wisdom/markdown/22-proverbs/`](III-Wisdom/markdown/22-proverbs/README.md) | [`22-proverbs.json`](III-Wisdom/json/22-proverbs.json) |
| 23 | Ecclesiastes | 12 | 222 | — | 52 | [`III-Wisdom/markdown/23-ecclesiastes/`](III-Wisdom/markdown/23-ecclesiastes/README.md) | [`23-ecclesiastes.json`](III-Wisdom/json/23-ecclesiastes.json) |
| 24 | Song of Songs | 8 | 117 | — | 35 | [`III-Wisdom/markdown/24-song-of-songs/`](III-Wisdom/markdown/24-song-of-songs/README.md) | [`24-song-of-songs.json`](III-Wisdom/json/24-song-of-songs.json) |
| 25 | Lamentations | 5 | 150 | 4 | 30 | [`III-Wisdom/markdown/25-lamentations/`](III-Wisdom/markdown/25-lamentations/README.md) | [`25-lamentations.json`](III-Wisdom/json/25-lamentations.json) |

## Division IV. Providence (16 / 16 Complete)

| # | Book | Chapters | Verses | Additional | Notes | Reading Edition | Book JSON |
|---:|---|---:|---:|---:|---:|---|---|
| 28 | Isaiah | 66 | 1,289 | 2 | 294 | [`IV-Providence/markdown/28-isaiah/`](IV-Providence/markdown/28-isaiah/README.md) | [`28-isaiah.json`](IV-Providence/json/28-isaiah.json) |
| 29 | Jeremiah | 52 | 1,296 | 68 | 260 | [`IV-Providence/markdown/29-jeremiah/`](IV-Providence/markdown/29-jeremiah/README.md) | [`29-jeremiah.json`](IV-Providence/json/29-jeremiah.json) |
| 30 | Ezekiel | 48 | 1,266 | 6 | 229 | [`IV-Providence/markdown/30-ezekiel/`](IV-Providence/markdown/30-ezekiel/README.md) | [`30-ezekiel.json`](IV-Providence/json/30-ezekiel.json) |
| 31 | Daniel | 12 | 339 | 15 | 87 | [`IV-Providence/markdown/31-daniel/`](IV-Providence/markdown/31-daniel/README.md) | [`31-daniel.json`](IV-Providence/json/31-daniel.json) |
| 32 | Hosea | 14 | 197 | — | 59 | [`IV-Providence/markdown/32-hosea/`](IV-Providence/markdown/32-hosea/README.md) | [`32-hosea.json`](IV-Providence/json/32-hosea.json) |
| 33 | Joel | 4 | 73 | — | 17 | [`IV-Providence/markdown/33-joel/`](IV-Providence/markdown/33-joel/README.md) | [`33-joel.json`](IV-Providence/json/33-joel.json) |
| 34 | Amos | 9 | 146 | — | 42 | [`IV-Providence/markdown/34-amos/`](IV-Providence/markdown/34-amos/README.md) | [`34-amos.json`](IV-Providence/json/34-amos.json) |
| 35 | Obadiah | 1 | 21 | — | 5 | [`IV-Providence/markdown/35-obadiah/`](IV-Providence/markdown/35-obadiah/README.md) | [`35-obadiah.json`](IV-Providence/json/35-obadiah.json) |
| 36 | Jonah | 4 | 48 | — | 17 | [`IV-Providence/markdown/36-jonah/`](IV-Providence/markdown/36-jonah/README.md) | [`36-jonah.json`](IV-Providence/json/36-jonah.json) |
| 37 | Micah | 7 | 105 | — | 32 | [`IV-Providence/markdown/37-micah/`](IV-Providence/markdown/37-micah/README.md) | [`37-micah.json`](IV-Providence/json/37-micah.json) |
| 38 | Nahum | 3 | 47 | — | 15 | [`IV-Providence/markdown/38-nahum/`](IV-Providence/markdown/38-nahum/README.md) | [`38-nahum.json`](IV-Providence/json/38-nahum.json) |
| 39 | Habakkuk | 3 | 56 | — | 15 | [`IV-Providence/markdown/39-habakkuk/`](IV-Providence/markdown/39-habakkuk/README.md) | [`39-habakkuk.json`](IV-Providence/json/39-habakkuk.json) |
| 40 | Zephaniah | 3 | 53 | — | 15 | [`IV-Providence/markdown/40-zephaniah/`](IV-Providence/markdown/40-zephaniah/README.md) | [`40-zephaniah.json`](IV-Providence/json/40-zephaniah.json) |
| 41 | Haggai | 2 | 38 | — | 10 | [`IV-Providence/markdown/41-haggai/`](IV-Providence/markdown/41-haggai/README.md) | [`41-haggai.json`](IV-Providence/json/41-haggai.json) |
| 42 | Zechariah | 14 | 211 | — | 57 | [`IV-Providence/markdown/42-zechariah/`](IV-Providence/markdown/42-zechariah/README.md) | [`42-zechariah.json`](IV-Providence/json/42-zechariah.json) |
| 43 | Malachi | 3 | 55 | — | 15 | [`IV-Providence/markdown/43-malachi/`](IV-Providence/markdown/43-malachi/README.md) | [`43-malachi.json`](IV-Providence/json/43-malachi.json) |
