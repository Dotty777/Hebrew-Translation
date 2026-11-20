# Hosea 02 — Saints Hebrew Critical Text

**Division:** `04_Providence` · **Language:** `Hebrew` · **Engine:** `Textual Analysis Brain (Claude-designed · internal evidence · offline)` · **Updated:** `2026-11-18T03:15:56Z`

**Versification:** Masoretic (MT) numbering. Psalms 10–147 carry MT numbers, one higher than the Septuagint/Vulgate psalm numbers used by the Greek and Latin editions. Numbering anchor for this chapter: `WLC (L)`. Spelling and punctuation follow `MAM (Aleppo)` where it attests the adopted reading.

**Sigla in the text:** `⟦ ⟧` = verse absent from (or bracketed by) witnesses that outweigh those containing it — printed for reference, probably not original. `(…)` before a Hebrew word = ketiv, followed by the qere.

---

## Section I — Admitted Witnesses & Gatekeeper Quarantine Declaration

### Admitted Collation Witnesses (Open-Source Tiers 1–4)
| Siglum | Witness Title | Tier | Weight | License | Text-Type |
| :--- | :--- | :---: | :---: | :--- | :--- |
| **MAM (Aleppo)** | Miqra 'al-pi ha-Mesorah (Aleppo Codex Tradition, OSIS XML) | Tier 1 | `0.98` | CC BY-SA 3.0 | Ben Asher Tiberian Masoretic (Aleppo-Weighted) |
| **WLC (L)** | Westminster Leningrad Codex (Firkovich B 19A, 1008 CE) | Tier 1 | `0.96` | Public Domain | Ben Asher Tiberian Masoretic (Leningradensis) |

### Apparatus Witnesses (Majority / Ecclesiastical Editions — recorded, not voting)
Collated against the adopted text and listed in the apparatus wherever they differ in substance; they do not vote on the text.

| Siglum | Witness Title | Tier | License | Text-Type |
| :--- | :--- | :---: | :--- | :--- |
| **BenChayyim (1525)** | Jacob ben Chayyim Masoretic Majority Text (Second Rabbinic Bible Tradition) | Tier 3 | Public Domain | Medieval Masoretic Majority / Rabbinic Bible Textus Receptus |
| **Letteris (1852)** | Meir Halevi Letteris Masoretic Hebrew Bible (1852 / 1866 Edition) | Tier 3 | Public Domain / GPL-3.0 | Van der Hooght / Ben Chayyim / Erfurt Masoretic Majority |

### Disregarded / Quarantined Sources (Excluded by AI Gatekeeper)
| Source | Status | Reason Excluded from Open Critical Text |
| :--- | :---: | :--- |
| Leningrad-USFX [DISREGARDED] | `DISREGARDED_CORRUPT` | AI GATEKEEPER CATCH — DISREGARDED (Corrupt Transcription): Word-boundary spaces were stripped during upstream USFX export and '/' morpheme dividers remain glued inside tokens (e.g., בִּ/שְׁנַ֤תשְׁתַּ֙יִם֙). Superseded by clean WLC TSV and MAM OSIS XML. |

---

## Section II — Continuous Hebrew Critical Text

**1** וְֽ֠הָיָה מִסְפַּ֤ר בְּנֵֽי־יִשְׂרָאֵל֙ כְּח֣וֹל הַיָּ֔ם אֲשֶׁ֥ר לֹֽא־יִמַּ֖ד וְלֹ֣א יִסָּפֵ֑ר וְֽ֠הָיָ֠ה בִּמְק֞וֹם אֲשֶׁר־יֵאָמֵ֤ר לָהֶם֙ לֹא־עַמִּ֣י אַתֶּ֔ם יֵאָמֵ֥ר לָהֶ֖ם בְּנֵ֥י אֵֽל־חָֽי׃
**2** וְ֠נִקְבְּצ֠וּ בְּנֵֽי־יְהוּדָ֤ה וּבְנֵֽי־יִשְׂרָאֵל֙ יַחְדָּ֔ו וְשָׂמ֥וּ לָהֶ֛ם רֹ֥אשׁ אֶחָ֖ד וְעָל֣וּ מִן־הָאָ֑רֶץ כִּ֥י גָד֖וֹל י֥וֹם יִזְרְעֶֽאל׃
**3** אִמְר֥וּ לַאֲחֵיכֶ֖ם עַמִּ֑י וְלַאֲחוֹתֵיכֶ֖ם רֻחָֽמָה׃
**4** רִ֤יבוּ בְאִמְּכֶם֙ רִ֔יבוּ כִּי־הִיא֙ לֹ֣א אִשְׁתִּ֔י וְאָנֹכִ֖י לֹ֣א אִישָׁ֑הּ וְתָסֵ֤ר זְנוּנֶ֙יהָ֙ מִפָּנֶ֔יהָ וְנַאֲפוּפֶ֖יהָ מִבֵּ֥ין שָׁדֶֽיהָ׃
**5** פֶּן־אַפְשִׁיטֶ֣נָּה עֲרֻמָּ֔ה וְהִ֨צַּגְתִּ֔יהָ כְּי֖וֹם הִוָּֽלְדָ֑הּ וְשַׂמְתִּ֣יהָ כַמִּדְבָּ֗ר וְשַׁתִּ֙הָ֙ כְּאֶ֣רֶץ צִיָּ֔ה וַהֲמִתִּ֖יהָ בַּצָּמָֽא׃
**6** וְאֶת־בָּנֶ֖יהָ לֹ֣א אֲרַחֵ֑ם כִּֽי־בְנֵ֥י זְנוּנִ֖ים הֵֽמָּה׃
**7** כִּ֤י זָֽנְתָה֙ אִמָּ֔ם הֹבִ֖ישָׁה הוֹרָתָ֑ם כִּ֣י אָמְרָ֗ה אֵלְכָ֞ה אַחֲרֵ֤י מְאַֽהֲבַי֙ נֹתְנֵ֤י לַחְמִי֙ וּמֵימַ֔י צַמְרִ֣י וּפִשְׁתִּ֔י שַׁמְנִ֖י וְשִׁקּוּיָֽי׃
**8** לָכֵ֛ן הִנְנִי־שָׂ֥ךְ אֶת־דַּרְכֵּ֖ךְ בַּסִּירִ֑ים וְגָֽדַרְתִּי֙ אֶת־גְּדֵרָ֔הּ וּנְתִיבוֹתֶ֖יהָ לֹ֥א תִמְצָֽא׃
**9** וְרִדְּפָ֤ה אֶת־מְאַהֲבֶ֙יהָ֙ וְלֹא־תַשִּׂ֣יג אֹתָ֔ם וּבִקְשָׁ֖תַם וְלֹ֣א תִמְצָ֑א וְאָמְרָ֗ה אֵלְכָ֤ה וְאָשׁ֙וּבָה֙ אֶל־אִישִׁ֣י הָרִאשׁ֔וֹן כִּ֣י ט֥וֹב לִ֛י אָ֖ז מֵעָֽתָּה׃
**10** וְהִיא֙ לֹ֣א יָֽדְעָ֔ה כִּ֤י אָנֹכִי֙ נָתַ֣תִּי לָ֔הּ הַדָּגָ֖ן וְהַתִּיר֣וֹשׁ וְהַיִּצְהָ֑ר וְכֶ֨סֶף הִרְבֵּ֥יתִי לָ֛הּ וְזָהָ֖ב עָשׂ֥וּ לַבָּֽעַל׃
**11** לָכֵ֣ן אָשׁ֔וּב וְלָקַחְתִּ֤י דְגָנִי֙ בְּעִתּ֔וֹ וְתִירוֹשִׁ֖י בְּמוֹעֲד֑וֹ וְהִצַּלְתִּי֙ צַמְרִ֣י וּפִשְׁתִּ֔י לְכַסּ֖וֹת אֶת־עֶרְוָתָֽהּ׃
**12** וְעַתָּ֛ה אֲגַלֶּ֥ה אֶת־נַבְלֻתָ֖הּ לְעֵינֵ֣י מְאַהֲבֶ֑יהָ וְאִ֖ישׁ לֹא־יַצִּילֶ֥נָּה מִיָּדִֽי׃
**13** וְהִשְׁבַּתִּי֙ כׇּל־מְשׂוֹשָׂ֔הּ חַגָּ֖הּ חׇדְשָׁ֣הּ וְשַׁבַּתָּ֑הּ וְכֹ֖ל מוֹעֲדָֽהּ׃
**14** וַהֲשִׁמֹּתִ֗י גַּפְנָהּ֙ וּתְאֵ֣נָתָ֔הּ אֲשֶׁ֣ר אָמְרָ֗ה אֶתְנָ֥ה הֵ֙מָּה֙ לִ֔י אֲשֶׁ֥ר נָתְנוּ־לִ֖י מְאַהֲבָ֑י וְשַׂמְתִּ֣ים לְיַ֔עַר וַאֲכָלָ֖תַם חַיַּ֥ת הַשָּׂדֶֽה׃
**15** וּפָקַדְתִּ֣י עָלֶ֗יהָ אֶת־יְמֵ֤י הַבְּעָלִים֙ אֲשֶׁ֣ר תַּקְטִ֣יר לָהֶ֔ם וַתַּ֤עַד נִזְמָהּ֙ וְחֶלְיָתָ֔הּ וַתֵּ֖לֶךְ אַחֲרֵ֣י מְאַהֲבֶ֑יהָ וְאֹתִ֥י שָׁכְחָ֖ה נְאֻם־יְהֹוָֽה׃
**16** לָכֵ֗ן הִנֵּ֤ה אָנֹכִי֙ מְפַתֶּ֔יהָ וְהֹלַכְתִּ֖יהָ הַמִּדְבָּ֑ר וְדִבַּרְתִּ֖י עַל־לִבָּֽהּ׃
**17** וְנָתַ֨תִּי לָ֤הּ אֶת־כְּרָמֶ֙יהָ֙ מִשָּׁ֔ם וְאֶת־עֵ֥מֶק עָכ֖וֹר לְפֶ֣תַח תִּקְוָ֑ה וְעָ֤נְתָה שָּׁ֙מָּה֙ כִּימֵ֣י נְעוּרֶ֔יהָ וּכְי֖וֹם עֲלוֹתָ֥הּ מֵאֶרֶץ־מִצְרָֽיִם׃
**18** וְהָיָ֤ה בַיּוֹם־הַהוּא֙ נְאֻם־יְהֹוָ֔ה תִּקְרְאִ֖י אִישִׁ֑י וְלֹא־תִקְרְאִי־לִ֥י ע֖וֹד בַּעְלִֽי׃
**19** וַהֲסִרֹתִ֛י אֶת־שְׁמ֥וֹת הַבְּעָלִ֖ים מִפִּ֑יהָ וְלֹא־יִזָּכְר֥וּ ע֖וֹד בִּשְׁמָֽם׃
**20** וְכָרַתִּ֨י לָהֶ֤ם בְּרִית֙ בַּיּ֣וֹם הַה֔וּא עִם־חַיַּ֤ת הַשָּׂדֶה֙ וְעִם־ע֣וֹף הַשָּׁמַ֔יִם וְרֶ֖מֶשׂ הָאֲדָמָ֑ה וְקֶ֨שֶׁת וְחֶ֤רֶב וּמִלְחָמָה֙ אֶשְׁבּ֣וֹר מִן־הָאָ֔רֶץ וְהִשְׁכַּבְתִּ֖ים לָבֶֽטַח׃
**21** וְאֵרַשְׂתִּ֥יךְ לִ֖י לְעוֹלָ֑ם וְאֵרַשְׂתִּ֥יךְ לִי֙ בְּצֶ֣דֶק וּבְמִשְׁפָּ֔ט וּבְחֶ֖סֶד וּֽבְרַחֲמִֽים׃
**22** וְאֵרַשְׂתִּ֥יךְ לִ֖י בֶּאֱמוּנָ֑ה וְיָדַ֖עַתְּ אֶת־יְהֹוָֽה׃
**23** וְהָיָ֣ה ׀ בַּיּ֣וֹם הַה֗וּא אֶֽעֱנֶה֙ נְאֻם־יְהֹוָ֔ה אֶעֱנֶ֖ה אֶת־הַשָּׁמָ֑יִם וְהֵ֖ם יַעֲנ֥וּ אֶת־הָאָֽרֶץ׃
**24** וְהָאָ֣רֶץ תַּעֲנֶ֔ה אֶת־הַדָּגָ֖ן וְאֶת־הַתִּיר֣וֹשׁ וְאֶת־הַיִּצְהָ֑ר וְהֵ֖ם יַעֲנ֥וּ אֶֽת־יִזְרְעֶֽאל׃
**25** וּזְרַעְתִּ֤יהָ לִּי֙ בָּאָ֔רֶץ וְרִחַמְתִּ֖י אֶת־לֹ֣א רֻחָ֑מָה וְאָמַרְתִּ֤י לְלֹֽא־עַמִּי֙ עַמִּי־אַ֔תָּה וְה֖וּא יֹאמַ֥ר אֱלֹהָֽי׃

