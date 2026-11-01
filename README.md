# Hebrew–English column of the Saints.Bible Parallel Reader

The Hebrew–English rendering ("Literal-Smooth, Rabbinic Priority") for every verse of the 39 books of the Hebrew Bible on Saints.Bible, captured from the staging Parallel Reader on 1 November 2026, with the Westminster Leningrad Codex Hebrew beside it for reference and an audit of the column's fidelity to the Masoretic Text. Companion to [Saints-Translation](https://github.com/Dotty777/Saints-Translation) (the Greek-based Saints English) and [Latin-translation](https://github.com/Dotty777/Latin-translation) (the Clementine Vulgate column), in the same layout.

- [AUDIT.md](AUDIT.md): the fidelity and accuracy audit (verdict, method, findings, recommendations).
- `audit/`: working data — a per-verse check table, the 186 Hebrew verses with no rendering, the 1,284 readings with editorial tags inside the text, and the 652 Genesis readings whose wording matches the Greek column.
- One folder per book: `README.md` (counts), `<Book>.txt` (Hebrew and English by chapter), `verses.json` (structured text with card ids, classifications, notes and Masoretic numbering).

Verse numbers follow the Saints (Greek) column; where the Masoretic Text numbers a verse differently, `verses.json` records the Masoretic reference. The Hebrew text is not displayed on the site (except in Chronicles); it is included here from the public-domain [embabel-worlds/realm-tanakh](https://github.com/embabel-worlds/realm-tanakh) dataset (Sefaria/WLC) so the rendering can be checked.

## Books

- [Genesis — 50 chapters](genesis/README.md): 1,534 readings; 0 Hebrew verses without a rendering; 43% share the Greek column's wording; 33 editorial tags in the text.
- [Exodus — 40 chapters](exodus/README.md): 1,227 readings; 59 Hebrew verses without a rendering; 14% share the Greek column's wording; 31 editorial tags in the text.
- [Leviticus — 27 chapters](leviticus/README.md): 866 readings; 7 Hebrew verses without a rendering; 10% share the Greek column's wording; 30 editorial tags in the text.
- [Numbers — 36 chapters](numbers/README.md): 1,304 readings; 16 Hebrew verses without a rendering; 12% share the Greek column's wording; 46 editorial tags in the text.
- [Deuteronomy — 34 chapters](deuteronomy/README.md): 962 readings; 3 Hebrew verses without a rendering; 1% share the Greek column's wording; 91 editorial tags in the text.
- [Joshua — 24 chapters](joshua/README.md): 659 readings; 0 Hebrew verses without a rendering; 5% share the Greek column's wording; 0 editorial tags in the text.
- [Judges — 21 chapters](judges/README.md): 618 readings; 0 Hebrew verses without a rendering; 25% share the Greek column's wording; 0 editorial tags in the text.
- [Ruth — 4 chapters](ruth/README.md): 85 readings; 0 Hebrew verses without a rendering; 6% share the Greek column's wording; 0 editorial tags in the text.
- [1 Samuel — 31 chapters](1-samuel/README.md): 773 readings; 0 Hebrew verses without a rendering; 13% share the Greek column's wording; 0 editorial tags in the text.
- [2 Samuel — 24 chapters](2-samuel/README.md): 696 readings; 0 Hebrew verses without a rendering; 35% share the Greek column's wording; 0 editorial tags in the text.
- [1 Kings — 22 chapters](1-kings/README.md): 883 readings; 58 Hebrew verses without a rendering; 17% share the Greek column's wording; 0 editorial tags in the text.
- [2 Kings — 25 chapters](2-kings/README.md): 723 readings; 0 Hebrew verses without a rendering; 20% share the Greek column's wording; 0 editorial tags in the text.
- [1 Chronicles — 29 chapters](1-chronicles/README.md): 930 readings; 0 Hebrew verses without a rendering; 5% share the Greek column's wording; 0 editorial tags in the text.
- [2 Chronicles — 36 chapters](2-chronicles/README.md): 833 readings; 12 Hebrew verses without a rendering; 3% share the Greek column's wording; 821 editorial tags in the text.
- [Ezra — 10 chapters](ezra/README.md): 280 readings; 0 Hebrew verses without a rendering; 9% share the Greek column's wording; 67 editorial tags in the text.
- [Nehemiah — 13 chapters](nehemiah/README.md): 392 readings; 0 Hebrew verses without a rendering; 8% share the Greek column's wording; 0 editorial tags in the text.
- [Esther — 10 chapters](esther/README.md): 247 readings; 17 Hebrew verses without a rendering; 0% share the Greek column's wording; 165 editorial tags in the text.
- [Job — 42 chapters](job/README.md): 1,083 readings; 0 Hebrew verses without a rendering; 1% share the Greek column's wording; 0 editorial tags in the text.
- [Psalms — 150 chapters](psalms/README.md): 2,527 readings; 1 Hebrew verses without a rendering; 4% share the Greek column's wording; 0 editorial tags in the text.
- [Proverbs — 31 chapters](proverbs/README.md): 939 readings; 0 Hebrew verses without a rendering; 1% share the Greek column's wording; 0 editorial tags in the text.
- [Ecclesiastes — 12 chapters](ecclesiastes/README.md): 222 readings; 0 Hebrew verses without a rendering; 30% share the Greek column's wording; 0 editorial tags in the text.
- [Song of Songs — 8 chapters](song-of-songs/README.md): 117 readings; 0 Hebrew verses without a rendering; 18% share the Greek column's wording; 0 editorial tags in the text.
- [Lamentations — 5 chapters](lamentations/README.md): 150 readings; 0 Hebrew verses without a rendering; 7% share the Greek column's wording; 0 editorial tags in the text.
- [Isaiah — 66 chapters](isaiah/README.md): 1,289 readings; 0 Hebrew verses without a rendering; 0% share the Greek column's wording; 0 editorial tags in the text.
- [Jeremiah — 52 chapters](jeremiah/README.md): 1,299 readings; 0 Hebrew verses without a rendering; 2% share the Greek column's wording; 0 editorial tags in the text.
- [Ezekiel — 48 chapters](ezekiel/README.md): 1,267 readings; 0 Hebrew verses without a rendering; 5% share the Greek column's wording; 0 editorial tags in the text.
- [Daniel — 12 chapters](daniel/README.md): 451 readings; 13 Hebrew verses without a rendering; 1% share the Greek column's wording; 0 editorial tags in the text.
- [Hosea — 14 chapters](hosea/README.md): 197 readings; 0 Hebrew verses without a rendering; 2% share the Greek column's wording; 0 editorial tags in the text.
- [Joel — 4 chapters](joel/README.md): 73 readings; 0 Hebrew verses without a rendering; 4% share the Greek column's wording; 0 editorial tags in the text.
- [Amos — 9 chapters](amos/README.md): 146 readings; 0 Hebrew verses without a rendering; 1% share the Greek column's wording; 0 editorial tags in the text.
- [Obadiah — 1 chapters](obadiah/README.md): 21 readings; 0 Hebrew verses without a rendering; 0% share the Greek column's wording; 0 editorial tags in the text.
- [Jonah — 4 chapters](jonah/README.md): 48 readings; 0 Hebrew verses without a rendering; 6% share the Greek column's wording; 0 editorial tags in the text.
- [Micah — 7 chapters](micah/README.md): 105 readings; 0 Hebrew verses without a rendering; 1% share the Greek column's wording; 0 editorial tags in the text.
- [Nahum — 3 chapters](nahum/README.md): 47 readings; 0 Hebrew verses without a rendering; 2% share the Greek column's wording; 0 editorial tags in the text.
- [Habakkuk — 3 chapters](habakkuk/README.md): 56 readings; 0 Hebrew verses without a rendering; 2% share the Greek column's wording; 0 editorial tags in the text.
- [Zephaniah — 3 chapters](zephaniah/README.md): 53 readings; 0 Hebrew verses without a rendering; 2% share the Greek column's wording; 0 editorial tags in the text.
- [Haggai — 2 chapters](haggai/README.md): 38 readings; 0 Hebrew verses without a rendering; 5% share the Greek column's wording; 0 editorial tags in the text.
- [Zechariah — 14 chapters](zechariah/README.md): 211 readings; 0 Hebrew verses without a rendering; 7% share the Greek column's wording; 0 editorial tags in the text.
- [Malachi — 3 chapters](malachi/README.md): 55 readings; 0 Hebrew verses without a rendering; 2% share the Greek column's wording; 0 editorial tags in the text.
