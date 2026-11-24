# Critical-text and data points found during the 24 November 2026 review

For the Saints Critical Text Studio. None of these changed the critical text; the English translates it as it stands.

## Saints Hebrew Critical Text

1. **Ketiv/qere order in the printed text.** In 1 Kings 4:7 and 6:10 (also Nehemiah 11:17) the ketiv in parentheses comes *after* the qere word (e.g. `הָאֶחָ֖ד (אחד)`, `הַיָּצִ֙יעַ֙ (היצוע)`), whereas elsewhere it comes before (`(יצוע) יָצִ֙יעַ֙`, 6:5). Formatting only; the English follows the qere.
2. **Joshua 21:36–37** are printed in ⟦ ⟧ brackets (absent from the Leningrad and Aleppo codices, present in other manuscripts). The English keeps the brackets and the note explains them.
3. **Masoretic verses with no Saints.Bible slot** (Greek-based numbering has no verse for them). They are carried as additional verses: 293 in all, e.g. Exodus 28:23–28, 35:8, 35:15–18; Joshua 6:4, 8:13, 8:26, 8:30–35, 10:15, 10:43, 13:33, 20:4–6; 1 Kings (many, 3 Kingdoms order); Jeremiah (68, Greek chapter order); Ezekiel 1:14, 10:14, 27:31, 32:19, 33:26, 40:30; Proverbs (Greek order in 15–20).
4. **Saints slots with no Hebrew** (Greek-only content: e.g. Daniel 3:31–33, whose Saints slots hold Greek prayer content while Masoretic 3:31–33 is translated in English 4:37; Proverbs 16:7–8). They stay empty in the Hebrew-based edition; the Hebrew for them is mapped elsewhere (`verse-map.json`).

## Edition data (not the critical text)

1. **Duplicate keys in Daniel 4.** Keys 4:4, 4:5 and 4:32 are used both as English verse slots (mapped to other Masoretic verses) and as additional-verse source keys. This predates the review and is valid (the additional item's `src` is a Masoretic key, the verse key a Saints key), but tools that look up "Daniel 4:4" must say which they mean.
2. **`masoretic_reference` in the per-book `verses.json`** does not record that some Saints-slot English verses translate two Masoretic verses (e.g. 1 Kings 7:6 = MT 7:18 + 7:20; Numbers 6:23 = MT 6:23 + 6:27; Proverbs 31:28 = MT 31:26 + 31:28; Ezekiel 7:10 = MT 7:5 + 7:10). `verse-map.json` in this folder is complete.
3. **Notes that credited this edition's Greek-based verse order to the Hebrew** were corrected (Exodus 20:13, 21:16; Numbers 6:23, 10:34; Deuteronomy 5:17; Proverbs 31:28; Ezekiel 7:10; Malachi 3:24; and others listed in `wording-changes.jsonl` / `structural-changes.jsonl`).