---

## Section III — Critical Apparatus & Disregarded Surface Noise

### Hosea 2:1
- *Disregarded Surface Variant:* kept `וְֽ֠הָיָ֠ה` over `וְֽ֠הָיָה` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `לֹא־` over `לֹֽא־` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*

### Hosea 2:2
- *Disregarded Surface Variant:* kept `וְ֠נִקְבְּצ֠וּ` over `וְ֠נִקְבְּצוּ` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*

### Hosea 2:3
- *Disregarded Surface Variant:* kept `וְלַאֲחוֹתֵיכֶ֖ם` over `וְלַאֲחֽוֹתֵיכֶ֖ם` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*

### Hosea 2:4
- *Disregarded Surface Variant:* kept `כִּי־` over `כִּֽי־` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `מִפָּנֶ֔יהָ` over `מִפָּנֶ֔יה` (WLC (L)) — *Pointing convention, Aleppo tradition (MAM) vs Leningrad (WLC): a vowel point left out by one edition*
- *Disregarded Surface Variant:* kept `(adopted text)` over `מִפָּנֶ֔יהָ / מִפָּנֶ֔יה`, `מִפָּנֶ֔יהָ / מִפָּנֶ֔יה` (BenChayyim (1525), Letteris (1852)) — *Apparatus witness, not a variant: Masoretic pointing / cantillation convention of the edition (same consonants)*

### Hosea 2:7
- *Disregarded Surface Variant:* kept `הוֹרָתָ֑ם` over `הֽוֹרָתָ֑ם` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `מְאַֽהֲבַי֙` over `מְאַהֲבַי֙` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*

### Hosea 2:9
- *Disregarded Surface Variant:* kept `וְלֹא־` over `וְלֹֽא־` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `הָרִאשׁ֔וֹן` over `הָֽרִאשׁ֔וֹן` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `(adopted text)` over `הָרִאשׁ֔וֹן / הָֽרִאשֹׁ֔ון` (BenChayyim (1525)) — *Apparatus witness, not a variant: Masoretic pointing / cantillation convention of the edition (same consonants)*

### Hosea 2:10
- *Disregarded Surface Variant:* kept `אָנֹכִי֙` over `אָֽנֹכִי֙` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*

### Hosea 2:11
- *Disregarded Surface Variant:* kept `בְּמוֹעֲד֑וֹ` over `בְּמֽוֹעֲד֑וֹ` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `(adopted text)` over `בְּעִתּ֔וֹ / בְּעִתֹּ֔ו`, `לְכַסּ֖וֹת / לְכַסֹּ֖ות` (BenChayyim (1525)) — *Apparatus witness, not a variant: Masoretic pointing / cantillation convention of the edition (same consonants)*

### Hosea 2:12
- *Disregarded Surface Variant:* kept `לֹא־` over `לֹֽא־` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*

### Hosea 2:13
- *Disregarded Surface Variant:* kept `כׇּל־` over `כָּל־` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `חׇדְשָׁ֣הּ` over `חָדְשָׁ֣הּ` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `(adopted text)` over `מְשׂוֹשָׂ֔הּ / מְשֹׂושָׂ֔הּ` (BenChayyim (1525)) — *Apparatus witness, not a variant: Masoretic pointing / cantillation convention of the edition (same consonants)*

### Hosea 2:14
- *Disregarded Surface Variant:* kept `נָתְנוּ־` over `נָֽתְנוּ־` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `מְאַהֲבָ֑י` over `מְאַֽהֲבָ֑י` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*

### Hosea 2:15
- *Disregarded Surface Variant:* kept `יְהֹוָֽה׃` over `יְהוָֽה׃` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*

### Hosea 2:16
- *Disregarded Surface Variant:* kept `אָנֹכִי֙` over `אָֽנֹכִי֙` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `וְהֹלַכְתִּ֖יהָ` over `וְהֹֽלַכְתִּ֖יהָ` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `עַל־` over `עַל` (WLC (L)) — *Punctuation / spacing difference only*

### Hosea 2:17
- **Apparatus:** `וּכְי֖וֹם` MAM (Aleppo) BenChayyim (1525) Letteris (1852) **]** **וִּכְי֖וֹם** WLC (L) *(lexical substitution)*
  - *external: independent streams:* Adopted reading: Aleppo tradition (MAM); other reading(s): Leningrad Codex (WLC).
  - *external: two-stream policy:* Aleppo tradition (MAM) against the Leningrad Codex (WLC): a codex-level difference within the Masoretic text. MAM is followed.
- *Disregarded Surface Variant:* kept `עֲלוֹתָ֥הּ` over `עֲלֹתָ֥הּ` (WLC (L)) — *Plene / defective spelling (mater lectionis)*
- *Disregarded Surface Variant:* kept `מֵאֶרֶץ־` over `מֵאֶֽרֶץ־` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `(adopted text)` over `וּכְי֖וֹם עֲלוֹתָ֥הּ / וִּכְי֖וֹם עֲלֹתָ֥הּ` (BenChayyim (1525)) — *Apparatus witness, not a variant: Plene / defective spelling (vav or yod as a vowel letter)*

### Hosea 2:18
- *Disregarded Surface Variant:* kept `יְהֹוָ֔ה` over `יְהוָ֔ה` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `וְלֹא־` over `וְלֹֽא־` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `(adopted text)` over `בַיּוֹם־ / בַיֹּום־` (BenChayyim (1525)) — *Apparatus witness, not a variant: Masoretic pointing / cantillation convention of the edition (same consonants)*

### Hosea 2:19
- *Disregarded Surface Variant:* kept `וְלֹא־` over `וְלֹֽא־` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*

