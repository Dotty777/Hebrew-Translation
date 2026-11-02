# 2 November 2026: KJV classification of the Wisdom Division

Psalms, Proverbs, Ecclesiastes, Song of Songs, Lamentations, Wisdom of Solomon and Sirach. All changes were made on the **staging** site only; production has not been touched. The nine KJV comparison pages as they were before are in [staging-backups/2026-11-02-wisdom-kjv](../../staging-backups/2026-11-02-wisdom-kjv/). The KJV text itself was not changed.

| File | What it is |
| --- | --- |
| `kjv-<book>.json.gz` (9 files) | The new content of each KJV comparison page, applied only if the page still had the md5 it had before ([manifest.json](manifest.json)). |
| [kjv-classifications.json](kjv-classifications.json) | The 5,650 new classifications (KJV ↔ Greek-English): category, layer-1 note, layer-5 note. |
| [blind-sample-check.json](blind-sample-check.json) | A separate reader's blind classification of 180 random cards, beside the review's category. |
| [review-brief.md](review-brief.md) | The rules the review followed. |

## Result by book

| Book | Newly classified | Classification of every card now |
| --- | --- | --- |
| Psalms | 2,504 | Same: 721 · Similar: 840 · Different: 676 · Divergent: 184 · Disparate: 110 |
| Proverbs | 883 | Same: 94 · Similar: 258 · Different: 358 · Divergent: 142 · Disparate: 106 |
| Ecclesiastes | 212 | Same: 79 · Similar: 72 · Different: 54 · Divergent: 10 · Disparate: 7 |
| Song of Songs | 108 | Same: 17 · Similar: 44 · Different: 41 · Divergent: 11 · Disparate: 4 |
| Lamentations | 144 | Same: 27 · Similar: 51 · Different: 47 · Divergent: 16 · Disparate: 13 |
| Wisdom of Solomon | 427 | Same: 292 · Similar: 103 · Different: 15 · Divergent: 17 |
| Sirach | 1,372 | Same: 904 · Similar: 285 · Different: 72 · Divergent: 105 · Disparate: 6 |

In the five Hebrew-Bible books the KJV translates the Masoretic Hebrew and the Greek column is the Septuagint, so most real differences are Hebrew against Greek (the site's earlier Hebrew–Greek note stays on each card as source context). Wisdom of Solomon and Sirach are mostly Same or Similar because the KJV Apocrypha was translated from the Greek; the Divergent cards there are mainly the extra lines of the longer Sirach text, the two prologues and the verses the Greek main text lacks.

## What changed on each card

- **Psalms–Lamentations (layered cards):** badge "KJV assessment: open" → "Text: <category>"; the layer-1 open sentence → the comparison note; layer 4 "Assessment open · open" → "<category> · focused"; the layer-5 open sentence → the note on how the difference arose. The earlier Hebrew–Greek note is kept. The header's "N KJV semantic classifications remain open" now gives the full tally.
- **Wisdom of Solomon and Sirach (cards without layers):** the "KJV classification pending" badge → "Text: <category>", and a short note below the comparison gives the classification, the comparison and how the difference arose. The shared per-chapter layers no longer say the verse is pending, and the header gives the tally.
- **Still open:** the "Protestant ↔ Medieval Christian" reception rows of layer 4 were not assessed in this round.

## Checks

- A blind re-classification of 100 random KJV cards (and 80 Latin cards) by a separate reader matched exactly in 82% of the 180 cards and within one step in 97%.
- Every page was read back after saving and matched the expected md5. The Parallel Reader's KJV column reads the same text as before (checked word for word for Wisdom of Solomon, the template that gained new markup).
