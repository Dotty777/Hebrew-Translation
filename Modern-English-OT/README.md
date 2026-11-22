# Saints Modern English — Old Testament (Hebrew & Biblical Aramaic)

> **Status:** `draft: true` — Post-audit polished  
> **Current Coverage:** **18 of 39 Hebrew Bible books complete** (478 chapters, 13,731 verses, 2,206 translator notes).  
> **Validation:** 100% validated against `Saints-Hebrew-Critical-Text` with `validate_modern_english.py --lang heb --strict` and scholarly audits (`0` hard/soft failures).

## Overview

This directory contains the **Saints Modern English** translation of the Hebrew Bible (Masoretic Hebrew & Biblical Aramaic), translated fresh from `Saints-Hebrew-Critical-Text` under the locked style policy ([`STYLE.md`](STYLE.md)) and shared term glossary ([`glossary.json`](glossary.json)).

- **Method:** Formal-equivalent (literal) Modern English smoothed for natural reading, with zero archaisms, own-source Masoretic fidelity (`יהוה` → `the LORD`, `אֲדֹנָי יֱהֹוִה` → `the Lord GOD`, *qere* rendered cleanly), and original wording.
- **Saints.Bible versification:** Chapter and verse keys align with `Saints-Hebrew-Critical-Text` and the Saints.Bible Parallel Reader.
- **Related directory:** Original reviewed 6-passage Hebrew/Aramaic pilot in [`../Modern-English-Pilot/`](../Modern-English-Pilot/README.md).

## Divisions

| Division | Status | Books | Chapters | Verses | Notes | Directory |
|---|---|---:|---:|---:|---:|---|
| **I. Law (Pentateuch / Torah)** | **Complete** | 5 / 5 | 187 | 5,791 | 883 | [`I-Law/`](I-Law/README.md) |
| **II. Judgement (Historical Books & Job)** | **Complete** | 13 / 13 | 291 | 7,940 | 1,323 | [`II-Judgement/`](II-Judgement/README.md) |
| **III. Wisdom (Wisdom & Poetry)** | In progress | 0 / 5 | — | — | — | — |
| **IV. Providence (Prophets)** | In progress | 0 / 16 | — | — | — | — |

## Division I. Law (5 / 5 Complete)

| # | Book | Chapters | Verses | Notes | Reading Edition | Book JSON |
|---:|---|---:|---:|---:|---|---|
| 1 | Genesis | 50 | 1,531 | 251 | [`I-Law/markdown/01-genesis/`](I-Law/markdown/01-genesis/README.md) | [`01-genesis.json`](I-Law/json/01-genesis.json) |
| 2 | Exodus | 40 | 1,155 | 180 | [`I-Law/markdown/02-exodus/`](I-Law/markdown/02-exodus/README.md) | [`02-exodus.json`](I-Law/json/02-exodus.json) |
| 3 | Leviticus | 27 | 859 | 123 | [`I-Law/markdown/03-leviticus/`](I-Law/markdown/03-leviticus/README.md) | [`03-leviticus.json`](I-Law/json/03-leviticus.json) |
| 4 | Numbers | 36 | 1,287 | 174 | [`I-Law/markdown/04-numbers/`](I-Law/markdown/04-numbers/README.md) | [`04-numbers.json`](I-Law/json/04-numbers.json) |
| 5 | Deuteronomy | 34 | 959 | 155 | [`I-Law/markdown/05-deuteronomy/`](I-Law/markdown/05-deuteronomy/README.md) | [`05-deuteronomy.json`](I-Law/json/05-deuteronomy.json) |

## Division II. Judgement (13 / 13 Complete)

| # | Book | Chapters | Verses | Notes | Reading Edition | Book JSON |
|---:|---|---:|---:|---:|---|---|
| 6 | Joshua | 24 | 643 | 109 | [`II-Judgement/markdown/06-joshua/`](II-Judgement/markdown/06-joshua/README.md) | [`06-joshua.json`](II-Judgement/json/06-joshua.json) |
| 7 | Judges | 21 | 618 | 96 | [`II-Judgement/markdown/07-judges/`](II-Judgement/markdown/07-judges/README.md) | [`07-judges.json`](II-Judgement/json/07-judges.json) |
| 8 | Ruth | 4 | 85 | 18 | [`II-Judgement/markdown/08-ruth/`](II-Judgement/markdown/08-ruth/README.md) | [`08-ruth.json`](II-Judgement/json/08-ruth.json) |
| 9 | 1 Samuel | 31 | 772 | 137 | [`II-Judgement/markdown/09-1-samuel/`](II-Judgement/markdown/09-1-samuel/README.md) | [`09-1-samuel.json`](II-Judgement/json/09-1-samuel.json) |
| 10 | 2 Samuel | 24 | 695 | 114 | [`II-Judgement/markdown/10-2-samuel/`](II-Judgement/markdown/10-2-samuel/README.md) | [`10-2-samuel.json`](II-Judgement/json/10-2-samuel.json) |
| 11 | 1 Kings | 22 | 754 | 103 | [`II-Judgement/markdown/11-1-kings/`](II-Judgement/markdown/11-1-kings/README.md) | [`11-1-kings.json`](II-Judgement/json/11-1-kings.json) |
| 12 | 2 Kings | 25 | 718 | 120 | [`II-Judgement/markdown/12-2-kings/`](II-Judgement/markdown/12-2-kings/README.md) | [`12-2-kings.json`](II-Judgement/json/12-2-kings.json) |
| 13 | 1 Chronicles | 29 | 930 | 139 | [`II-Judgement/markdown/13-1-chronicles/`](II-Judgement/markdown/13-1-chronicles/README.md) | [`13-1-chronicles.json`](II-Judgement/json/13-1-chronicles.json) |
| 14 | 2 Chronicles | 36 | 821 | 149 | [`II-Judgement/markdown/14-2-chronicles/`](II-Judgement/markdown/14-2-chronicles/README.md) | [`14-2-chronicles.json`](II-Judgement/json/14-2-chronicles.json) |
| 15 | Ezra | 10 | 280 | 50 | [`II-Judgement/markdown/15-ezra/`](II-Judgement/markdown/15-ezra/README.md) | [`15-ezra.json`](II-Judgement/json/15-ezra.json) |
| 16 | Nehemiah | 13 | 391 | 62 | [`II-Judgement/markdown/16-nehemiah/`](II-Judgement/markdown/16-nehemiah/README.md) | [`16-nehemiah.json`](II-Judgement/json/16-nehemiah.json) |
| 17 | Esther | 10 | 164 | 36 | [`II-Judgement/markdown/17-esther/`](II-Judgement/markdown/17-esther/README.md) | [`17-esther.json`](II-Judgement/json/17-esther.json) |
| 20 | Job | 42 | 1,069 | 190 | [`II-Judgement/markdown/20-job/`](II-Judgement/markdown/20-job/README.md) | [`20-job.json`](II-Judgement/json/20-job.json) |