### Hosea 2:20
- *Disregarded Surface Variant:* kept `הָאֲדָמָ֑ה` over `הָֽאֲדָמָ֑ה` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `(adopted text)` over `בַּיּ֣וֹם / בַּיֹּ֣ום`, `אֶשְׁבּ֣וֹר / אֶשְׁבֹּ֣ור` (BenChayyim (1525)) — *Apparatus witness, not a variant: Masoretic pointing / cantillation convention of the edition (same consonants)*

### Hosea 2:22
- *Disregarded Surface Variant:* kept `יְהֹוָֽה׃` over `יְהוָֽה׃` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*

### Hosea 2:23
- *Disregarded Surface Variant:* kept `יְהֹוָ֔ה` over `יְהוָ֔ה` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*
- *Disregarded Surface Variant:* kept `(adopted text)` over `בַּיּ֣וֹם / בַּיֹּ֣ום` (BenChayyim (1525)) — *Apparatus witness, not a variant: Masoretic pointing / cantillation convention of the edition (same consonants)*

### Hosea 2:25
- *Disregarded Surface Variant:* kept `וְרִחַמְתִּ֖י` over `וְרִֽחַמְתִּ֖י` (WLC (L)) — *Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention*

---

## Section IV — Verse-by-Verse Text-Critical Rationale & Witness Matrix

### Verse 1 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וְֽ֠הָיָה מִסְפַּ֤ר בְּנֵֽי־יִשְׂרָאֵל֙ כְּח֣וֹל הַיָּ֔ם אֲשֶׁ֥ר לֹֽא־יִמַּ֖ד וְלֹ֣א יִסָּפֵ֑ר וְֽ֠הָיָ֠ה בִּמְק֞וֹם אֲשֶׁר־יֵאָמֵ֤ר לָהֶם֙ לֹא־עַמִּ֣י אַתֶּ֔ם יֵאָמֵ֥ר לָהֶ֖ם בְּנֵ֥י אֵֽל־חָֽי׃
  - `MAM (Aleppo)`: וְֽ֠הָיָה מִסְפַּ֤ר בְּנֵֽי־יִשְׂרָאֵל֙ כְּח֣וֹל הַיָּ֔ם אֲשֶׁ֥ר לֹֽא־יִמַּ֖ד וְלֹ֣א יִסָּפֵ֑ר וְֽ֠הָיָ֠ה בִּמְק֞וֹם אֲשֶׁר־יֵאָמֵ֤ר לָהֶם֙ לֹא־עַמִּ֣י אַתֶּ֔ם יֵאָמֵ֥ר לָהֶ֖ם בְּנֵ֥י אֵֽל־חָֽי׃
  - `WLC (L)`: וְֽ֠הָיָה מִסְפַּ֤ר בְּנֵֽי־יִשְׂרָאֵל֙ כְּח֣וֹל הַיָּ֔ם אֲשֶׁ֥ר לֹֽא־יִמַּ֖ד וְלֹ֣א יִסָּפֵ֑ר וְֽ֠הָיָה בִּמְק֞וֹם אֲשֶׁר־יֵאָמֵ֤ר לָהֶם֙ לֹֽא־עַמִּ֣י אַתֶּ֔ם יֵאָמֵ֥ר לָהֶ֖ם בְּנֵ֥י אֵֽל־חָֽי׃
  - `BenChayyim (1525)`: וְֽ֠הָיָה מִסְפַּ֤ר בְּנֵֽי־יִשְׂרָאֵל֙ כְּח֣וֹל הַיָּ֔ם אֲשֶׁ֥ר לֹֽא־יִמַּ֖ד וְלֹ֣א יִסָּפֵ֑ר וְֽ֠הָיָה בִּמְק֞וֹם אֲשֶׁר־יֵאָמֵ֤ר לָהֶם֙ לֹֽא־עַמִּ֣י אַתֶּ֔ם יֵאָמֵ֥ר לָהֶ֖ם בְּנֵ֥י אֵֽל־חָֽי׃
  - `Letteris (1852)`: וְֽ֠הָיָה מִסְפַּ֤ר בְּנֵֽי־יִשְׂרָאֵל֨ כְּח֣וֹל הַיָּ֔ם אֲשֶׁ֥ר לֹֽא־יִמַּ֖ד וְלֹ֣א יִסָּפֵ֑ר וְֽ֠הָיָה בִּמְק֞וֹם אֲשֶׁר־יֵֽאָמֵ֤ר לָהֶם֙ לֹֽא־עַמִּ֣י אַתֶּ֔ם יֵֽאָמֵ֥ר לָהֶ֖ם בְּנֵ֥י אֵֽל־חָֽי׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 2 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 2 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וְ֠נִקְבְּצ֠וּ בְּנֵֽי־יְהוּדָ֤ה וּבְנֵֽי־יִשְׂרָאֵל֙ יַחְדָּ֔ו וְשָׂמ֥וּ לָהֶ֛ם רֹ֥אשׁ אֶחָ֖ד וְעָל֣וּ מִן־הָאָ֑רֶץ כִּ֥י גָד֖וֹל י֥וֹם יִזְרְעֶֽאל׃
  - `MAM (Aleppo)`: וְ֠נִקְבְּצ֠וּ בְּנֵֽי־יְהוּדָ֤ה וּבְנֵֽי־יִשְׂרָאֵל֙ יַחְדָּ֔ו וְשָׂמ֥וּ לָהֶ֛ם רֹ֥אשׁ אֶחָ֖ד וְעָל֣וּ מִן־הָאָ֑רֶץ כִּ֥י גָד֖וֹל י֥וֹם יִזְרְעֶֽאל׃
  - `WLC (L)`: וְ֠נִקְבְּצוּ בְּנֵֽי־יְהוּדָ֤ה וּבְנֵֽי־יִשְׂרָאֵל֙ יַחְדָּ֔ו וְשָׂמ֥וּ לָהֶ֛ם רֹ֥אשׁ אֶחָ֖ד וְעָל֣וּ מִן־הָאָ֑רֶץ כִּ֥י גָד֖וֹל י֥וֹם יִזְרְעֶֽאל׃
  - `BenChayyim (1525)`: וְ֠נִקְבְּצוּ בְּנֵֽי־יְהוּדָ֤ה וּבְנֵֽי־יִשְׂרָאֵל֙ יַחְדָּ֔ו וְשָׂמ֥וּ לָהֶ֛ם רֹ֥אשׁ אֶחָ֖ד וְעָל֣וּ מִן־הָאָ֑רֶץ כִּ֥י גָד֖וֹל י֥וֹם יִזְרְעֶֽאל׃
  - `Letteris (1852)`: וְ֠נִקְבְּצוּ בְּנֵֽי־יְהוּדָ֤ה וּבְנֵֽי־יִשְׂרָאֵל֨ יַחְדָּ֔ו וְשָׂמ֥וּ לָהֶ֛ם רֹ֥אשׁ אֶחָ֖ד וְעָל֣וּ מִן־הָאָ֑רֶץ כִּ֥י גָד֖וֹל י֥וֹם יִזְרְעֶֽאל׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 1 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 3 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** אִמְר֥וּ לַאֲחֵיכֶ֖ם עַמִּ֑י וְלַאֲחוֹתֵיכֶ֖ם רֻחָֽמָה׃
  - `MAM (Aleppo)`: אִמְר֥וּ לַאֲחֵיכֶ֖ם עַמִּ֑י וְלַאֲחוֹתֵיכֶ֖ם רֻחָֽמָה׃
  - `WLC (L)`: אִמְר֥וּ לַאֲחֵיכֶ֖ם עַמִּ֑י וְלַאֲחֽוֹתֵיכֶ֖ם רֻחָֽמָה׃
  - `BenChayyim (1525)`: אִמְר֥וּ לַאֲחֵיכֶ֖ם עַמִּ֑י וְלַאֲחֽוֹתֵיכֶ֖ם רֻחָֽמָה׃
  - `Letteris (1852)`: אִמְר֥וּ לַֽאֲחֵיכֶ֖ם עַמִּ֑י וְלַֽאֲחֽוֹתֵיכֶ֖ם רֻחָֽמָה׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 1 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 4 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** רִ֤יבוּ בְאִמְּכֶם֙ רִ֔יבוּ כִּי־הִיא֙ לֹ֣א אִשְׁתִּ֔י וְאָנֹכִ֖י לֹ֣א אִישָׁ֑הּ וְתָסֵ֤ר זְנוּנֶ֙יהָ֙ מִפָּנֶ֔יהָ וְנַאֲפוּפֶ֖יהָ מִבֵּ֥ין שָׁדֶֽיהָ׃
  - `MAM (Aleppo)`: רִ֤יבוּ בְאִמְּכֶם֙ רִ֔יבוּ כִּי־הִיא֙ לֹ֣א אִשְׁתִּ֔י וְאָנֹכִ֖י לֹ֣א אִישָׁ֑הּ וְתָסֵ֤ר זְנוּנֶ֙יהָ֙ מִפָּנֶ֔יהָ וְנַאֲפוּפֶ֖יהָ מִבֵּ֥ין שָׁדֶֽיהָ׃
  - `WLC (L)`: רִ֤יבוּ בְאִמְּכֶם֙ רִ֔יבוּ כִּֽי־הִיא֙ לֹ֣א אִשְׁתִּ֔י וְאָנֹכִ֖י לֹ֣א אִישָׁ֑הּ וְתָסֵ֤ר זְנוּנֶ֙יהָ֙ מִפָּנֶ֔יה וְנַאֲפוּפֶ֖יהָ מִבֵּ֥ין שָׁדֶֽיהָ׃
  - `BenChayyim (1525)`: רִ֤יבוּ בְאִמְּכֶם֙ רִ֔יבוּ כִּֽי־הִיא֙ לֹ֣א אִשְׁתִּ֔י וְאָנֹכִ֖י לֹ֣א אִישָׁ֑הּ וְתָסֵ֤ר זְנוּנֶ֙יהָ֙ מִפָּנֶ֔יה וְנַאֲפוּפֶ֖יהָ מִבֵּ֥ין שָׁדֶֽיהָ׃
  - `Letteris (1852)`: רִ֤יבוּ בְאִמְּכֶם֨ רִ֔יבוּ כִּי־הִיא֨ לֹ֣א אִשְׁתִּ֔י וְאָֽנֹכִ֖י לֹ֣א אִישָׁ֑הּ וְתָסֵ֤ר זְנוּנֶ֙יהָ֨ מִפָּנֶ֔יה וְנַֽאֲפוּפֶ֖יהָ מִבֵּ֥ין שָׁדֶֽיהָ׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 2 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention; Pointing convention, Aleppo tradition (MAM) vs Leningrad (WLC): a vowel point left out by one edition).

