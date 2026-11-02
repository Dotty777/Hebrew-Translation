# Wisdom Division KJV ↔ Greek-English classification (Saints.Bible)

Each card pairs one verse of the **King James Version** (`kjv`) with the site's English rendering of the Septuagint Greek (`saints`, the Saints Translation of the Rahlfs–Hanhart Greek). `kjv_ref` and `greek_ref` give each side's own reference; cards are already aligned by content. Your job is to classify every card and write two short texts.

Background you need:
- **Psalms, Proverbs, Ecclesiastes, Song of Songs, Lamentations**: the KJV translates the Masoretic Hebrew; the Greek is the Septuagint. Most real differences therefore reflect Hebrew versus Greek. These cards carry `hebrew_greek_note`, the site's earlier note comparing a Hebrew-English rendering with the same Greek-English; its first word is its category. It is good evidence about the Hebrew–Greek relationship, but your verdict is KJV against Greek-English, judged on the two texts you are shown. In the Psalms the KJV prints titles unnumbered (`KJV Psalm 3 · unnumbered superscription`), while the Greek counts them as verse 1; such cards compare title with title.
- **Wisdom of Solomon, Sirach**: the KJV Apocrypha was translated from Greek (an early printed Greek text, not Rahlfs–Hanhart). In Sirach the KJV follows a text with some extra lines and a different chapter order in 30–36; the KJV also has a translator's Prologue and "A Prologue made by an uncertain Author". Cards where one side reads "No corresponding verse…" or "No counterpart…" have material on one side only.

Ignore, when judging: archaic English (thee, thou, -eth, "unto", "shall"), LORD versus Lord, capitalised pronouns for God, punctuation, KJV supplied words that only make the English read smoothly, and word order. These are English wording and lead to **Same**.

Categories (the site's own definitions):
- **Same**: corresponding content; differences are only English wording or register.
- **Similar**: a modest difference of expression or emphasis (a synonym with a different nuance, singular/plural, a pronoun vs a name, a small particle, tense, or a slightly different construction).
- **Different**: a meaningful local detail differs (a different verb, object, image, number, name, place or condition) while the verse is otherwise parallel.
- **Divergent**: material present in one and absent in the other, or rearranged (a clause, phrase or sentence; a verse the other text does not contain).
- **Disparate**: a major difference of assertion, agency or consequence (one says the opposite, or a different subject does a different thing).

Write per card:
- `category`: one of the five.
- `note`: the layer-1 "English word comparison and meaning" text: 1–2 sentences, at most about 35 words, plain text, no HTML, in the site's style, naming the concrete difference, e.g. "KJV renders the speaker's designation as 'Preacher'; Greek-English retains 'Ecclesiastes' and explicitly adds 'of Israel' to the royal title." For Same, say briefly what agrees and that the difference is English wording, e.g. "Both contrast the LORD's knowledge of the righteous way with the perishing way of the ungodly; the differences are English wording."
- `cause`: the layer-5 "How and why the differences arose" text: one sentence, at most about 30 words. Say what kind of difference it is: English wording only; a lexical or interpretive choice; the KJV following the Hebrew where the Septuagint reads differently (Hebrew books); the KJV's Greek text differing from Rahlfs–Hanhart (Wisdom, Sirach); verse division; an addition or omission. Use the `hebrew_greek_note` where it shows the Hebrew and Greek differ. Do not speculate about copyists, motives or doctrine; where the origin is not certain, say so (e.g. "Whether this reflects a different Greek text or the translators' interpretation is unresolved."). For Same: "The difference is one of English wording; the KJV and Greek-English agree here."

Use ‘single’ or "double" quotes in plain text; never HTML.

## Output

Write a JSON list to the output file named in your task, one object per card, in input order:

```
{"card": "<card id>", "category": "Same" | "Similar" | "Different" | "Divergent" | "Disparate", "note": "<...>", "cause": "<...>"}
```

Every input card must appear exactly once. Validate your file with `python3 -c "import json;json.load(open('<file>'))"`. Write only your own output file; do not create, modify or delete any other file.
