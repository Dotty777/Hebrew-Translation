# Full Hebrew–English review of the Old Testament · 9 November 2026

Every Hebrew–English reading in this repository was read from scratch against the Masoretic Text paired with it: 23,118 distinct readings across the 39 books (23,244 reader rows with both Hebrew and English, including the 64 additional source readings of 1 Kings and Daniel). The review worked from the GitHub record only. **Nothing was changed on the staging site or in the book folders;** everything here is a proposal or a note for decision.

## Result

The Hebrew column is in very good shape. Only 47 readings (0.2%) have a proposed English correction that survived a second reading, 6 of them major, and 22 of the 39 books drew none. Reviewers reported again and again that the English follows the Masoretic Text where the Septuagint differs. The larger findings concern the archive, not the translation: Hebrew paired with the wrong verse, and Masoretic verses missing from the record.

| Outcome | Count | File |
| --- | ---: | --- |
| Proposed English corrections, confirmed on second reading | 47 (6 major, 41 minor) | [proposed-english-corrections.json](proposed-english-corrections.json) |
| First-reading proposals withdrawn on second reading | 9 | [withdrawn-on-second-reading.json](withdrawn-on-second-reading.json) |
| Hebrew pairing findings | 79 | [hebrew-pairing-findings.json](hebrew-pairing-findings.json) |
| Masoretic verses whose Hebrew is in no reading | 232 | [masoretic-verses-not-in-record.json](masoretic-verses-not-in-record.json) |
| Planted errors caught in the sensitivity test | 21 of 23 | [calibration-test.json](calibration-test.json) |

Per-book pages are in [books/](books/); counts per book are in [coverage.csv](coverage.csv) and the table at the end.

## The 6 major corrections

- **1 Chronicles 2:18.** "Azubah-ishah" fuses *ishah* (wife) into an invented name and makes Azubah Caleb's child. The Hebrew is "by Azubah his wife".
- **Deuteronomy 32:43.** "Rejoice, nations, with His people" is the Septuagint and KJV reading. The Masoretic Text has no "with"; *ammo* is the object ("acclaim His people", as Onkelos and Rashi take it).
- **Judges 5:13.** "YHWH's people went down" follows the Septuagint's division of the line. The Masoretic accents end the first half at "people" and make YHWH the subject of the second.
- **Exodus 29:28.** The clause "and it shall be a contribution from the sons of Israel" is missing.
- **Psalms 58:13 (Masoretic 59:13).** "The poor are trapped" names a subject the Hebrew does not have. The second reader could not rule out that this is a gloss from Rashi; check before changing.
- **Isaiah 48:7.** "I let you hear before their day" adds a clause with no Hebrew verb behind it. Same caution: check Rashi and Radak first.

## The 41 minor corrections

Most are a small word left out or added: *gam* (also) twice in Genesis 24:46, "from here" in Exodus 11:1, "from there" in Deuteronomy 5:15, "all" in Deuteronomy 6:11, "about" in Genesis 38:24, an added "completely" in Genesis 41:21, an added "another" in 1 Kings 11:23. Eleven follow another text against the Masoretic pointing, for example "all the Egyptians" (Genesis 41:56), "his brothers" for the singular (Ezra 8:17), "the thirsty" (Job 5:5), "you run with him" (Psalms 49:18) and "clouds" for *avotim* (Ezekiel 31:3, 31:10, 31:14). Genesis has the most (11), which fits the earlier audit's finding that Genesis carried wording from the Greek column; "plain" for *sadeh* survives at Genesis 27:5 and 36:35.

The second reading withdrew nine proposals, among them three that asked for "the land of Egypt" where the English has "Egypt". The same shortening occurs elsewhere and was left alone as idiom.

## Hebrew pairing in the archive (79)

The site does not display the Hebrew. It was paired with the English in this repository for checking, and in 79 readings the pairing is wrong or misleading. In most of them the English is a sound rendering of the right verse and the Hebrew beside it is a neighbouring verse.