### Verse 5 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** פֶּן־אַפְשִׁיטֶ֣נָּה עֲרֻמָּ֔ה וְהִ֨צַּגְתִּ֔יהָ כְּי֖וֹם הִוָּֽלְדָ֑הּ וְשַׂמְתִּ֣יהָ כַמִּדְבָּ֗ר וְשַׁתִּ֙הָ֙ כְּאֶ֣רֶץ צִיָּ֔ה וַהֲמִתִּ֖יהָ בַּצָּמָֽא׃
  - `MAM (Aleppo)`: פֶּן־אַפְשִׁיטֶ֣נָּה עֲרֻמָּ֔ה וְהִ֨צַּגְתִּ֔יהָ כְּי֖וֹם הִוָּֽלְדָ֑הּ וְשַׂמְתִּ֣יהָ כַמִּדְבָּ֗ר וְשַׁתִּ֙הָ֙ כְּאֶ֣רֶץ צִיָּ֔ה וַהֲמִתִּ֖יהָ בַּצָּמָֽא׃
  - `WLC (L)`: פֶּן־אַפְשִׁיטֶ֣נָּה עֲרֻמָּ֔ה וְהִ֨צַּגְתִּ֔יהָ כְּי֖וֹם הִוָּֽלְדָ֑הּ וְשַׂמְתִּ֣יהָ כַמִּדְבָּ֗ר וְשַׁתִּ֙הָ֙ כְּאֶ֣רֶץ צִיָּ֔ה וַהֲמִתִּ֖יהָ בַּצָּמָֽא׃
  - `BenChayyim (1525)`: פֶּן־אַפְשִׁיטֶ֣נָּה עֲרֻמָּ֔ה וְהִ֨צַּגְתִּ֔יהָ כְּי֖וֹם הִוָּֽלְדָ֑הּ וְשַׂמְתִּ֣יהָ כַמִּדְבָּ֗ר וְשַׁתִּ֙הָ֙ כְּאֶ֣רֶץ צִיָּ֔ה וַהֲמִתִּ֖יהָ בַּצָּמָֽא׃
  - `Letteris (1852)`: פֶּן־אַפְשִׁיטֶ֣נָּה עֲרֻמָּ֔ה וְהִ֨צַּגְתִּ֔יהָ כְּי֖וֹם הִוָּֽלְדָ֑הּ וְשַׂמְתִּ֣יהָ כַמִּדְבָּ֗ר וְשַׁתִּ֙הָ֙ כְּאֶ֣רֶץ צִיָּ֔ה וַֽהֲמִתִּ֖יהָ בַּצָּמָֽא׃
- **Philological Rationale:** Unanimous witness agreement across MAM (Aleppo), WLC (L) (2 admitted witnesses; zero substantive divergence).

### Verse 6 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וְאֶת־בָּנֶ֖יהָ לֹ֣א אֲרַחֵ֑ם כִּֽי־בְנֵ֥י זְנוּנִ֖ים הֵֽמָּה׃
  - `MAM (Aleppo)`: וְאֶת־בָּנֶ֖יהָ לֹ֣א אֲרַחֵ֑ם כִּֽי־בְנֵ֥י זְנוּנִ֖ים הֵֽמָּה׃
  - `WLC (L)`: וְאֶת־בָּנֶ֖יהָ לֹ֣א אֲרַחֵ֑ם כִּֽי־בְנֵ֥י זְנוּנִ֖ים הֵֽמָּה׃
  - `BenChayyim (1525)`: וְאֶת־בָּנֶ֖יהָ לֹ֣א אֲרַחֵ֑ם כִּֽי־בְנֵ֥י זְנוּנִ֖ים הֵֽמָּה׃
  - `Letteris (1852)`: וְאֶת־בָּנֶ֖יהָ לֹ֣א אֲרַחֵ֑ם כִּֽי־בְנֵ֥י זְנוּנִ֖ים הֵֽמָּה׃
- **Philological Rationale:** Unanimous witness agreement across MAM (Aleppo), WLC (L) (2 admitted witnesses; zero substantive divergence).

### Verse 7 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** כִּ֤י זָֽנְתָה֙ אִמָּ֔ם הֹבִ֖ישָׁה הוֹרָתָ֑ם כִּ֣י אָמְרָ֗ה אֵלְכָ֞ה אַחֲרֵ֤י מְאַֽהֲבַי֙ נֹתְנֵ֤י לַחְמִי֙ וּמֵימַ֔י צַמְרִ֣י וּפִשְׁתִּ֔י שַׁמְנִ֖י וְשִׁקּוּיָֽי׃
  - `MAM (Aleppo)`: כִּ֤י זָֽנְתָה֙ אִמָּ֔ם הֹבִ֖ישָׁה הוֹרָתָ֑ם כִּ֣י אָמְרָ֗ה אֵלְכָ֞ה אַחֲרֵ֤י מְאַֽהֲבַי֙ נֹתְנֵ֤י לַחְמִי֙ וּמֵימַ֔י צַמְרִ֣י וּפִשְׁתִּ֔י שַׁמְנִ֖י וְשִׁקּוּיָֽי׃
  - `WLC (L)`: כִּ֤י זָֽנְתָה֙ אִמָּ֔ם הֹבִ֖ישָׁה הֽוֹרָתָ֑ם כִּ֣י אָמְרָ֗ה אֵלְכָ֞ה אַחֲרֵ֤י מְאַהֲבַי֙ נֹתְנֵ֤י לַחְמִי֙ וּמֵימַ֔י צַמְרִ֣י וּפִשְׁתִּ֔י שַׁמְנִ֖י וְשִׁקּוּיָֽי׃
  - `BenChayyim (1525)`: כִּ֤י זָֽנְתָה֙ אִמָּ֔ם הֹבִ֖ישָׁה הֽוֹרָתָ֑ם כִּ֣י אָמְרָ֗ה אֵלְכָ֞ה אַחֲרֵ֤י מְאַהֲבַי֙ נֹתְנֵ֤י לַחְמִי֙ וּמֵימַ֔י צַמְרִ֣י וּפִשְׁתִּ֔י שַׁמְנִ֖י וְשִׁקּוּיָֽי׃
  - `Letteris (1852)`: כִּ֤י זָֽנְתָה֙ אִמָּ֔ם הֹבִ֖ישָׁה הֽוֹרָתָ֑ם כִּ֣י אָֽמְרָ֗ה אֵֽלְכָ֞ה אַֽחֲרֵ֤י מְאַֽהֲבַי֨ נֹֽתְנֵ֤י לַחְמִי֨ וּמֵימַ֔י צַמְרִ֣י וּפִשְׁתִּ֔י שַׁמְנִ֖י וְשִׁקּוּיָֽי׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 2 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 8 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** לָכֵ֛ן הִנְנִי־שָׂ֥ךְ אֶת־דַּרְכֵּ֖ךְ בַּסִּירִ֑ים וְגָֽדַרְתִּי֙ אֶת־גְּדֵרָ֔הּ וּנְתִיבוֹתֶ֖יהָ לֹ֥א תִמְצָֽא׃
  - `MAM (Aleppo)`: לָכֵ֛ן הִנְנִי־שָׂ֥ךְ אֶת־דַּרְכֵּ֖ךְ בַּסִּירִ֑ים וְגָֽדַרְתִּי֙ אֶת־גְּדֵרָ֔הּ וּנְתִיבוֹתֶ֖יהָ לֹ֥א תִמְצָֽא׃
  - `WLC (L)`: לָכֵ֛ן הִנְנִי־שָׂ֥ךְ אֶת־דַּרְכֵּ֖ךְ בַּסִּירִ֑ים וְגָֽדַרְתִּי֙ אֶת־גְּדֵרָ֔הּ וּנְתִיבוֹתֶ֖יהָ לֹ֥א תִמְצָֽא׃
  - `BenChayyim (1525)`: לָכֵ֛ן הִנְנִי־שָׂ֥ךְ אֶת־דַּרְכֵּ֖ךְ בַּסִּירִ֑ים וְגָֽדַרְתִּי֙ אֶת־גְּדֵרָ֔הּ וּנְתִיבוֹתֶ֖יהָ לֹ֥א תִמְצָֽא׃
  - `Letteris (1852)`: לָכֵ֛ן הִֽנְנִי־שָׂ֥ךְ אֶת־דַּרְכֵּ֖ךְ בַּסִּירִ֑ים וְגָֽדַרְתִּי֨ אֶת־גְּדֵרָ֔הּ וּנְתִֽיבוֹתֶ֖יהָ לֹ֥א תִמְצָֽא׃
