# Hebrew–English column of the Saints.Bible Parallel Reader

The Hebrew–English rendering ("Literal-Smooth, Rabbinic Priority") for every verse of the 39 books of the Hebrew Bible on Saints.Bible, captured from the staging Parallel Reader on 1 November 2026, with the Westminster Leningrad Codex Hebrew beside it for reference and an audit of the column's fidelity to the Masoretic Text. Companion to [Saints-Translation](https://github.com/Dotty777/Saints-Translation) (the Greek-based Saints English) and [Latin-translation](https://github.com/Dotty777/Latin-translation) (the Clementine Vulgate column), in the same layout.

- [AUDIT.md](AUDIT.md): the fidelity and accuracy audit (verdict, method, findings, recommendations).
- `audit/`: working data — a per-verse check table, the 186 Hebrew verses with no rendering, the 1,284 readings with editorial tags inside the text, and the 652 Genesis readings whose wording matches the Greek column.
- One folder per book: `README.md` (counts and audit results), `<Book>.txt` (Hebrew and English by chapter), `verses.json` (structured text with card ids, classifications, notes and Masoretic numbering).

Verse numbers follow the Saints (Greek) column; where the Masoretic Text numbers a verse differently, `verses.json` records the Masoretic reference. The Hebrew text is not displayed on the site (except in Chronicles); it is included here from the public-domain [embabel-worlds/realm-tanakh](https://github.com/embabel-worlds/realm-tanakh) dataset (Sefaria/WLC) so the rendering can be checked.

## Books

- [Genesis — 50 chapters](genesis/README.md): 1,534 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew (43% shares the Greek column's wording); 0% still unclassified on the site.
- [Exodus — 40 chapters](exodus/README.md): 1,227 readings; English covers 95.1% of the Masoretic verses (59 Hebrew verses have no rendering); English is a literal rendering of the Hebrew (14% shares the Greek column's wording); 5% still unclassified on the site.
- [Leviticus — 27 chapters](leviticus/README.md): 866 readings; English covers 99.2% of the Masoretic verses (7 Hebrew verses have no rendering); English is a literal rendering of the Hebrew (10% shares the Greek column's wording); 43% still unclassified on the site.
- [Numbers — 36 chapters](numbers/README.md): 1,304 readings; English covers 98.8% of the Masoretic verses (16 Hebrew verses have no rendering); English is a literal rendering of the Hebrew (12% shares the Greek column's wording); 100% still unclassified on the site.
- [Deuteronomy — 34 chapters](deuteronomy/README.md): 962 readings; English covers 99.7% of the Masoretic verses (3 Hebrew verses have no rendering); English is a literal rendering of the Hebrew; 100% still unclassified on the site.
- [Joshua — 24 chapters](joshua/README.md): 659 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Judges — 21 chapters](judges/README.md): 618 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew (25% shares the Greek column's wording); 0% still unclassified on the site.
- [Ruth — 4 chapters](ruth/README.md): 85 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [1 Samuel — 31 chapters](1-samuel/README.md): 773 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew (13% shares the Greek column's wording); 0% still unclassified on the site.
- [2 Samuel — 24 chapters](2-samuel/README.md): 696 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew (35% shares the Greek column's wording); 0% still unclassified on the site.
- [1 Kings — 22 chapters](1-kings/README.md): 883 readings; English covers 92.9% of the Masoretic verses (58 Hebrew verses have no rendering); English is a literal rendering of the Hebrew (17% shares the Greek column's wording); 7% still unclassified on the site.
- [2 Kings — 25 chapters](2-kings/README.md): 723 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew (20% shares the Greek column's wording); 0% still unclassified on the site.
- [1 Chronicles — 29 chapters](1-chronicles/README.md): 930 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [2 Chronicles — 36 chapters](2-chronicles/README.md): 833 readings; English covers 98.5% of the Masoretic verses (12 Hebrew verses have no rendering); English is a literal rendering of the Hebrew; 1% still unclassified on the site.
- [Ezra — 10 chapters](ezra/README.md): 280 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Nehemiah — 13 chapters](nehemiah/README.md): 392 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Esther — 10 chapters](esther/README.md): 247 readings; English covers 89.8% of the Masoretic verses (17 Hebrew verses have no rendering); English is a literal rendering of the Hebrew; 7% still unclassified on the site.
- [Job — 42 chapters](job/README.md): 1,083 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Psalms — 150 chapters](psalms/README.md): 2,527 readings; English covers 100.0% of the Masoretic verses (1 Hebrew verses have no rendering); English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Proverbs — 31 chapters](proverbs/README.md): 939 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Ecclesiastes — 12 chapters](ecclesiastes/README.md): 222 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew (30% shares the Greek column's wording); 0% still unclassified on the site.
- [Song of Songs — 8 chapters](song-of-songs/README.md): 117 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew (18% shares the Greek column's wording); 0% still unclassified on the site.
- [Lamentations — 5 chapters](lamentations/README.md): 150 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Isaiah — 66 chapters](isaiah/README.md): 1,289 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Jeremiah — 52 chapters](jeremiah/README.md): 1,299 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Ezekiel — 48 chapters](ezekiel/README.md): 1,267 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Daniel — 12 chapters](daniel/README.md): 451 readings; English covers 96.4% of the Masoretic verses (13 Hebrew verses have no rendering); English is a literal rendering of the Hebrew; 24% still unclassified on the site.
- [Hosea — 14 chapters](hosea/README.md): 197 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Joel — 4 chapters](joel/README.md): 73 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Amos — 9 chapters](amos/README.md): 146 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Obadiah — 1 chapters](obadiah/README.md): 21 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Jonah — 4 chapters](jonah/README.md): 48 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Micah — 7 chapters](micah/README.md): 105 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Nahum — 3 chapters](nahum/README.md): 47 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Habakkuk — 3 chapters](habakkuk/README.md): 56 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Zephaniah — 3 chapters](zephaniah/README.md): 53 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Haggai — 2 chapters](haggai/README.md): 38 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Zechariah — 14 chapters](zechariah/README.md): 211 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Malachi — 3 chapters](malachi/README.md): 55 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
