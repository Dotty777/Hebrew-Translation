# Hebrew–English column of the Saints.Bible Parallel Reader

The Hebrew–English rendering ("Literal-Smooth, Rabbinic Priority") for every verse of the 39 books of the Hebrew Bible on Saints.Bible, captured from the staging Parallel Reader on 1 November 2026 (Genesis–Deuteronomy recaptured on 2 November 2026 after corrections), with the Westminster Leningrad Codex Hebrew beside it for reference and an audit of the column's fidelity to the Masoretic Text. Companion to [Saints-Translation](https://github.com/Dotty777/Saints-Translation) (the Greek-based Saints English) and [Latin-translation](https://github.com/Dotty777/Latin-translation) (the Clementine Vulgate column), in the same layout.

- [AUDIT.md](AUDIT.md): the fidelity and accuracy audit (verdict, method, findings, recommendations).
- `audit/`: working data — a per-verse check table, the Hebrew verses with no rendering (historical candidates, rechecked on 7 November), the readings with editorial tags inside the text (1,053, none left in the Pentateuch), and the Genesis readings whose wording matches the Greek column.
- `corrections/`: the data files applied to the staging site, with a change log per date ([2 November 2026](corrections/2026-11-02/README.md)).
- `staging-backups/`: the staging pages as they were before each set of corrections.
- One folder per book: `README.md` (counts and audit results), `<Book>.txt` (Hebrew and English by chapter), `verses.json` (structured text with card ids, classifications, notes and Masoretic numbering).