- **Philological Rationale:** Unanimous witness agreement across MAM (Aleppo), WLC (L) (2 admitted witnesses; zero substantive divergence).

### Verse 9 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וְרִדְּפָ֤ה אֶת־מְאַהֲבֶ֙יהָ֙ וְלֹא־תַשִּׂ֣יג אֹתָ֔ם וּבִקְשָׁ֖תַם וְלֹ֣א תִמְצָ֑א וְאָמְרָ֗ה אֵלְכָ֤ה וְאָשׁ֙וּבָה֙ אֶל־אִישִׁ֣י הָרִאשׁ֔וֹן כִּ֣י ט֥וֹב לִ֛י אָ֖ז מֵעָֽתָּה׃
  - `MAM (Aleppo)`: וְרִדְּפָ֤ה אֶת־מְאַהֲבֶ֙יהָ֙ וְלֹא־תַשִּׂ֣יג אֹתָ֔ם וּבִקְשָׁ֖תַם וְלֹ֣א תִמְצָ֑א וְאָמְרָ֗ה אֵלְכָ֤ה וְאָשׁ֙וּבָה֙ אֶל־אִישִׁ֣י הָרִאשׁ֔וֹן כִּ֣י ט֥וֹב לִ֛י אָ֖ז מֵעָֽתָּה׃
  - `WLC (L)`: וְרִדְּפָ֤ה אֶת־מְאַהֲבֶ֙יהָ֙ וְלֹֽא־תַשִּׂ֣יג אֹתָ֔ם וּבִקְשָׁ֖תַם וְלֹ֣א תִמְצָ֑א וְאָמְרָ֗ה אֵלְכָ֤ה וְאָשׁ֙וּבָה֙ אֶל־אִישִׁ֣י הָֽרִאשׁ֔וֹן כִּ֣י ט֥וֹב לִ֛י אָ֖ז מֵעָֽתָּה׃
  - `BenChayyim (1525)`: וְרִדְּפָ֤ה אֶת־מְאַהֲבֶ֙יהָ֙ וְלֹֽא־תַשִּׂ֣יג אֹתָ֔ם וּבִקְשָׁ֖תַם וְלֹ֣א תִמְצָ֑א וְאָמְרָ֗ה אֵלְכָ֤ה וְאָשׁ֙וּבָה֙ אֶל־אִישִׁ֣י הָֽרִאשֹׁ֔ון כִּ֣י ט֥וֹב לִ֛י אָ֖ז מֵעָֽתָּה׃
  - `Letteris (1852)`: וְרִדְּפָ֤ה אֶת־מְאַֽהֲבֶ֨יהָ֨ וְלֹֽא־תַשִּׂ֣יג אֹתָ֔ם וּבִקְשָׁ֖תַם וְלֹ֣א תִמְצָ֑א וְאָֽמְרָ֗ה אֵֽלְכָ֤ה וְאָשׁ֨וּבָה֨ אֶל־אִישִׁ֣י הָֽרִאשׁ֔וֹן כִּ֣י ט֥וֹב לִ֛י אָ֖ז מֵעָֽתָּה׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 2 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 10 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וְהִיא֙ לֹ֣א יָֽדְעָ֔ה כִּ֤י אָנֹכִי֙ נָתַ֣תִּי לָ֔הּ הַדָּגָ֖ן וְהַתִּיר֣וֹשׁ וְהַיִּצְהָ֑ר וְכֶ֨סֶף הִרְבֵּ֥יתִי לָ֛הּ וְזָהָ֖ב עָשׂ֥וּ לַבָּֽעַל׃
  - `MAM (Aleppo)`: וְהִיא֙ לֹ֣א יָֽדְעָ֔ה כִּ֤י אָנֹכִי֙ נָתַ֣תִּי לָ֔הּ הַדָּגָ֖ן וְהַתִּיר֣וֹשׁ וְהַיִּצְהָ֑ר וְכֶ֨סֶף הִרְבֵּ֥יתִי לָ֛הּ וְזָהָ֖ב עָשׂ֥וּ לַבָּֽעַל׃
  - `WLC (L)`: וְהִיא֙ לֹ֣א יָֽדְעָ֔ה כִּ֤י אָֽנֹכִי֙ נָתַ֣תִּי לָ֔הּ הַדָּגָ֖ן וְהַתִּיר֣וֹשׁ וְהַיִּצְהָ֑ר וְכֶ֨סֶף הִרְבֵּ֥יתִי לָ֛הּ וְזָהָ֖ב עָשׂ֥וּ לַבָּֽעַל׃
  - `BenChayyim (1525)`: וְהִיא֙ לֹ֣א יָֽדְעָ֔ה כִּ֤י אָֽנֹכִי֙ נָתַ֣תִּי לָ֔הּ הַדָּגָ֖ן וְהַתִּיר֣וֹשׁ וְהַיִּצְהָ֑ר וְכֶ֨סֶף הִרְבֵּ֥יתִי לָ֛הּ וְזָהָ֖ב עָשׂ֥וּ לַבָּֽעַל׃
  - `Letteris (1852)`: וְהִיא֙ לֹ֣א יָֽדְעָ֔ה כִּ֤י אָֽנֹכִי֙ נָתַ֣תִּי לָ֔הּ הַדָּגָ֖ן וְהַתִּיר֣וֹשׁ וְהַיִּצְהָ֑ר וְכֶ֨סֶף הִרְבֵּ֥יתִי לָ֛הּ וְזָהָ֖ב עָשׂ֥וּ לַבָּֽעַל׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 1 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 11 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** לָכֵ֣ן אָשׁ֔וּב וְלָקַחְתִּ֤י דְגָנִי֙ בְּעִתּ֔וֹ וְתִירוֹשִׁ֖י בְּמוֹעֲד֑וֹ וְהִצַּלְתִּי֙ צַמְרִ֣י וּפִשְׁתִּ֔י לְכַסּ֖וֹת אֶת־עֶרְוָתָֽהּ׃
  - `MAM (Aleppo)`: לָכֵ֣ן אָשׁ֔וּב וְלָקַחְתִּ֤י דְגָנִי֙ בְּעִתּ֔וֹ וְתִירוֹשִׁ֖י בְּמוֹעֲד֑וֹ וְהִצַּלְתִּי֙ צַמְרִ֣י וּפִשְׁתִּ֔י לְכַסּ֖וֹת אֶת־עֶרְוָתָֽהּ׃
  - `WLC (L)`: לָכֵ֣ן אָשׁ֔וּב וְלָקַחְתִּ֤י דְגָנִי֙ בְּעִתּ֔וֹ וְתִירוֹשִׁ֖י בְּמֽוֹעֲד֑וֹ וְהִצַּלְתִּי֙ צַמְרִ֣י וּפִשְׁתִּ֔י לְכַסּ֖וֹת אֶת־עֶרְוָתָֽהּ׃
  - `BenChayyim (1525)`: לָכֵ֣ן אָשׁ֔וּב וְלָקַחְתִּ֤י דְגָנִי֙ בְּעִתֹּ֔ו וְתִירוֹשִׁ֖י בְּמֽוֹעֲד֑וֹ וְהִצַּלְתִּי֙ צַמְרִ֣י וּפִשְׁתִּ֔י לְכַסֹּ֖ות אֶת־עֶרְוָתָֽהּ׃
  - `Letteris (1852)`: לָכֵ֣ן אָשׁ֔וּב וְלָֽקַחְתִּ֤י דְגָנִי֨ בְּעִתּ֔וֹ וְתִֽירוֹשִׁ֖י בְּמֽוֹעֲד֑וֹ וְהִצַּלְתִּי֙ צַמְרִ֣י וּפִשְׁתִּ֔י לְכַסּ֖וֹת אֶת־עֶרְוָתָֽהּ׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 1 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 12 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וְעַתָּ֛ה אֲגַלֶּ֥ה אֶת־נַבְלֻתָ֖הּ לְעֵינֵ֣י מְאַהֲבֶ֑יהָ וְאִ֖ישׁ לֹא־יַצִּילֶ֥נָּה מִיָּדִֽי׃
  - `MAM (Aleppo)`: וְעַתָּ֛ה אֲגַלֶּ֥ה אֶת־נַבְלֻתָ֖הּ לְעֵינֵ֣י מְאַהֲבֶ֑יהָ וְאִ֖ישׁ לֹא־יַצִּילֶ֥נָּה מִיָּדִֽי׃
  - `WLC (L)`: וְעַתָּ֛ה אֲגַלֶּ֥ה אֶת־נַבְלֻתָ֖הּ לְעֵינֵ֣י מְאַהֲבֶ֑יהָ וְאִ֖ישׁ לֹֽא־יַצִּילֶ֥נָּה מִיָּדִֽי׃
  - `BenChayyim (1525)`: וְעַתָּ֛ה אֲגַלֶּ֥ה אֶת־נַבְלֻתָ֖הּ לְעֵינֵ֣י מְאַהֲבֶ֑יהָ וְאִ֖ישׁ לֹֽא־יַצִּילֶ֥נָּה מִיָּדִֽי׃
  - `Letteris (1852)`: וְעַתָּ֛ה אֲגַלֶּ֥ה אֶת־נַבְלֻתָ֖הּ לְעֵינֵ֣י מְאַֽהֲבֶ֑יהָ וְאִ֖ישׁ לֹֽא־יַצִּילֶ֥נָּה מִיָּדִֽי׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 1 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 13 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וְהִשְׁבַּתִּי֙ כׇּל־מְשׂוֹשָׂ֔הּ חַגָּ֖הּ חׇדְשָׁ֣הּ וְשַׁבַּתָּ֑הּ וְכֹ֖ל מוֹעֲדָֽהּ׃
  - `MAM (Aleppo)`: וְהִשְׁבַּתִּי֙ כׇּל־מְשׂוֹשָׂ֔הּ חַגָּ֖הּ חׇדְשָׁ֣הּ וְשַׁבַּתָּ֑הּ וְכֹ֖ל מוֹעֲדָֽהּ׃
  - `WLC (L)`: וְהִשְׁבַּתִּי֙ כָּל־מְשׂוֹשָׂ֔הּ חַגָּ֖הּ חָדְשָׁ֣הּ וְשַׁבַּתָּ֑הּ וְכֹ֖ל מוֹעֲדָֽהּ׃
  - `BenChayyim (1525)`: וְהִשְׁבַּתִּי֙ כָּל־מְשֹׂושָׂ֔הּ חַגָּ֖הּ חָדְשָׁ֣הּ וְשַׁבַּתָּ֑הּ וְכֹ֖ל מוֹעֲדָֽהּ׃
  - `Letteris (1852)`: וְהִשְׁבַּתִּי֙ כָּל־מְשׂוֹשָׂ֔הּ חַגָּ֖הּ חָדְשָׁ֣הּ וְשַׁבַּתָּ֑הּ וְכֹ֖ל מֽוֹעֲדָֽהּ׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 2 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 14 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וַהֲשִׁמֹּתִ֗י גַּפְנָהּ֙ וּתְאֵ֣נָתָ֔הּ אֲשֶׁ֣ר אָמְרָ֗ה אֶתְנָ֥ה הֵ֙מָּה֙ לִ֔י אֲשֶׁ֥ר נָתְנוּ־לִ֖י מְאַהֲבָ֑י וְשַׂמְתִּ֣ים לְיַ֔עַר וַאֲכָלָ֖תַם חַיַּ֥ת הַשָּׂדֶֽה׃
  - `MAM (Aleppo)`: וַהֲשִׁמֹּתִ֗י גַּפְנָהּ֙ וּתְאֵ֣נָתָ֔הּ אֲשֶׁ֣ר אָמְרָ֗ה אֶתְנָ֥ה הֵ֙מָּה֙ לִ֔י אֲשֶׁ֥ר נָתְנוּ־לִ֖י מְאַהֲבָ֑י וְשַׂמְתִּ֣ים לְיַ֔עַר וַאֲכָלָ֖תַם חַיַּ֥ת הַשָּׂדֶֽה׃
  - `WLC (L)`: וַהֲשִׁמֹּתִ֗י גַּפְנָהּ֙ וּתְאֵ֣נָתָ֔הּ אֲשֶׁ֣ר אָמְרָ֗ה אֶתְנָ֥ה הֵ֙מָּה֙ לִ֔י אֲשֶׁ֥ר נָֽתְנוּ־לִ֖י מְאַֽהֲבָ֑י וְשַׂמְתִּ֣ים לְיַ֔עַר וַאֲכָלָ֖תַם חַיַּ֥ת הַשָּׂדֶֽה׃
  - `BenChayyim (1525)`: וַהֲשִׁמֹּתִ֗י גַּפְנָהּ֙ וּתְאֵ֣נָתָ֔הּ אֲשֶׁ֣ר אָמְרָ֗ה אֶתְנָ֥ה הֵ֙מָּה֙ לִ֔י אֲשֶׁ֥ר נָֽתְנוּ־לִ֖י מְאַֽהֲבָ֑י וְשַׂמְתִּ֣ים לְיַ֔עַר וַאֲכָלָ֖תַם חַיַּ֥ת הַשָּׂדֶֽה׃
  - `Letteris (1852)`: וַֽהֲשִׁמֹּתִ֤י גַּפְנָהּ֨ וּתְאֵ֣נָתָ֔הּ אֲשֶׁ֣ר אָֽמְרָ֗ה אֶתְנָ֥ה הֵ֨מָּה֙ לִ֔י אֲשֶׁ֥ר נָֽתְנוּ־לִ֖י מְאַֽהֲבָ֑י וְשַׂמְתִּ֣ים לְיַ֔עַר וַֽאֲכָלָ֖תַם חַיַּ֥ת הַשָּׂדֶֽה׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 2 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 15 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וּפָקַדְתִּ֣י עָלֶ֗יהָ אֶת־יְמֵ֤י הַבְּעָלִים֙ אֲשֶׁ֣ר תַּקְטִ֣יר לָהֶ֔ם וַתַּ֤עַד נִזְמָהּ֙ וְחֶלְיָתָ֔הּ וַתֵּ֖לֶךְ אַחֲרֵ֣י מְאַהֲבֶ֑יהָ וְאֹתִ֥י שָׁכְחָ֖ה נְאֻם־יְהֹוָֽה׃
  - `MAM (Aleppo)`: וּפָקַדְתִּ֣י עָלֶ֗יהָ אֶת־יְמֵ֤י הַבְּעָלִים֙ אֲשֶׁ֣ר תַּקְטִ֣יר לָהֶ֔ם וַתַּ֤עַד נִזְמָהּ֙ וְחֶלְיָתָ֔הּ וַתֵּ֖לֶךְ אַחֲרֵ֣י מְאַהֲבֶ֑יהָ וְאֹתִ֥י שָׁכְחָ֖ה נְאֻם־יְהֹוָֽה׃
  - `WLC (L)`: וּפָקַדְתִּ֣י עָלֶ֗יהָ אֶת־יְמֵ֤י הַבְּעָלִים֙ אֲשֶׁ֣ר תַּקְטִ֣יר לָהֶ֔ם וַתַּ֤עַד נִזְמָהּ֙ וְחֶלְיָתָ֔הּ וַתֵּ֖לֶךְ אַחֲרֵ֣י מְאַהֲבֶ֑יהָ וְאֹתִ֥י שָׁכְחָ֖ה נְאֻם־יְהוָֽה׃
  - `BenChayyim (1525)`: וּפָקַדְתִּ֣י עָלֶ֗יהָ אֶת־יְמֵ֤י הַבְּעָלִים֙ אֲשֶׁ֣ר תַּקְטִ֣יר לָהֶ֔ם וַתַּ֤עַד נִזְמָהּ֙ וְחֶלְיָתָ֔הּ וַתֵּ֖לֶךְ אַחֲרֵ֣י מְאַהֲבֶ֑יהָ וְאֹתִ֥י שָׁכְחָ֖ה נְאֻם־יְהוָֽה׃
  - `Letteris (1852)`: וּפָֽקַדְתִּ֣י עָלֶ֔יהָ אֶת־יְמֵ֤י הַבְּעָלִים֨ אֲשֶׁ֣ר תַּקְטִ֣יר לָהֶ֔ם וַתַּ֤עַד נִזְמָהּ֙ וְחֶלְיָתָ֔הּ וַתֵּ֖לֶךְ אַֽחֲרֵ֣י מְאַֽהֲבֶ֑יהָ וְאֹתִ֥י שָֽׁכְחָ֖ה נְאֻם־יְהֹוָֽה׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 1 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 16 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** לָכֵ֗ן הִנֵּ֤ה אָנֹכִי֙ מְפַתֶּ֔יהָ וְהֹלַכְתִּ֖יהָ הַמִּדְבָּ֑ר וְדִבַּרְתִּ֖י עַל־לִבָּֽהּ׃
  - `MAM (Aleppo)`: לָכֵ֗ן הִנֵּ֤ה אָנֹכִי֙ מְפַתֶּ֔יהָ וְהֹלַכְתִּ֖יהָ הַמִּדְבָּ֑ר וְדִבַּרְתִּ֖י עַל־לִבָּֽהּ׃
  - `WLC (L)`: לָכֵ֗ן הִנֵּ֤ה אָֽנֹכִי֙ מְפַתֶּ֔יהָ וְהֹֽלַכְתִּ֖יהָ הַמִּדְבָּ֑ר וְדִבַּרְתִּ֖י עַל לִבָּֽהּ׃
  - `BenChayyim (1525)`: לָכֵ֗ן הִנֵּ֤ה אָֽנֹכִי֙ מְפַתֶּ֔יהָ וְהֹֽלַכְתִּ֖יהָ הַמִּדְבָּ֑ר וְדִבַּרְתִּ֖י עַל־לִבָּֽהּ׃
  - `Letteris (1852)`: לָכֵ֗ן הִנֵּ֤ה אָֽנֹכִי֨ מְפַתֶּ֔יהָ וְהֹֽלַכְתִּ֖יהָ הַמִּדְבָּ֑ר וְדִבַּרְתִּ֖י עַל־לִבָּֽהּ׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 3 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention; Punctuation / spacing difference only).

