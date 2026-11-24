# Saints Modern English (Hebrew) — Fidelity Review against the Saints Hebrew Critical Text (24 November 2026)

- **Status:** `provisional_source_checked_ai_review`. These are AI-made corrections that still need the editor's decisions, an independent human Hebrew review and a read-aloud review. Verse placement should be re-checked against the Saints Critical Text Studio, which was not available to this review.
- **Scope:** the whole Hebrew-based Saints Modern English edition (`Modern-English-OT/`): 39 books, 929 chapters, 22,874 verses at Saints.Bible slots, 293 additional (`unplaced`, `no-site-verse`) Masoretic verses and 4,270 translator notes. Every one of the 23,167 verses and additional verses was read against its Hebrew or Aramaic.
- **Source authority:** the Saints Hebrew Critical Text as held in this repository (`Saints-Hebrew-Critical-Text/`, Masoretic Text with Masoretic numbering). The English translates it as it stands, with the qere. Nothing was harmonized to the Septuagint, the Vulgate, the Dead Sea Scrolls, the New Testament or any published English Bible.
- **Target:** *literal-smooth*, as defined in `Modern-English-OT/STYLE.md`: formal-equivalent English (NASB-1995 method), smoothed only as far as natural modern English requires.
- **Files:**
  - `README.md` (this file): method, results, open decisions.
  - `wording-changes.jsonl`: every wording and note change in canonical order. Each line holds `ref`, `field` (`verse`/`note`), `category`, `pass` (`verse-review`/`edition-wide`), `old`, `new` and `reason`. For additional verses the `ref` is `Book src`.
  - `structural-changes.jsonl`: every verse, note, additional-verse and verse-map change made by the structural repair (`book`, `kind`, `key`, `old`, `new`).
  - `verse-map.json`: for each book, the English verses (Saints.Bible numbers) that translate critical-text verses filed under different Masoretic numbers (`{english key: [critical-text keys]}`). Everything not listed pairs with the critical-text verse of the same number. Psalms (Greek psalm numbering) and Jeremiah (Greek chapter order) are mapped in full.
  - `critical-text-anomalies.md`: points in the critical text and in the edition's data for the Studio.

## Method

1. **Verse alignment.** The English keeps Saints.Bible verse slots, which follow the Greek numbering where it differs from the Masoretic (Psalms, Jeremiah, 1 Kings as 3 Kingdoms, Daniel 3–4, Exodus 35–40, Joshua 8–9, Proverbs 15–16 and 20, and others). The map from English slots to Masoretic verses was rebuilt from each book's `verses.json` (`masoretic_reference`) and checked with a statistical Hebrew–English word-alignment model trained on the edition, which compares each English verse with the Hebrew at its mapped number and at neighbouring numbers. Flagged chapters were then checked verse by verse in two structural passes. The rule applied:
   - keep English at Saints.Bible verse slots;
   - translate every critical-text verse exactly once;
   - critical-text verses with no Saints slot are additional verses (`unplaced`, `no-site-verse`);
   - where an English verse translates Hebrew filed under another number, keep it at its slot and record the pairing in `verse-map.json`.

   After repair every critical-text verse is covered exactly once: **0 uncovered, 0 doubled, 0 English keys without Hebrew**.
2. **Verse-by-verse review.** 52 parallel reviewers each covered about 450 verses (in 100-verse parts), comparing every verse word by word with the Hebrew or Aramaic under a single brief. The brief looked for:
   - **additions** with no Hebrew basis (intensifiers such as "only", "very", "indeed", "continually"; supplied causal "for"/"therefore");
   - **omissions** (כִּי, גַּם, אַךְ, רַק, וְעַתָּה, infinitive-absolute emphasis, וְהִנֵּה);
   - **meaning errors**: stem, aspect, mood, person, number, referent, negation, statement vs question;
   - **harmonization**: English that follows the Septuagint, Vulgate, an emendation, an NT quotation or a familiar English Bible instead of this Hebrew;
   - **doctrinal bias**, including capitals or wording that settle a referent the Hebrew leaves open;
   - **consistency** with the edition's established renderings;
   - **notes** that were doctrinal, used YHWH, described other translations, or were false for this Hebrew.
   Genesis–Joshua and the books with structural repairs (1 Kings, Nehemiah, Proverbs, Ezekiel, Daniel) were reviewed after their repair.
