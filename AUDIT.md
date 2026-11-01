# Hebrew–English column audit — Saints.Bible

1 November 2026. Audit of the Hebrew–English column ("Literal-Smooth, Rabbinic Priority") of the Saints.Bible Parallel Reader (staging) for fidelity to the Masoretic Text. A living copy is kept as a Claude doc; this file is the record for the repository.

## Summary

The Hebrew–English column is a careful, literal rendering of the Masoretic Text. In a close reading of 92 randomly chosen verses against the Hebrew, none mistranslated it, and the column keeps the Tetragrammaton as "YHWH" consistently (a mismatch in fewer than 0.5% of 23,126 readings, nearly all alignment artefacts). The site shows no Hebrew text beside the English, so the audit compared the English with the Westminster Leningrad Codex text and, as an independent rendering, the JPS 1917 translation.

Four problems, the first of which does affect fidelity:

- **Genesis carries Septuagint readings into the Hebrew column.** In Genesis, 652 of 1,534 readings (43%) repeat the Greek column's wording almost word for word, and in a 60-verse sample of those, 5 keep a Greek reading the Hebrew does not have: "plain" for *sadeh* "field" (27:3, 29:2, 41:48), "their hearts were astonished" for "their heart went out" (42:28), "the two slave women" where the Hebrew has no number (33:2). Roughly 40–60 Genesis verses need a Hebrew-first pass. Elsewhere the shared wording is rare (2–18% by section) and the samples showed no carried-over readings.
- **Exodus 35–40 and 1 Kings 7 follow the Septuagint's order, not the Hebrew's.** The Hebrew-column text at those verse numbers is Hebrew material from a different Masoretic verse (46 rows in Exodus 36–39; 1 Kings 7:1 shows 7:13, 7:30 shows 7:44), and 59 Exodus verses and 58 1 Kings verses that exist in Hebrew have no rendering at all. 186 such gaps in total.
- **1,284 readings carry editorial tags inside the verse text** ("[BHS 18:6]" on every verse of 2 Chronicles, "[MT 32:15]", "(Chabad 5:23)", "[Aramaic]", a stray "BHS/RH 5:20" at the end of Leviticus 6:1). These are useful notes in the wrong place.
- **3,755 readings are numbered by the Greek column, not the Hebrew** (all of Psalms 10–147, Jeremiah 26–52, Joel 3–4, Malachi 3), with the Masoretic number given only sometimes.

The column is not borrowed text: only 441 readings (1.9%) match JPS 1917, and those are genealogies and lists where any literal rendering agrees.

## What was checked and how

Every Hebrew–English reading in the staging Parallel Reader: 23,406 readings in the 39 books of the Hebrew Bible. 23,126 have text; 280 are blank. Unlike the Latin cards, the Hebrew comparison cards do not display the Hebrew source (only 1–2 Chronicles show pointed Hebrew), so the source text had to come from outside the site.