### Verse 17 (Confidence: `50.6%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וְנָתַ֨תִּי לָ֤הּ אֶת־כְּרָמֶ֙יהָ֙ מִשָּׁ֔ם וְאֶת־עֵ֥מֶק עָכ֖וֹר לְפֶ֣תַח תִּקְוָ֑ה וְעָ֤נְתָה שָּׁ֙מָּה֙ כִּימֵ֣י נְעוּרֶ֔יהָ וּכְי֖וֹם עֲלוֹתָ֥הּ מֵאֶרֶץ־מִצְרָֽיִם׃
  - `MAM (Aleppo)`: וְנָתַ֨תִּי לָ֤הּ אֶת־כְּרָמֶ֙יהָ֙ מִשָּׁ֔ם וְאֶת־עֵ֥מֶק עָכ֖וֹר לְפֶ֣תַח תִּקְוָ֑ה וְעָ֤נְתָה שָּׁ֙מָּה֙ כִּימֵ֣י נְעוּרֶ֔יהָ וּכְי֖וֹם עֲלוֹתָ֥הּ מֵאֶרֶץ־מִצְרָֽיִם׃
  - `WLC (L)`: וְנָתַ֨תִּי לָ֤הּ אֶת־כְּרָמֶ֙יהָ֙ מִשָּׁ֔ם וְאֶת־עֵ֥מֶק עָכ֖וֹר לְפֶ֣תַח תִּקְוָ֑ה וְעָ֤נְתָה שָּׁ֙מָּה֙ כִּימֵ֣י נְעוּרֶ֔יהָ וִּכְי֖וֹם עֲלֹתָ֥הּ מֵאֶֽרֶץ־מִצְרָֽיִם׃
  - `BenChayyim (1525)`: וְנָתַ֨תִּי לָ֤הּ אֶת־כְּרָמֶ֙יהָ֙ מִשָּׁ֔ם וְאֶת־עֵ֥מֶק עָכ֖וֹר לְפֶ֣תַח תִּקְוָ֑ה וְעָ֤נְתָה שָּׁ֙מָּה֙ כִּימֵ֣י נְעוּרֶ֔יהָ וִּכְי֖וֹם עֲלֹתָ֥הּ מֵאֶֽרֶץ־מִצְרָֽיִם׃
  - `Letteris (1852)`: וְנָֽתַ֨תִּי לָ֤הּ אֶת־כְּרָמֶ֨יהָ֨ מִשָּׁ֔ם וְאֶת־עֵ֥מֶק עָכ֖וֹר לְפֶ֣תַח תִּקְוָ֑ה וְעָ֤נְתָה שָּׁ֨מָּה֙ כִּימֵ֣י נְעוּרֶ֔יהָ וּכְי֖וֹם עֲלוֹתָ֥הּ מֵאֶֽרֶץ־מִצְרָֽיִם׃
