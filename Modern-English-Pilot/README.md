# Saints Modern English Pilot — Hebrew & Biblical Aramaic — Masoretic Text

> **Pilot Status:** `draft: true`  
> **Coverage:** 6 passages, 147 verses, 80 translator notes  
> **Validation:** Passed peer translation review and `validate_modern_english.py --strict` (0 FAIL, 0 WARN)

## Overview

This directory contains the reviewed **Saints Modern English Pilot** translated directly from `Saints-Hebrew-Critical-Text` under the Saints Modern English style policy ([`STYLE.md`](STYLE.md)) and shared term glossary ([`glossary.json`](glossary.json)).

- Follows **Saints.Bible versification keys** (e.g., MT Psalm 23 is keyed as `22:1`–`22:6` to align with the Saints/Greek column).
- Daniel 2:1–4a is translated from Hebrew and Daniel 2:4b–49 from Biblical Aramaic; all 16 *ketiv/qere* cases follow the *qere* (read form).
- Divine names follow the locked style policy (`יְהוָה` → `the LORD`, `אֲדֹנָי יְהוָה` → `the Lord GOD`, `אֱלֹהִים` → `God`).

## Directory Contents

- [`STYLE.md`](STYLE.md) — Locked translation style policy (formal-equivalent Modern English, own-source fidelity, no archaisms, original wording).
- [`glossary.json`](glossary.json) — Standardized proper names and recurring theological/lexical terms.
- `json/` — Structured per-passage JSON (`verses` keyed by Saints `ch:v`, plus `notes`).
- `markdown/` — Human-readable Markdown reading editions with inline verse numbers and translator notes.

## Pilot Passages

| Passage | Saints Keys | Verses | Notes | Reading Edition | Structured JSON |
|---|---|---:|---:|---|---|
| Genesis 1 | `1:1–31` | 31 | 10 | [`01-genesis-1.md`](markdown/01-genesis-1.md) | [`01-genesis-1.json`](json/01-genesis-1.json) |
| Genesis 2 | `2:1–25` | 25 | 14 | [`01-genesis-2.md`](markdown/01-genesis-2.md) | [`01-genesis-2.json`](json/01-genesis-2.json) |
| Genesis 3 | `3:1–24` | 24 | 12 | [`01-genesis-3.md`](markdown/01-genesis-3.md) | [`01-genesis-3.json`](json/01-genesis-3.json) |
| Psalms 22 (MT/English Ps 23) | `22:1–6` | 6 | 6 | [`21-psalms-22.md`](markdown/21-psalms-22.md) | [`21-psalms-22.json`](json/21-psalms-22.json) |
| Isaiah 53 | `53:1–12` | 12 | 11 | [`28-isaiah-53.md`](markdown/28-isaiah-53.md) | [`28-isaiah-53.json`](json/28-isaiah-53.json) |
| Daniel 2 | `2:1–49` | 49 | 27 | [`31-daniel-2.md`](markdown/31-daniel-2.md) | [`31-daniel-2.json`](json/31-daniel-2.json) |