**Reference texts.** The pointed Hebrew of the Westminster Leningrad Codex and the JPS 1917 English, verse-aligned with the King James numbering, from the public-domain [embabel-worlds/realm-tanakh](https://github.com/embabel-worlds/realm-tanakh) dataset (Sefaria text). JPS 1917 is a literal rendering of the same Hebrew and serves as an independent comparison, not as a standard.

**Alignment.** The site numbers the Hebrew column by the Greek column (Psalms, Jeremiah, Joel, Malachi, parts of Exodus, Numbers, 1 Kings, Daniel), so each reading was matched to its Masoretic verse by content, using the site's own "[MT x:y]" tags where present. 3,755 readings carry a different number from the Masoretic one.

**Automated checks on every reading**

| Check | What it catches |
| --- | --- |
| English against JPS 1917 (content overlap) | Readings whose content differs sharply from an independent literal rendering; misplaced verses |
| English against the Saints (Greek) column | Readings that repeat the Greek column's wording, where Septuagint readings might survive |
| Tetragrammaton count in Hebrew against "YHWH" count in English | Dropped or added divine names |
| Hebrew negations (lo, ein, bal) and number words against the English | Reversed sense, wrong figures |
| English length against Hebrew word count | Omissions, additions, text from the wrong verse |
| Blank readings against the Masoretic verse list | Hebrew verses with no rendering |

**Manual reading.** The Hebrew was read against the English for 92 randomly chosen readings (23 each from Law, History, Wisdom and Prophets), 60 randomly chosen Genesis readings whose wording matches the Greek column, and 100 readings across all books flagged as sharing the Greek column's wording while differing from JPS. A second pass on 1 November 2026 read, for each of the 39 books, the reading with the lowest content overlap with JPS 1917 and one further reading chosen at random (78 readings): every reading with a Hebrew counterpart was literal and accurate; the low-overlap cases were placeholders ("No MT counterpart") or the versification shifts described under finding 3, not translation errors.

**Limits.** The automated checks compare words, not meaning; the manual samples are where meaning was judged. A 92-verse random sample detects a problem affecting more than about 3% of readings but not a rarer one, so the Genesis finding came from the targeted sample, not the random one. Ketiv/qere choices, the site's textual notes and the Aramaic sections of Daniel and Ezra beyond the sample were not assessed separately. Per-verse results are in `audit/per-verse-checks.csv`.

## Findings

**1. The renderings are literal and accurate.** In the 92-verse random sample, and in the later 78-verse per-book sample, every reading followed the Hebrew clause by clause, including hard cases: Deuteronomy 28:30 renders the ketiv *yishgalennah* ("violate her") rather than the softer qere; Psalm 103:5 keeps "satisfies your adornment with good" (*edyekh*); Job 12:16 "the one who errs and the one who leads astray belong to Him"; Isaiah 28:7 keeps all four verbs of staggering and wandering. The Tetragrammaton is rendered "YHWH" throughout, *Adonai* as "the Lord", *Elohim* as "God"; the counts match the Hebrew in 99.6% of readings and the rest are alignment artefacts or "Yah" in Psalms.

**2. Genesis keeps Septuagint readings where its Hebrew column was built from the Greek column.**

| Verse | Hebrew | Site Hebrew–English | What the Hebrew says |
| --- | --- | --- | --- |
| Genesis 27:3 | וצא השדה | go out into the plain | go out to the field (Greek *pedion*) |
| Genesis 29:2 | באר בשדה | a well was in the plain | a well in the field |
| Genesis 41:48 | אכל שדה העיר | the food from the plains surrounding each city | the food of the field around each city |
| Genesis 33:2 | את השפחות | the two slave women | the slave women (Greek adds "two") |
| Genesis 42:28 | ויצא לבם | their hearts were astonished | their heart went out (failed them); Greek *exestē* |
| Genesis 41:37 | וייטב הדבר | the words were well-pleasing | the thing was good; Greek *ta rhēmata* |
| Genesis 41:20 | הרקות והרעות | the ugly, thin cows ate up the first seven good, fat cows | no "good" in the Hebrew; Greek *kalas* |

In Genesis 652 readings (43%) share the Greek column's wording at 90% similarity or more (list in `audit/genesis-shared-with-greek.json`); 5 of 60 sampled carried a Greek reading, so 40–60 verses are likely affected, concentrated in chapters 12–50. In the other 38 books shared wording is 2–18% by section and the 100 flagged readings examined showed no carried-over Greek readings.

**3. Three sections follow the Septuagint's arrangement.** Exodus 35–40 (176 rows): the Hebrew column is laid out in the Greek order, so 46 rows show Hebrew text belonging to another Masoretic verse (36:19 shows 39:12's "ligure, agate and amethyst"; 36:34 shows 39:27's linen tunics), and 59 Masoretic verses, including 28:23–28 and 32:9, have no rendering. 1 Kings 7 and 9–14: 7:1 shows the Hebrew of 7:13, 7:30 of 7:44; 58 verses have no rendering (3:1, 4:20, 5:5–6, 6:11–14, 8:12–13, 9:15–25, 14:1–20, 22:47–50), while 69 rows correctly say "no Hebrew counterpart" for Greek-only material. Proverbs: Masoretic 16:8 appears at the Greek row 15:29a while 16:7–8 say "no corresponding text". Smaller gaps: Numbers 17:14–28 (16), Esther (17), 2 Chronicles 35–36 (12), Leviticus (7), Deuteronomy (3), Psalms (1). Daniel's 94 blank rows are Susanna and Greek additions and are correct. The 186 gaps are listed in `audit/hebrew-verses-without-rendering.json`.

**4. Editorial tags sit inside the Scripture text.** 1,284 readings begin or end with a reference note: every verse of 2 Chronicles ("[BHS 18:6]", 821), Esther (165), Deuteronomy ("(Chabad 5:23)", 91), Ezra and Daniel ("[Aramaic]", 67), and single cases such as Leviticus 6:1 "YHWH spoke to Moses, saying: BHS/RH 5:20". The Parallel Reader prints them as part of the verse, and the highlighting and word-note scripts count them as words. List in `audit/editorial-tags-in-text.json`.

**5. Numbering follows the Greek column.** 3,755 readings carry a verse number that is not the Masoretic one: Psalms 10–147 (Greek numbering, one behind the Hebrew), Jeremiah 26–52 (Greek chapter order: site 25:16 holds the Hebrew of 49:36), Joel 3–4, Malachi 3:19–24, Numbers 17 and 30, Deuteronomy 5 and 13, 1 Kings 4–5, Genesis 32. The Masoretic number is given in the text for some ("[MT 32:15]") but not most.

**6. Minor.** Genesis 43:27 "How are you?" for *vayyishal lahem leshalom* (asked after their welfare) and Genesis 41:36 "utterly destroyed" for *lo tikkaret* (not be cut off) are paraphrases toward the Greek; the English never says which of ketiv or qere it followed; 441 readings (1.9%) coincide with JPS 1917, all in genealogies, place lists and formulae.

## Results by section

| Section | Readings | Hebrew verses with no rendering | Wording shared with the Greek column | Matches JPS 1917 | Editorial tags in text | Verse number differs from Masoretic |
| --- | --- | --- | --- | --- | --- | --- |
| Law (Genesis–Deuteronomy) | 5,893 | 85 | 18% | 2.4% | 231 | 295 |
| History (Joshua–Esther) | 7,119 | 87 | 13% | 2.6% | 1,053 | 261 |
| Wisdom (Job–Song of Songs, Lamentations) | 5,038 | 1 | 4% | 2.4% | 0 | 2,459 |
| Prophets (Isaiah–Malachi, Daniel) | 5,356 | 13 | 2% | 0.7% | 0 | 740 |

Shared wording is only a risk where it hides a Septuagint reading; in the samples that happened in Genesis and nowhere else. The Wisdom numbering figure is Psalms' Greek numbering.

## Recommendations

1. **Re-read Genesis 12–50 against the Hebrew**, starting with the 652 readings that share the Greek column's wording; correct *sadeh* "field", drop added numbers and adjectives, and restore the Hebrew idiom where the Greek paraphrase was kept.
2. **Re-lay Exodus 35–40 and 1 Kings 7 in Masoretic order** and supply the 186 missing Hebrew verses. Where the Greek column has no row for a Hebrew verse, add a row rather than dropping the verse.
3. **Move the editorial tags out of the verse text** into the card's note field: the "[BHS x:y]" and "(Chabad x:y)" references and "[Aramaic]" markers (1,284 readings).
4. **Show the Masoretic verse number** on every reading whose number follows the Greek column (3,755), in the same place for all books instead of an occasional "[MT x:y]".
5. **Show the Hebrew text on the comparison cards**, as 1–2 Chronicles already do, so readers and future reviews can check the rendering without leaving the site.
6. **Keep the column as the Hebrew comparison text**, labelled as a literal rendering of the Leningrad Codex; after the Genesis pass it can be presented with confidence.