- **Philological Rationale:** [Vocalisation / pointing difference (same consonantal text)] Adopted 'וּכְי֖וֹם' [MAM (Aleppo)] (weight 0.98, confidence 51%) over וִּכְי֖וֹם (WLC (L)). Also normalised 2 orthographic/surface variation(s).
- *confidence:* Verse confidence 51% = product of 1 unit confidence(s); not calibrated for this corpus (same formula as the Greek NT; read it as a relative measure). 1 unit(s) are one witness against one, where any choice is weakly supported.

### Verse 18 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וְהָיָ֤ה בַיּוֹם־הַהוּא֙ נְאֻם־יְהֹוָ֔ה תִּקְרְאִ֖י אִישִׁ֑י וְלֹא־תִקְרְאִי־לִ֥י ע֖וֹד בַּעְלִֽי׃
  - `MAM (Aleppo)`: וְהָיָ֤ה בַיּוֹם־הַהוּא֙ נְאֻם־יְהֹוָ֔ה תִּקְרְאִ֖י אִישִׁ֑י וְלֹא־תִקְרְאִי־לִ֥י ע֖וֹד בַּעְלִֽי׃
  - `WLC (L)`: וְהָיָ֤ה בַיּוֹם־הַהוּא֙ נְאֻם־יְהוָ֔ה תִּקְרְאִ֖י אִישִׁ֑י וְלֹֽא־תִקְרְאִי־לִ֥י ע֖וֹד בַּעְלִֽי׃
  - `BenChayyim (1525)`: וְהָיָ֤ה בַיֹּום־הַהוּא֙ נְאֻם־יְהוָ֔ה תִּקְרְאִ֖י אִישִׁ֑י וְלֹֽא־תִקְרְאִי־לִ֥י ע֖וֹד בַּעְלִֽי׃
  - `Letteris (1852)`: וְהָיָ֤ה בַיּֽוֹם־הַהוּא֨ נְאֻם־יְהֹוָ֔ה תִּקְרְאִ֖י אִישִׁ֑י וְלֹֽא־תִקְרְאִי־לִ֛י ע֖וֹד בַּעְלִֽי׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 2 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 19 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וַהֲסִרֹתִ֛י אֶת־שְׁמ֥וֹת הַבְּעָלִ֖ים מִפִּ֑יהָ וְלֹא־יִזָּכְר֥וּ ע֖וֹד בִּשְׁמָֽם׃
  - `MAM (Aleppo)`: וַהֲסִרֹתִ֛י אֶת־שְׁמ֥וֹת הַבְּעָלִ֖ים מִפִּ֑יהָ וְלֹא־יִזָּכְר֥וּ ע֖וֹד בִּשְׁמָֽם׃
  - `WLC (L)`: וַהֲסִרֹתִ֛י אֶת־שְׁמ֥וֹת הַבְּעָלִ֖ים מִפִּ֑יהָ וְלֹֽא־יִזָּכְר֥וּ ע֖וֹד בִּשְׁמָֽם׃
  - `BenChayyim (1525)`: וַהֲסִרֹתִ֛י אֶת־שְׁמ֥וֹת הַבְּעָלִ֖ים מִפִּ֑יהָ וְלֹֽא־יִזָּכְר֥וּ ע֖וֹד בִּשְׁמָֽם׃
  - `Letteris (1852)`: וַֽהֲסִרֹתִ֛י אֶת־שְׁמ֥וֹת הַבְּעָלִ֖ים מִפִּ֑יהָ וְלֹֽא־יִזָּֽכְר֥וּ ע֖וֹד בִּשְׁמָֽם׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 1 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 20 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וְכָרַתִּ֨י לָהֶ֤ם בְּרִית֙ בַּיּ֣וֹם הַה֔וּא עִם־חַיַּ֤ת הַשָּׂדֶה֙ וְעִם־ע֣וֹף הַשָּׁמַ֔יִם וְרֶ֖מֶשׂ הָאֲדָמָ֑ה וְקֶ֨שֶׁת וְחֶ֤רֶב וּמִלְחָמָה֙ אֶשְׁבּ֣וֹר מִן־הָאָ֔רֶץ וְהִשְׁכַּבְתִּ֖ים לָבֶֽטַח׃
  - `MAM (Aleppo)`: וְכָרַתִּ֨י לָהֶ֤ם בְּרִית֙ בַּיּ֣וֹם הַה֔וּא עִם־חַיַּ֤ת הַשָּׂדֶה֙ וְעִם־ע֣וֹף הַשָּׁמַ֔יִם וְרֶ֖מֶשׂ הָאֲדָמָ֑ה וְקֶ֨שֶׁת וְחֶ֤רֶב וּמִלְחָמָה֙ אֶשְׁבּ֣וֹר מִן־הָאָ֔רֶץ וְהִשְׁכַּבְתִּ֖ים לָבֶֽטַח׃
  - `WLC (L)`: וְכָרַתִּ֨י לָהֶ֤ם בְּרִית֙ בַּיּ֣וֹם הַה֔וּא עִם־חַיַּ֤ת הַשָּׂדֶה֙ וְעִם־ע֣וֹף הַשָּׁמַ֔יִם וְרֶ֖מֶשׂ הָֽאֲדָמָ֑ה וְקֶ֨שֶׁת וְחֶ֤רֶב וּמִלְחָמָה֙ אֶשְׁבּ֣וֹר מִן־הָאָ֔רֶץ וְהִשְׁכַּבְתִּ֖ים לָבֶֽטַח׃
  - `BenChayyim (1525)`: וְכָרַתִּ֨י לָהֶ֤ם בְּרִית֙ בַּיֹּ֣ום הַה֔וּא עִם־חַיַּ֤ת הַשָּׂדֶה֙ וְעִם־ע֣וֹף הַשָּׁמַ֔יִם וְרֶ֖מֶשׂ הָֽאֲדָמָ֑ה וְקֶ֨שֶׁת וְחֶ֤רֶב וּמִלְחָמָה֙ אֶשְׁבֹּ֣ור מִן־הָאָ֔רֶץ וְהִשְׁכַּבְתִּ֖ים לָבֶֽטַח׃
  - `Letteris (1852)`: וְכָֽרַתִּ֨י לָהֶ֤ם בְּרִית֨ בַּיּ֣וֹם הַה֔וּא עִם־חַיַּ֤ת הַשָּׂדֶה֙ וְעִם־ע֣וֹף הַשָּׁמַ֔יִם וְרֶ֖מֶשׂ הָֽאֲדָמָ֑ה וְקֶ֨שֶׁת וְחֶ֤רֶב וּמִלְחָמָה֨ אֶשְׁבּ֣וֹר מִן־הָאָ֔רֶץ וְהִשְׁכַּבְתִּ֖ים לָבֶֽטַח׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 1 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 21 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וְאֵרַשְׂתִּ֥יךְ לִ֖י לְעוֹלָ֑ם וְאֵרַשְׂתִּ֥יךְ לִי֙ בְּצֶ֣דֶק וּבְמִשְׁפָּ֔ט וּבְחֶ֖סֶד וּֽבְרַחֲמִֽים׃
  - `MAM (Aleppo)`: וְאֵרַשְׂתִּ֥יךְ לִ֖י לְעוֹלָ֑ם וְאֵרַשְׂתִּ֥יךְ לִי֙ בְּצֶ֣דֶק וּבְמִשְׁפָּ֔ט וּבְחֶ֖סֶד וּֽבְרַחֲמִֽים׃
  - `WLC (L)`: וְאֵרַשְׂתִּ֥יךְ לִ֖י לְעוֹלָ֑ם וְאֵרַשְׂתִּ֥יךְ לִי֙ בְּצֶ֣דֶק וּבְמִשְׁפָּ֔ט וּבְחֶ֖סֶד וּֽבְרַחֲמִֽים׃
  - `BenChayyim (1525)`: וְאֵרַשְׂתִּ֥יךְ לִ֖י לְעוֹלָ֑ם וְאֵרַשְׂתִּ֥יךְ לִי֙ בְּצֶ֣דֶק וּבְמִשְׁפָּ֔ט וּבְחֶ֖סֶד וּֽבְרַחֲמִֽים׃
  - `Letteris (1852)`: וְאֵרַשְׂתִּ֥יךְ לִ֖י לְעוֹלָ֑ם וְאֵֽרַשְׂתִּ֥יךְ לִי֙ בְּצֶ֣דֶק וּבְמִשְׁפָּ֔ט וּבְחֶ֖סֶד וּבְרַֽחֲמִֽים׃