- **Jeremiah (29).** In the chapters that follow the Septuagint's order of the oracles against the nations: reader rows 25:14–20 carry the English of the Elam oracle (Masoretic 49:34–39) beside chapter 25 Hebrew; rows 30:1–7, 30:17–21 and 30:29–33 carry English of Masoretic 49 beside other verses of that chapter; rows 51:31–35 carry the English of Masoretic 45:1–5 beside the Hebrew of chapter 44.
- **Proverbs (11).** Greek-order rows: the English of Masoretic 16:6–9 sits at rows 15:27a–29b and of 20:20–22 at 20:9a–c, beside the Hebrew of the neighbouring verse.
- **Psalms (8), Job (6), Ezekiel (4), Isaiah (2), Daniel 11:18, 2 Samuel 5:18.** Single readings where a later verse's Hebrew was duplicated in place of the right one (for example Psalms 115:2, 115:3, 115:6 and 115:7, whose English renders Masoretic 116:11, 12, 15 and 16; Job 6:18, 11:7, 29:5, 30:24, 40:1 and 40:11; Isaiah 2:9 and 3:22).
- **Joshua (6).** Rows 9:2a–f carry the English of Masoretic 8:30–35 beside the Hebrew of 9:2 repeated.
- **1 Kings (6), Daniel (3), Nehemiah 7:68.** The English is only a "no Masoretic counterpart" note, yet real Hebrew that is rendered elsewhere sits beside it. Daniel 5:26 carries English through 5:28 beside the Aramaic of 5:26 alone.

An independent mechanical comparison (site English against the JPS 1917 of each verse) reached the same conclusion for 26 of the 79.

## Masoretic verses missing from the record (232)

A comparison with the reference Westminster Leningrad text found 232 Masoretic verses whose Hebrew appears in no reading: Jeremiah 77, 1 Samuel 39, Proverbs 24, Daniel 17, Nehemiah 14, Joshua 13, 1 Chronicles 13, Ezekiel 9, Psalms 8, Job 6, Lamentations 4, Isaiah 4, Esther 3, 2 Samuel 1.

- For 47 of them the English is in the record beside other Hebrew (the pairing faults above).
- For the other 185 no matching English was found. These are mostly verses the Greek lacks, so the reader has no row for them: 1 Samuel 17:12–31 and 17:55–18:5, Jeremiah 33:14–26 and 39:4–13, Proverbs 20:14–19, verses within Nehemiah 11:16–35 and 12:4–6, 1 Chronicles 1:11–16 and 1:18–23, Joshua 20:4–6, Lamentations 3:22–24. The word-overlap test is rough and will have missed some renderings.
- **This contradicts the book READMEs** that say the English "covers 100% of the Masoretic verses" for Joshua, 1 Samuel, 1 Chronicles, Nehemiah, Jeremiah and others.
- For 1 Kings and Daniel the 7 November check found such verses on staging under "Additional source readings" and added them to this archive. The same may hold for the other books. **Whether staging has these 185 was not checked here.**

## Method

