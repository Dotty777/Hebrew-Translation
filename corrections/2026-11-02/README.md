# Corrections of 2 November 2026: Genesis–Deuteronomy

All changes were made on the **staging** site (staging-8e0d-waywardnightjars.wpcomstaging.com) only; production has not been touched. The pages as they were before any change are in [staging-backups/2026-11-02](../../staging-backups/2026-11-02/) (187 chapter comparison pages and the 5 KJV comparison pages; the 5 Vulgate comparison pages are backed up in [Latin-Translation](https://github.com/Dotty777/Latin-Translation/tree/main/staging-backups/2026-11-02)).

Each data file is in the format the staging helper applies: for every page, the md5 of the page before, the exact edits, and the md5 after. A page whose content had changed is skipped rather than overwritten, and every page was checked after saving.

| File | What it changes | Pages | Edits |
| --- | --- | --- | --- |
| [genesis-hebrew-fixes.json](genesis-hebrew-fixes.json) | Genesis Hebrew–English readings that kept a Septuagint reading now give the Masoretic wording; card notes and highlighted comparisons updated to match. The review behind it is in [genesis-review.json](genesis-review.json) (652 readings read, 45 changed, with the Hebrew basis for each). | 23 | 71 |
| [tags-and-rows.json](tags-and-rows.json) | Editorial verse-number tags ("[MT x:y]", "(H x:y)", "(Chabad x:y)", "BHS/RH x:y") moved out of the Hebrew–English verse text into citations, so the Parallel Reader shows the Masoretic number in the verse label instead of inside Scripture; the 23 Hebrew-only Exodus verses given their own reader rows. | 26 | 317 |
| Exodus 20:16 label | The tag "(H 20:12d)" named the wrong verse; it is part of Masoretic 20:13 (as Deuteronomy 5:17a–d already shows), so it now reads "(H 20:13d)". Applied directly (one edit on page 1235). | 1 | 1 |
| [alignment/](alignment/README.md) | Row alignment: 761 Hebrew, Latin and KJV comparison cards in the versification zones get the Rahlfs reference of the Greek verse they compare, so all four columns of the reader show the same verse on each row. | 22 | 761 |

Latin-column changes of the same day (classification of every open Vulgate card, grouped cards shown once) are recorded in [Latin-Translation corrections/2026-11-02](https://github.com/Dotty777/Latin-Translation/tree/main/corrections/2026-11-02).

## Checks after the changes

- Every Masoretic verse of Genesis–Deuteronomy has a Hebrew–English rendering in the reader (5,847 of 5,847 Masoretic verses, Sefaria numbering), and no reader row lacks its Hebrew verse.
- Row alignment: each Hebrew, Latin and KJV reading was compared with the Saints reading on its own row and on the twelve rows either side. Across the five books, before: 396 readings sat clearly closer to another row; after: 91, nearly all single rows inside formula-heavy passages ("The Lord spoke to Moses, saying") or the Septuagint-order sections of Exodus 35–39, Numbers 1 and Numbers 26, which keep the Greek order by design.
- Highlighting: the Parallel Reader's colour plans still apply to every corrected or moved reading (Latin column 5,817 of 5,820 readings coloured; the three without colours, Exodus 33:7 and Numbers 21:33 and 25:3, had none before).
- The book folders here were recaptured from the reader after all changes (`captured: 2026-11-02`).