- **Philological Rationale:** Unanimous witness agreement across MAM (Aleppo), WLC (L) (2 admitted witnesses; zero substantive divergence).

### Verse 22 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וְאֵרַשְׂתִּ֥יךְ לִ֖י בֶּאֱמוּנָ֑ה וְיָדַ֖עַתְּ אֶת־יְהֹוָֽה׃
  - `MAM (Aleppo)`: וְאֵרַשְׂתִּ֥יךְ לִ֖י בֶּאֱמוּנָ֑ה וְיָדַ֖עַתְּ אֶת־יְהֹוָֽה׃
  - `WLC (L)`: וְאֵרַשְׂתִּ֥יךְ לִ֖י בֶּאֱמוּנָ֑ה וְיָדַ֖עַתְּ אֶת־יְהוָֽה׃
  - `BenChayyim (1525)`: וְאֵרַשְׂתִּ֥יךְ לִ֖י בֶּאֱמוּנָ֑ה וְיָדַ֖עַתְּ אֶת־יְהוָֽה׃
  - `Letteris (1852)`: וְאֵֽרַשְׂתִּ֥יךְ לִ֖י בֶּֽאֱמוּנָ֑ה וְיָדַ֖עַתְּ אֶת־יְהֹוָֽה׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 1 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 23 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וְהָיָ֣ה ׀ בַּיּ֣וֹם הַה֗וּא אֶֽעֱנֶה֙ נְאֻם־יְהֹוָ֔ה אֶעֱנֶ֖ה אֶת־הַשָּׁמָ֑יִם וְהֵ֖ם יַעֲנ֥וּ אֶת־הָאָֽרֶץ׃
  - `MAM (Aleppo)`: וְהָיָ֣ה ׀ בַּיּ֣וֹם הַה֗וּא אֶֽעֱנֶה֙ נְאֻם־יְהֹוָ֔ה אֶעֱנֶ֖ה אֶת־הַשָּׁמָ֑יִם וְהֵ֖ם יַעֲנ֥וּ אֶת־הָאָֽרֶץ׃
  - `WLC (L)`: וְהָיָ֣ה ׀ בַּיּ֣וֹם הַה֗וּא אֶֽעֱנֶה֙ נְאֻם־יְהוָ֔ה אֶעֱנֶ֖ה אֶת־הַשָּׁמָ֑יִם וְהֵ֖ם יַעֲנ֥וּ אֶת־הָאָֽרֶץ׃
  - `BenChayyim (1525)`: וְהָיָ֣ה ׀ בַּיֹּ֣ום הַה֗וּא אֶֽעֱנֶה֙ נְאֻם־יְהוָ֔ה אֶעֱנֶ֖ה אֶת־הַשָּׁמָ֑יִם וְהֵ֖ם יַעֲנ֥וּ אֶת־הָאָֽרֶץ׃
  - `Letteris (1852)`: וְהָיָ֣ה ׀ בַּיּ֣וֹם הַה֗וּא אֶֽעֱנֶה֨ נְאֻם־יְהֹוָ֔ה אֶֽעֱנֶ֖ה אֶת־הַשָּׁמָ֑יִם וְהֵ֖ם יַֽעֲנ֥וּ אֶת־הָאָֽרֶץ׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 1 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).

### Verse 24 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וְהָאָ֣רֶץ תַּעֲנֶ֔ה אֶת־הַדָּגָ֖ן וְאֶת־הַתִּיר֣וֹשׁ וְאֶת־הַיִּצְהָ֑ר וְהֵ֖ם יַעֲנ֥וּ אֶֽת־יִזְרְעֶֽאל׃
  - `MAM (Aleppo)`: וְהָאָ֣רֶץ תַּעֲנֶ֔ה אֶת־הַדָּגָ֖ן וְאֶת־הַתִּיר֣וֹשׁ וְאֶת־הַיִּצְהָ֑ר וְהֵ֖ם יַעֲנ֥וּ אֶֽת־יִזְרְעֶֽאל׃
  - `WLC (L)`: וְהָאָ֣רֶץ תַּעֲנֶ֔ה אֶת־הַדָּגָ֖ן וְאֶת־הַתִּיר֣וֹשׁ וְאֶת־הַיִּצְהָ֑ר וְהֵ֖ם יַעֲנ֥וּ אֶֽת־יִזְרְעֶֽאל׃
  - `BenChayyim (1525)`: וְהָאָ֣רֶץ תַּעֲנֶ֔ה אֶת־הַדָּגָ֖ן וְאֶת־הַתִּיר֣וֹשׁ וְאֶת־הַיִּצְהָ֑ר וְהֵ֖ם יַעֲנ֥וּ אֶֽת־יִזְרְעֶֽאל׃
  - `Letteris (1852)`: וְהָאָ֣רֶץ תַּֽעֲנֶ֔ה אֶת־הַדָּגָ֖ן וְאֶת־הַתִּיר֣וֹשׁ וְאֶת־הַיִּצְהָ֑ר וְהֵ֖ם יַֽעֲנ֥וּ אֶֽת־יִזְרְעֶֽאל׃
- **Philological Rationale:** Unanimous witness agreement across MAM (Aleppo), WLC (L) (2 admitted witnesses; zero substantive divergence).

### Verse 25 (Confidence: `99.0%` · Source: `Textual Analysis Brain (Claude-designed · internal evidence · offline)`)
- **Critical Text:** וּזְרַעְתִּ֤יהָ לִּי֙ בָּאָ֔רֶץ וְרִחַמְתִּ֖י אֶת־לֹ֣א רֻחָ֑מָה וְאָמַרְתִּ֤י לְלֹֽא־עַמִּי֙ עַמִּי־אַ֔תָּה וְה֖וּא יֹאמַ֥ר אֱלֹהָֽי׃
  - `MAM (Aleppo)`: וּזְרַעְתִּ֤יהָ לִּי֙ בָּאָ֔רֶץ וְרִחַמְתִּ֖י אֶת־לֹ֣א רֻחָ֑מָה וְאָמַרְתִּ֤י לְלֹֽא־עַמִּי֙ עַמִּי־אַ֔תָּה וְה֖וּא יֹאמַ֥ר אֱלֹהָֽי׃
  - `WLC (L)`: וּזְרַעְתִּ֤יהָ לִּי֙ בָּאָ֔רֶץ וְרִֽחַמְתִּ֖י אֶת־לֹ֣א רֻחָ֑מָה וְאָמַרְתִּ֤י לְלֹֽא־עַמִּי֙ עַמִּי־אַ֔תָּה וְה֖וּא יֹאמַ֥ר אֱלֹהָֽי׃
  - `BenChayyim (1525)`: וּזְרַעְתִּ֤יהָ לִּי֙ בָּאָ֔רֶץ וְרִֽחַמְתִּ֖י אֶת־לֹ֣א רֻחָ֑מָה וְאָמַרְתִּ֤י לְלֹֽא־עַמִּי֙ עַמִּי־אַ֔תָּה וְה֖וּא יֹאמַ֥ר אֱלֹהָֽי׃
  - `Letteris (1852)`: וּזְרַעְתִּ֤יהָ לִּי֙ בָּאָ֔רֶץ וְרִֽחַמְתִּ֖י אֶת־לֹ֣א רֻחָ֑מָה וְאָֽמַרְתִּ֤י לְלֹֽא־עַמִּי֨ עַמִּי־אַ֔תָּה וְה֖וּא יֹאמַ֥ר אֱלֹהָֽי׃
- **Philological Rationale:** Substantively unanimous across MAM (Aleppo), WLC (L). Normalised 1 surface variation(s) (Masoretic cantillation / meteg / qamats-qatan / divine-name pointing convention).