1. **Inputs.** Every reading with both Hebrew and English was taken from the book folders' `verses.json` (captured 1–7 November 2026), plus the 64 readings in the 1 Kings and Daniel `source-only-readings.json`, and cut into 357 batches.
2. **First reading.** Forty AI reviewers (Claude) read their batches unit by unit, Hebrew against English, under [review-brief.md](review-brief.md). The brief respects the column's stated approach ("Literal-Smooth, Rabbinic Priority"): a reading the Hebrew can bear on the authority of Targum, Rashi, Ibn Ezra or Radak is not a finding, nor is either side of a ketiv/qere. Editorial tags such as "[BHS 1:1]" were ignored as an already recorded issue. All batches came back with the full unit count.
3. **Sensitivity test.** Two passages were copied with 23 errors planted in the English (changed numbers, names and negations, dropped words, Septuagint readings) and given to two further reviewers under the same brief. They caught 21. The two they passed, "king" for *nagid* and "chief officials" for *kohanim* in 2 Samuel 8:18, they judged to be traditional readings.
4. **Second reading.** The 54 proposed English corrections from the main reading went to two further reviewers with the JPS 1917 rendering for reference, under [second-reading-brief.md](second-reading-brief.md): 45 confirmed, 9 withdrawn. The two proposals from the additional source readings were checked by the coordinator instead.
5. **Mechanical checks.** The recorded Hebrew was matched to the reference text ([embabel-worlds/realm-tanakh](https://github.com/embabel-worlds/realm-tanakh), the source this archive used) to find Masoretic verses in no reading, and the site English was compared with JPS 1917 to test the pairing findings.

## Limits

- The reviewers are AI models. No human Hebraist has read this, and the "specialist review pending" status stands.
- What counts as a traditional reading was judged from the reviewers' own knowledge of the commentators, with nothing looked up. Some accepted readings may not be traditional, and two of the six majors may turn out to be.
- The second readers saw the first reader's proposal and reason, so the second reading was independent but not blind.
- One reading pass finds most plain departures, not all. The sensitivity test suggests about nine in ten errors of the planted kinds are caught; subtler ones will be caught less often.
- The review read the GitHub capture, not live staging. Readings changed on staging after capture were not seen.
- Where the archive pairs the English with the wrong Hebrew, the English could be judged only by recognising which verse it renders.

## By book

| Book | Readings read | Corrections (major) | Pairing | Masoretic verses not in record (no English found) |
| --- | ---: | ---: | ---: | ---: |
| [Genesis](books/genesis.md) | 1,534 | 11 (0) | 0 | 0 (0) |
| [Exodus](books/exodus.md) | 1,217 | 3 (1) | 0 | 0 (0) |
| [Leviticus](books/leviticus.md) | 859 | 2 (0) | 0 | 0 (0) |
| [Numbers](books/numbers.md) | 1,288 | 1 (0) | 0 | 0 (0) |
| [Deuteronomy](books/deuteronomy.md) | 959 | 4 (1) | 0 | 0 (0) |
| [Joshua](books/joshua.md) | 656 | 0 (0) | 6 | 13 (5) |
| [Judges](books/judges.md) | 618 | 1 (1) | 0 | 0 (0) |
| [Ruth](books/ruth.md) | 85 | 0 (0) | 0 | 0 (0) |
| [1 Samuel](books/1-samuel.md) | 773 | 0 (0) | 0 | 39 (29) |
| [2 Samuel](books/2-samuel.md) | 696 | 0 (0) | 1 | 1 (0) |
| [1 Kings](books/1-kings.md) | 856 | 2 (0) | 6 | 0 (0) |
| [2 Kings](books/2-kings.md) | 720 | 0 (0) | 0 | 0 (0) |
| [1 Chronicles](books/1-chronicles.md) | 930 | 3 (1) | 0 | 13 (11) |
| [2 Chronicles](books/2-chronicles.md) | 821 | 1 (0) | 0 | 0 (0) |
| [Ezra](books/ezra.md) | 280 | 1 (0) | 0 | 0 (0) |
| [Nehemiah](books/nehemiah.md) | 392 | 1 (0) | 1 | 14 (14) |
| [Esther](books/esther.md) | 170 | 0 (0) | 0 | 3 (3) |
| [Job](books/job.md) | 1,074 | 1 (0) | 6 | 6 (5) |
| [Psalms](books/psalms.md) | 2,526 | 6 (1) | 8 | 8 (8) |
| [Proverbs](books/proverbs.md) | 927 | 0 (0) | 11 | 24 (22) |
| [Ecclesiastes](books/ecclesiastes.md) | 222 | 0 (0) | 0 | 0 (0) |
| [Song of Songs](books/song-of-songs.md) | 117 | 0 (0) | 0 | 0 (0) |
| [Lamentations](books/lamentations.md) | 150 | 0 (0) | 0 | 4 (4) |
| [Isaiah](books/isaiah.md) | 1,289 | 5 (1) | 2 | 4 (4) |
| [Jeremiah](books/jeremiah.md) | 1,298 | 0 (0) | 29 | 77 (58) |
| [Ezekiel](books/ezekiel.md) | 1,267 | 3 (0) | 4 | 9 (9) |
| [Daniel](books/daniel.md) | 344 | 1 (0) | 5 | 17 (13) |
| [Hosea](books/hosea.md) | 197 | 0 (0) | 0 | 0 (0) |
| [Joel](books/joel.md) | 73 | 0 (0) | 0 | 0 (0) |
| [Amos](books/amos.md) | 146 | 0 (0) | 0 | 0 (0) |
| [Obadiah](books/obadiah.md) | 21 | 0 (0) | 0 | 0 (0) |
| [Jonah](books/jonah.md) | 48 | 0 (0) | 0 | 0 (0) |
| [Micah](books/micah.md) | 105 | 0 (0) | 0 | 0 (0) |
| [Nahum](books/nahum.md) | 47 | 1 (0) | 0 | 0 (0) |
| [Habakkuk](books/habakkuk.md) | 56 | 0 (0) | 0 | 0 (0) |
| [Zephaniah](books/zephaniah.md) | 53 | 0 (0) | 0 | 0 (0) |
| [Haggai](books/haggai.md) | 38 | 0 (0) | 0 | 0 (0) |
| [Zechariah](books/zechariah.md) | 211 | 0 (0) | 0 | 0 (0) |
| [Malachi](books/malachi.md) | 55 | 0 (0) | 0 | 0 (0) |
| **Total** | **23,118** | **47 (6)** | **79** | **232 (185)** |

The last column counts Masoretic verses whose Hebrew is in no reading; the figure in brackets is how many of those had no matching English found.