Verse numbers follow the Saints (Greek) column; where the Masoretic Text numbers a verse differently, `verses.json` records the Masoretic reference. The Hebrew text is not displayed on the site (except in Chronicles); it is included here from the public-domain [embabel-worlds/realm-tanakh](https://github.com/embabel-worlds/realm-tanakh) dataset (Sefaria/WLC) so the rendering can be checked.

[7 November 2026 review](corrections/2026-11-07-hebrew-review/README.md) records the provisional editorial pass of Ruth, Jonah, and Habakkuk and its staging verification.

[9 November 2026 full review](corrections/2026-11-09-full-review/README.md) records a from-scratch reading of all 39 books against the Masoretic Text: 47 proposed English corrections (6 major), 79 readings where the archive pairs the English with the wrong Hebrew, and 232 Masoretic verses whose Hebrew is in no reading. The report records the findings before editorial changes. The per-book coverage statements below describe the original capture and may omit the source gaps documented in the audit.

## Books

- [Genesis — 50 chapters](genesis/README.md): 1,534 readings; English covers 100% of the Masoretic verses (1533 of 1533), each on the row of the Saints verse it is compared with; English is a literal rendering of the Hebrew (41% shares the Greek column's wording); 0% still unclassified on the site (updated 2 November 2026).
- [Exodus — 40 chapters](exodus/README.md): 1,222 readings; English covers 100% of the Masoretic verses (1210 of 1210), each on the row of the Saints verse it is compared with; English is a literal rendering of the Hebrew (13% shares the Greek column's wording); 0% still unclassified on the site (updated 2 November 2026).
- [Leviticus — 27 chapters](leviticus/README.md): 859 readings; English covers 100% of the Masoretic verses (859 of 859), each on the row of the Saints verse it is compared with; English is a literal rendering of the Hebrew (10% shares the Greek column's wording); 0% still unclassified on the site (updated 2 November 2026).
- [Numbers — 36 chapters](numbers/README.md): 1,288 readings; English covers 100% of the Masoretic verses (1289 of 1289), each on the row of the Saints verse it is compared with; English is a literal rendering of the Hebrew (12% shares the Greek column's wording); 0% still unclassified on the site (updated 2 November 2026).
- [Deuteronomy — 34 chapters](deuteronomy/README.md): 959 readings; English covers 100% of the Masoretic verses (956 of 956), each on the row of the Saints verse it is compared with; English is a literal rendering of the Hebrew (1% shares the Greek column's wording); 0% still unclassified on the site (updated 2 November 2026).
- [Joshua — 24 chapters](joshua/README.md): 659 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Judges — 21 chapters](judges/README.md): 618 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew (25% shares the Greek column's wording); 0% still unclassified on the site.
- [Ruth — 4 chapters](ruth/README.md): all 85 readings compared with the Masoretic text, 59 revised and verified on staging on 7 November 2026.
- [1 Samuel — 31 chapters](1-samuel/README.md): 773 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew (13% shares the Greek column's wording); 0% still unclassified on the site.
- [2 Samuel — 24 chapters](2-samuel/README.md): 696 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew (35% shares the Greek column's wording); 0% still unclassified on the site.
- [1 Kings — 22 chapters](1-kings/README.md): All 817 Masoretic references verified on staging, with 61 additional source readings archived and 51 source pairings corrected on 7 November 2026.
- [2 Kings — 25 chapters](2-kings/README.md): 723 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew (20% shares the Greek column's wording); 0% still unclassified on the site.
- [1 Chronicles — 29 chapters](1-chronicles/README.md): 930 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [2 Chronicles — 36 chapters](2-chronicles/README.md): The twelve entries in the earlier gap list are Greek-only rows. See the current audit.
- [Ezra — 10 chapters](ezra/README.md): 280 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Nehemiah — 13 chapters](nehemiah/README.md): 392 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Esther — 10 chapters](esther/README.md): The earlier gap list includes sixteen Greek-only rows and the existing Masoretic 1:1. See the current audit.
- [Job — 42 chapters](job/README.md): 1,083 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Psalms — 150 chapters](psalms/README.md): 2,527 readings; English covers 100.0% of the Masoretic verses (1 Hebrew verses have no rendering); English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Proverbs — 31 chapters](proverbs/README.md): 939 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Ecclesiastes — 12 chapters](ecclesiastes/README.md): 222 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew (30% shares the Greek column's wording); 0% still unclassified on the site.
- [Song of Songs — 8 chapters](song-of-songs/README.md): 117 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew (18% shares the Greek column's wording); 0% still unclassified on the site.
- [Lamentations — 5 chapters](lamentations/README.md): 150 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Isaiah — 66 chapters](isaiah/README.md): 1,289 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Jeremiah — 52 chapters](jeremiah/README.md): 1,299 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Ezekiel — 48 chapters](ezekiel/README.md): 1,267 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Daniel — 12 chapters](daniel/README.md): The ten flagged Masoretic readings verified on staging. Five source pairings corrected and three additional Aramaic readings archived on 7 November 2026.
- [Hosea — 14 chapters](hosea/README.md): 197 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Joel — 4 chapters](joel/README.md): 73 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Amos — 9 chapters](amos/README.md): 146 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Obadiah — 1 chapters](obadiah/README.md): 21 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Jonah — 4 chapters](jonah/README.md): all 48 readings compared with the Masoretic text, 39 revised and verified on staging on 7 November 2026.
- [Micah — 7 chapters](micah/README.md): 105 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Nahum — 3 chapters](nahum/README.md): 47 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Habakkuk — 3 chapters](habakkuk/README.md): all 56 readings compared with the Masoretic text, 51 revised and verified on staging on 7 November 2026.
- [Zephaniah — 3 chapters](zephaniah/README.md): 53 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Haggai — 2 chapters](haggai/README.md): 38 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Zechariah — 14 chapters](zechariah/README.md): 211 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.
- [Malachi — 3 chapters](malachi/README.md): 55 readings; English covers 100% of the Masoretic verses; English is a literal rendering of the Hebrew; 0% still unclassified on the site.


[9 November 2026 editorial revision](corrections/2026-11-09-hebrew-editorial/README.md) records the updated GitHub readings, repaired source pairings, and remaining archive coverage work.

[9 November 2026 Masoretic coverage and English revisions](corrections/2026-11-09-masoretic-coverage/README.md) adds 185 missing archive readings and refines 10 readings in Genesis, Daniel, and Ezekiel.
