# Parallel Reader row alignment (2 November 2026)

The Parallel Reader places every Hebrew, Latin and KJV comparison card on the Saints row named by the card's
Greek reference. In the Pentateuch's versification zones those references carried the English verse number,
while the Saints rows follow Rahlfs numbering, so whole runs of verses sat one to seven rows away from the
Saints verse they compare (for example Leviticus 6:1–7 = Rahlfs 5:20–26; Numbers 16:36–17:13 = 17:1–28;
Deuteronomy 12:32–13:18, 22:30–23:25 and 29:1–29; Exodus 8 and 22 in the Latin column).

Each card here gets a `data-greek-ref` naming the Rahlfs verse its own Greek reading already is (taken from the
card's stated "LXX x:y" / "BHS/RH x:y", otherwise from the standard English→Rahlfs offsets in the zone). Vulgate
and KJV cards also have their visible "Saints comparison anchor" / "Greek source" label corrected. No reading,
note or classification text changes.

Files: `alignment-hebrew.json.gz` (chapter comparison pages) and one file per Vulgate/KJV comparison page, in the
helper plugin's apply format (md5 of the page before, edits, md5 after). `manifest.json` lists sha256 values.
Multi-reference KJV cards in Exodus 28 and 36–39 and one duplicated Vulgate card (Exodus 37:1) were left as they are.