3. **Central validation.** Every proposal had to match the current text exactly. Proposals were rejected automatically if they added an archaism or Yahweh/YHWH/Jehovah, and flagged if they changed the quotation-mark count; flagged quotation changes were checked across the speech. Doctrinal, referent and capitalization changes were read individually. One proposal was rejected: Isaiah 26:3 keeps "complete peace" for שָׁלוֹם שָׁלוֹם.
4. **Edition-wide passes** standardized terms deliberately left to a central pass (see *Renderings standardized*), and cleaned up notes edition-wide.
5. **Final QA.**
   - All 929 chapter files were regenerated from the JSON: **0 mismatches**.
   - The critical-text coverage check passes (above).
   - No banned archaism and no Yahweh/YHWH/Tetragrammaton remains in verses or notes.
   - Edition counts were updated in the root, OT and division READMEs (additional verses 261 → 293; notes 4,260 → 4,270).
   - Chapters whose quotation marks balance only across a chapter break or an additional verse are deliberate: Genesis 31 (Laban's speech continues in additional 31:51), Exodus 21–23 (the rulings run 21:1–23:33), Numbers 28–29 (one speech, 28:2–29:39) and Job 12–14.
   - Joshua 21:36–37 keep the ⟦ ⟧ brackets that the critical text itself prints (absent from the Leningrad and Aleppo codices); the note says so.

## Results

**993 wording and note changes:**
- 788 to verse text (760 distinct verses) and 205 to notes;
- 581 from the verse-by-verse review and 412 from the edition-wide passes.

There were also **88 structural changes** across 9 books: 18 verses, 28 notes, 36 additional verses and 6 map completions, plus the map corrections listed below.

| Category | Changes | What it covers |
| :--- | ---: | :--- |
| consistency | 628 | Same Hebrew, same English (established renderings, formulas, names, headings, refrains) |
| note | 184 | Notes corrected: claims about other translations, doctrinal framing, YHWH/Tetragrammaton, false statements about the Hebrew or the verse numbering |
| addition | 70 | Words with no Hebrew basis removed |
| meaning | 39 | Wrong sense, aspect, mood or clause relation |
| grammar | 24 | Hebrew syntax misrepresented (imperatives, purpose clauses, number) |
| omission | 17 | Hebrew words or particles not represented |
| clarity | 11 | Quotation marks and word order |
| referent | 10 | Wrong subject or object; number that settled a collective/individual referent |
| harmonization | 8 | English that followed the Septuagint or another source instead of this Hebrew |
| doctrinal | 2 | Doctrinal labels in notes ("messianic") |

### By book

| Book | Verse edits | Note edits |
| :--- | ---: | ---: |
| Genesis | 79 | 14 |
| Exodus | 37 | 17 |
| Leviticus | 39 | 10 |
| Numbers | 37 | 10 |
| Deuteronomy | 35 | 9 |
| Joshua | 15 | 3 |
| Judges | 22 | 0 |
| Ruth | 5 | 0 |
| 1 Samuel | 12 | 6 |
| 2 Samuel | 19 | 2 |
| 1 Kings | 33 | 2 |
| 2 Kings | 17 | 3 |
| 1 Chronicles | 16 | 7 |
| 2 Chronicles | 32 | 5 |
| Ezra | 6 | 1 |
| Nehemiah | 12 | 3 |
| Esther | 9 | 3 |
| Job | 13 | 13 |
| Psalms | 118 | 38 |
| Proverbs | 16 | 4 |
| Ecclesiastes | 23 | 9 |
| Song of Songs | 5 | 1 |
| Lamentations | 1 | 0 |
| Isaiah | 47 | 9 |
| Jeremiah | 45 | 1 |
| Ezekiel | 37 | 6 |
| Daniel | 15 | 5 |
| Hosea | 1 | 5 |
| Joel | 0 | 2 |
| Amos | 2 | 0 |
| Obadiah | 0 | 0 |
| Jonah | 2 | 2 |
| Micah | 2 | 1 |
| Nahum | 0 | 1 |
| Habakkuk | 1 | 4 |
| Zephaniah | 1 | 1 |
| Haggai | 0 | 1 |
| Zechariah | 7 | 4 |
| Malachi | 27 | 3 |

## Structural repair (summary)

The full list is in `structural-changes.jsonl`; map entries are in `verse-map.json`.

- **Masoretic verses that had been merged into a neighbouring English verse, split out as additional verses:** Genesis 31:51, 35:21; Exodus 28:24–25, 35:15, 35:17, 37:4, 37:22; Numbers 25:19; Joshua 8:13, 8:30–35 (the Mount Ebal altar had been placed inside 9:2 in Greek order); 1 Kings 5:31, 8:12–13, 11:3, 12:2, 14:10–13, 14:17–18, 22:47–50; Daniel 5:25 (the inscription had been read before Daniel's speech).
- **Stale map entries removed or corrected** that shifted whole passages by a verse or more: Genesis 32 (32 entries), Exodus 20:17–26, Deuteronomy 5:21–33; Exodus 37–38 and 38:27 → 40:31–32; 1 Kings (35 operations, 10 map entries: Greek-slot verses that already carried Masoretic verses, e.g. 2:35 + 9:23, 9:25; 2:46 + 4:20, 5:1, 5:5; 10:22 + 9:15, 9:17–22).
- **Decalogue order.** The English keeps the Saints slot order (Exodus 20:13–15 adultery / theft / murder; Deuteronomy 5:17–18 adultery / murder), which is also the order of the Greek and Latin slots. The map pairs each slot with its Masoretic verse, and the notes now say that this edition's verse order, not the Hebrew, places them so.
- **Map completions found in final QA:** English Numbers 6:23 (+ MT 6:27), 1 Kings 7:6 (+ 7:20), 7:8 (+ 7:22), 7:18 (+ 7:31), Proverbs 31:28 (+ 31:26) and Ezekiel 7:10 (+ 7:5) already translated two Masoretic verses each; the map now says so.
- **Proverbs 15–16, 20; Daniel 3–4:** Masoretic 16:6–9 are in English 15:27–29, 20:20–22 in English 20:9, and Daniel 3:31–33 (the king's letter) in English 4:37; mapped, and notes that said the critical text itself arranged them so were corrected.
- **Notes rewritten** wherever they credited this edition's Greek-based verse order to the Hebrew (e.g. Exodus 20:13, 21:16; Numbers 6:23, 10:34; Proverbs 31:28; Ezekiel 7:10; Malachi 3:24).

## Renderings standardized (edition-wide)

| Hebrew | Rendering | Notes |
| :--- | :--- | :--- |
| חֶסֶד | "loyal love"; plural חֲסָדִים "acts of loyal love" | 239 verses now read "loyal love"; replaces "faithful love", "steadfast love", "loyal kindness", "kindness", "mercy", "constancy". Human hesed is the same word and the same English. Kept: the homonym "disgrace" (Leviticus 20:17; Proverbs 14:34); the verb (2 Samuel 22:26; Psalm 17:26 = MT 18:26); gaining hesed in a stranger's eyes (Esther 2:9, 2:17; Daniel 1:9 — see open items). Micah 6:8 now reads "to love loyal love". |
| זֶרַע (offspring) | "seed" | 161 verse edits; replaces "offspring", "descendants", "lineage"; "royal seed" for זֶרַע הַמְּלוּכָה. The noun stays grammatically singular where the Hebrew is (Genesis 3:15 note no longer says "collective"; Genesis 22:17, 24:60 "his enemies"); plural verbs and suffixes stay plural where the Hebrew has them. Agricultural seed and the sexual idioms of Leviticus 15, 18:20, 19:20 and Numbers 5:13 are unchanged. |
| כֹּה אָמַר יהוה | "This is what the LORD says" | Already almost uniform; Zechariah 7:9 aligned. |
| יהוה צְבָאוֹת | "the LORD of hosts" | Malachi used "the LORD of armies" (24 verses); Micah 4:4 likewise. |
| מַשָּׂא (oracle heading) | "A pronouncement" | Isaiah 19:1, 30:6; Habakkuk 1:1; Zechariah 9:1, 12:1. |
| לַמְנַצֵּחַ | "For the music director" | 11 psalm headings had "For the music leader". |
| הַקֹּהֶלֶת | "the Convener" | Ecclesiastes 7:27 ("the Preacher") and 12:8–10 ("the Assembler") aligned with 1:1, 2, 12. |
| הֶבֶל; רְעוּת רוּחַ (Ecclesiastes) | "vapor"; "chasing wind" | Chapters 4–9 had "futility" and "herding wind". |
| יַם־סוּף | "Sea of Reeds" | Literal; "Red Sea" (21 verses) followed the Septuagint. Notes give the Septuagint's name as a neutral comparison. |
| רֵיחַ נִיחֹחַ | "soothing fragrance" | Replaces "pleasing/soothing aroma" (Genesis 8:21; Exodus 29; Leviticus 17:6; Ezekiel; Daniel 2:46). |
| חַג … (festival names) | "Feast of Booths / Weeks / Unleavened Bread / Harvest / Ingathering" | Replaces "Festival of …". |
| סֵפֶר דִּבְרֵי הַיָּמִים (Kings formula) | "the book of the chronicles of the kings of Israel/Judah" | Replaces "scroll of the chronicles", "Book of the Chronicles", "annals". |
| bare רוּחַ (Ezekiel) | "a spirit" | Ezekiel 2:2; 3:12, 14, 24; 8:3; 11:1, 24; 43:5 (no article, no "of God"), as Isaiah 32:15. "Spirit" stays capitalized for רוּחַ אֱלֹהִים / רוּחַ יהוה and "My Spirit". Genesis 41:38 (Pharaoh) is lowercase. |
| Names | Ochran (Numbers 1:13, 2:27) | One spelling for עָכְרָן. |
| Notes | — | 38 notes in the final pass (184 note changes in all): no "traditionally rendered", "most English Bibles", "some versions", YHWH/Tetragrammaton, "messianic" or NT-fulfilment claims remain. Verse-numbering remarks now say "this edition's verse order" or "another verse division". |

## Open items for the editor

1. **Capitals for disputed figures.** As in the Greek and Latin reviews, the edition's existing capitals were kept and flagged:
   - Pentateuch: Genesis 18:10 ("He said", the visitor); 48:16 ("the Angel", "may He bless"); 49:24 ("the Shepherd, the Stone of Israel"); Exodus 8:8 ("He had imposed"); 23:20–23 (the angel, lowercase); Numbers 11:17, 25–26 (bare הָרוּחַ as "Spirit"); 23:22 ("He is to him" vs 24:8); Deuteronomy 18:15, 18 ("a prophet", lowercase); 32:11; 33:12; 34:6.
   - Joshua 5:14–15 (the commander, lowercase); 1 Chronicles 21:1 "Satan" and Job 1–2 "Satan" for הַשָּׂטָן (Zechariah 3:1 note now says "the Accuser").
   - Psalms: 2 ("anointed", "son", lowercase); 44:7–8 (MT 45:7–8, capitals only there); 109:1 ("my lord"), 109:7; 105:33 ("His Spirit"); 111:4; 131:10, 17 ("Your/My anointed one"); 138:16.
   - Job 19:25 ("Redeemer"); Proverbs 21:12 ("the Righteous One"); 23:11 ("their Redeemer"); Ecclesiastes 12:11 ("one Shepherd").
   - Isaiah: 4:2 (branch), 5:1–2, 7:14 and 8:8, 9:5–6 (throne names capitalized, "his" lowercase), 10:34, 11:1–10, 16:5, 24:16 and 26:7 ("Righteous One", "Upright One"), 28:16, 30:20 ("your Teacher"), 30:31, 33:6, 42:1–4 / 49:1–7 / 50:4–10 / 52:13–53:12 (the servant, lowercase; the 53:2 note's "does not mark the servant as divine" belongs with this decision), 48:16 note ("Servant"), 59:19–20 ("He will come", "a Redeemer"), 61:1.
   - Jeremiah 23:5 ("a righteous Branch"), 33:15 (additional verse, lowercase), 37:9, 37:21; Lamentations 3:28, 4:20; Ezekiel 1:27, 8:2 ("His waist"), 21:32, 34:23–24, 37:24–25.
   - Daniel 7:13–14 ("one like a son of man", lowercase), 7:27, 8:11, 8:25, 9:25–26 ("an anointed one, a prince", lowercase), 3:92.
   - Hosea 3:5, 6:7 ("like Adam"), 11:3, 11:7, 12:5; Micah 2:13, 5:1–5 (ruler, lowercase), 6:9; Zephaniah 2:14; Zechariah 3:8, 6:12 ("Branch"), 6:7–8, 9:9, 9:17, 12:10 ("mourn over Him"); Malachi 2:10, 3:1.

   One rule is needed for the whole edition, and it should match whatever is decided for the Greek- and Latin-based editions.
2. **חֶסֶד won in a stranger's eyes** (Esther 2:9, 2:17; Daniel 1:9) keeps "kindness"/"favor"; Daniel 1:9 still renders רַחֲמִים "mercy" (elsewhere "compassion").
3. **Verse order that follows the Greek slots** (Exodus 20:13–15, 21:16–17; Deuteronomy 5:17–18; Numbers 6:23–27, 10:34–36, 26:15–47; Deuteronomy 23:25–26; Proverbs 31:25–28; Ezekiel 7:3–10; Malachi 3:22–24). The English is complete and the notes now disclose the order, but a Hebrew-based edition could print these in Masoretic order. This is a site-wide versification decision.
4. **Remaining small variation, left to avoid churn:**
   - גֵּר: "resident alien" / "sojourner" / "foreign resident";
   - נָשִׂיא: "leader" / "chieftain"; קָדֵשׁ: "male cult prostitute" / "male shrine prostitute";
   - פָּדָה: "redeem" / "ransom"; מַצֵּבָה: "standing stone" / "sacred pillar"; טָמֵא: "unclean" / "impure";
   - אֲהָהּ: "Ah" / "Alas"; וְהָיָה: "it will come about" / "it will happen"; בַּיּוֹם הַהוּא: "on/in that day";
   - דֶּבֶר: "plague" (some additional Jeremiah verses) / "pestilence";
   - boundary terms in Joshua 16–19 ("outer limits"/"endpoints", "boundary"/"border");
   - "Lebo-hamath" (Ezekiel 48:1) / "the entrance of Hamath" (47:20); "gibbor chayil"; "perpetual / permanent statute"; "Israelites" / "sons of Israel" in Judges 10–11; "city of David" capitalization;
   - numbers with and without "and" (Numbers 4); "ten words" / "Ten Words" (Deuteronomy 4:13, 10:4).
5. **Quotation-mark structure** in Exodus 25:40–30:1 (divine speech partly unquoted) and Deuteronomy 32:28–34. The marks balance; the structure is an editorial choice.
6. **Notes that cite the New Testament** neutrally (Joel 3:1 → Acts 2:17; Amos 9:12 → Acts 15:17; Jeremiah 38:32 → Hebrews 8:9) were kept as factual cross-references; decide whether OT notes should cite the NT at all. Notes that use "fulfil(l)" for an internal cross-reference (Leviticus 9:4; Deuteronomy 31:23; 1 Kings 16:34; Isaiah 12:1) were kept.
7. **Judgement calls a human Hebraist should confirm:** Daniel 9:26 ("until the end of the war", following the accents) and 9:27 ("make a covenant strong"); Ezekiel 41:6 ("thirty-three times", literal); Zephaniah 1:5 ("swear by their king", MT pointing, not "Milcom"); Isaiah 40:6 ("all its loyal love"); Song of Songs 8:3 (statement, as 2:6); Exodus 12:42 ("a night of vigil for the LORD").
