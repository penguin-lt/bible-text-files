# Verification report

- files: **133** (87 translations, 21 critical editions, 25 lexicons/reference works)
- verse/entry rows total: **2,294,684**
- files with ERRORS: **0** | files with warnings: 2

Checks run on every file:

1. SQLite source: `PRAGMA integrity_check`, FTS row count == verse/entry count, no empty texts.
2. The written .txt is re-parsed line-by-line and compared row-for-row against the SQLite source (book, chapter, verse, text) — any mismatch is an error.
3. Leftover USFM/XML markup scan (`\marker`, `<tag>`, `strong=`): occurrences are preserved verbatim (the SQLite text is the source of truth) and reported as warnings.
4. One record per line: embedded newlines in source texts are flattened to spaces.

| file | rows | errors | warnings |
|---|---|---|---|
| translations/2001 Translation of the Holy Bible (2001) [T2001].txt | 33,328 | OK | - |
| translations/A Conservative Version [ACV].txt | 31,102 | OK | - |
| translations/American Bible Union New Testament [ABU1865].txt | 7,953 | OK | - |
| translations/American King James Version [AKJV].txt | 31,102 | OK | - |
| translations/American Standard Version Byzantine Text [ASVBT].txt | 37,761 | OK | - |
| translations/American Standard Version [ASV].txt | 31,086 | OK | - |
| translations/Anderson's New Testament [Anderson].txt | 7,946 | OK | - |
| translations/Berean Literal Bible [BLB].txt | 7,941 | OK | - |
| translations/Berean Standard Bible [BSB].txt | 31,086 | OK | - |
| translations/Bible in Basic English [BBE].txt | 31,102 | OK | - |
| translations/Bishops' Bible [BISHOPS].txt | 31,102 | OK | - |
| translations/Brenton Septuagint Translation [Brenton].txt | 28,690 | OK | - |
| translations/Catholic Public Domain Version [CPDV].txt | 35,812 | OK | - |
| translations/Charles Thomson Septuagint (transcribed books) [THOMSON].txt | 3,599 | OK | - |
| translations/Coverdale Bible [Coverdale].txt | 31,089 | OK | - |
| translations/Darby Translation [DBY].txt | 31,099 | OK | - |
| translations/Douay-Rheims Bible (American Edition) [DRA].txt | 35,811 | OK | - |
| translations/Easy to Translate English Jonah [E2T].txt | 47 | OK | - |
| translations/Etheridge's Peshitta New Testament [Etheridge].txt | 7,940 | OK | - |
| translations/Family 35 New Testament (Wilbur Pickering) [F35].txt | 7,953 | OK | - |
| translations/Free Bible Version [FBV].txt | 31,087 | OK | - |
| translations/Garth's Hyper-literal Translation [GHT].txt | 7,956 | OK | - |
| translations/Geneva Bible (1560) [GNV1560].txt | 31,102 | OK | - |
| translations/Geneva Bible (1599) [GNV1599].txt | 31,090 | OK | - |
| translations/Godbey New Testament [Godbey].txt | 7,913 | OK | - |
| translations/Great Bible [GREAT].txt | 31,095 | OK | - |
| translations/Haweis New Testament [HAWEIS].txt | 7,957 | OK | - |
| translations/JPS TaNaKH (Jewish Publication Society) [JPS1917].txt | 23,145 | OK | - |
| translations/Joseph Smith Translation (Inspired Version) [JST].txt | 30,829 | OK | - |
| translations/King James Bible (1611 First Edition) [KJV1611].txt | 31,102 | OK | - |
| translations/King James Version with Apocrypha [KJVA].txt | 36,822 | OK | - |
| translations/King James Version, Cambridge Paragraph Bible [engkjvcpb].txt | 36,822 | OK | - |
| translations/LXX2012 - Septuagint in American English [LXX2012].txt | 28,324 | OK | - |
| translations/Leeser Tanakh [Leeser].txt | 23,143 | OK | - |
| translations/Literal Standard Version [LSV].txt | 31,104 | OK | - |
| translations/Mace New Testament [MACE].txt | 7,957 | OK | - |
| translations/Majority Standard Bible [MSB].txt | 31,098 | OK | - |
| translations/Matthew Bible [Matthew].txt | 31,092 | OK | - |
| translations/Moffatt New Testament [MOFFATT].txt | 7,940 | OK | - |
| translations/Montgomery New Testament (Centenary Translation) [MONTGOMERY].txt | 7,927 | OK | - |
| translations/Murdock's Peshitta New Testament [Murdock].txt | 7,947 | OK | - |
| translations/New Heart English Bible [NHEB].txt | 31,097 | OK | - |
| translations/Noyes Bible [Noyes].txt | 18,213 | OK | - |
| translations/One Unity Resource Bible [OURB].txt | 15,230 | OK | - |
| translations/Open English Bible (US Spelling) [OEBUS].txt | 13,894 | OK | - |
| translations/Open Source English Bible [OSEN].txt | 31,167 | OK | 18 verses contain markup-like characters (preserved verbatim from source) |
| translations/Open Translation Bible (British English) [OTB].txt | 31,103 | OK | - |
| translations/Orthodox Jewish Bible [OJB].txt | 31,165 | OK | - |
| translations/Ottley Isaiah (from the Septuagint) [OTTLEY].txt | 1,286 | OK | - |
| translations/Panin Numeric New Testament [PANIN].txt | 7,937 | OK | - |
| translations/Plain English Version [PEV].txt | 7,374 | OK | - |
| translations/Restored Name King James Version [RNKJV].txt | 31,102 | OK | - |
| translations/Revised King James New Testament [RKJNT].txt | 7,956 | OK | - |
| translations/Revised Version with Apocrypha [RV1895].txt | 36,836 | OK | - |
| translations/Riverside New Testament [RIVERSIDE].txt | 7,932 | OK | - |
| translations/Rotherham's Emphasised Bible [Rotherham].txt | 31,086 | OK | - |
| translations/Sawyer New Testament (chronological) [SAWYER].txt | 7,957 | OK | 2 verses contain markup-like characters (preserved verbatim from source) |
| translations/Smith's Literal Translation (Julia E. Smith Parker) [SLT].txt | 31,102 | OK | - |
| translations/Targum Onkelos Etheridge (English) [OnkelosETHERIDGE].txt | 5,848 | OK | - |
| translations/Tegid Isaiah (John Jones, from the Hebrew) [TEG].txt | 1,292 | OK | - |
| translations/Text-Critical English New Testament [TCENT].txt | 7,954 | OK | - |
| translations/The Emphatic Diaglott (Benjamin Wilson Emphatic Version) [DIAGLOTT].txt | 7,910 | OK | - |
| translations/The Living Oracles [LIVINGORACLES].txt | 7,955 | OK | - |
| translations/Translation for Translators [T4T].txt | 30,640 | OK | - |
| translations/Twentieth Century New Testament [TCNT].txt | 7,940 | OK | - |
| translations/Tyndale New Testament (eBible.org edition) [TNT].txt | 7,954 | OK | - |
| translations/Updated Brenton English Septuagint [LXXUP].txt | 28,349 | OK | - |
| translations/Updated King James Version [UKJV].txt | 31,102 | OK | - |
| translations/Webster Bible [Webster].txt | 31,102 | OK | - |
| translations/Wesley New Testament [Wesley].txt | 7,957 | OK | - |
| translations/Weymouth New Testament [Weymouth].txt | 7,957 | OK | - |
| translations/Whiston Primitive New Testament [WHISTON].txt | 7,957 | OK | - |
| translations/William Tyndale Bible (surviving corpus) [Tyndale].txt | 13,852 | OK | - |
| translations/World English Bible Classic [WEB].txt | 38,029 | OK | - |
| translations/World English Bible Updated [engwebu].txt | 38,029 | OK | - |
| translations/World English Bible, Catholic Edition [engwebc].txt | 35,379 | OK | - |
| translations/World Messianic Bible [WMB].txt | 31,098 | OK | - |
| translations/Worrell New Testament [Worrell].txt | 7,946 | OK | - |
| translations/Worsley New Testament [Worsley].txt | 7,958 | OK | - |
| translations/Wycliffe Bible (Later Version, c. 1395) [WYCLIFFE].txt | 36,227 | OK | - |
| translations/Wycliffe Bible with Modern Spelling [WYCMS].txt | 35,996 | OK | - |
| translations/Young's Literal Translation [YLT].txt | 31,102 | OK | - |
| translations/unfoldingWord Literal Text [ULT].txt | 31,103 | OK | - |
| translations/unfoldingWord Simplified Text [UST].txt | 30,975 | OK | - |
| critical-editions/Brenton's Greek Text of the Septuagint [grcbrent].txt | 28,597 | OK | - |
| critical-editions/Church Slavonic Elizabeth Bible 1757, New Testament [chuEliz].txt | 7,939 | OK | - |
| critical-editions/Coptic New Testament (Bohairic, narrative form) [copcnt].txt | 7,957 | OK | - |
| critical-editions/Coptic New Testament, Bohairic [copbhc].txt | 7,956 | OK | - |
| critical-editions/Greek New Testament, Majority Text (Robinson-Pierpont) [grcmt].txt | 7,953 | OK | - |
| critical-editions/Greek Textus Receptus (Stephanus, Elzevir, Scrivener) [grctr].txt | 7,957 | OK | - |
| critical-editions/Hebrew Bible (Letteris, 1866) [hbolet].txt | 23,208 | OK | - |
| critical-editions/Hebrew Masoretic Text (Westminster Leningrad Codex) [hbo].txt | 23,213 | OK | - |
| critical-editions/Nestle Greek New Testament (1904) [grcnestle].txt | 7,943 | OK | - |
| critical-editions/Patriarchal Greek New Testament (1904, Antoniades) [grcbyz].txt | 7,958 | OK | - |
| critical-editions/Sahidic Coptic New Testament (Horner, 1911) [copsahh].txt | 7,936 | OK | - |
| critical-editions/Septuagint (Greek Old Testament) [grclxx].txt | 27,871 | OK | - |
| critical-editions/Solid Rock Greek New Testament (Scholar's Edition) [grcsr].txt | 7,961 | OK | - |
| critical-editions/Syriac Peshitta New Testament (BFBS 1905) [syrpesh].txt | 7,943 | OK | - |
| critical-editions/Text-Critical Greek New Testament [grctcgnt].txt | 7,954 | OK | - |
| critical-editions/Tischendorf Greek New Testament (8th edition) [grc-tisch].txt | 7,939 | OK | - |
| critical-editions/Tregelles Greek New Testament 1864 [grctreg].txt | 7,947 | OK | - |
| critical-editions/Vulgate (Clementine, 1598) [latVUC].txt | 35,809 | OK | - |
| critical-editions/Vulgate, Sixtine Edition 1590, New Testament [latVulSist].txt | 7,941 | OK | - |
| critical-editions/Westcott and Hort Greek New Testament (1881) [grcwh].txt | 7,941 | OK | - |
| critical-editions/Westminster Leningrad Codex with Strong's and morphology [hboWLC].txt | 23,213 | OK | - |
| lexicons/A Dictionary of Christian Biography and Literature to the End of the Sixth Century A.D., with an Account of the Principal Sects and Heresies.txt | 4 | OK | - |
| lexicons/American Tract Society Bible Dictionary.txt | 2,286 | OK | - |
| lexicons/An Intermediate GreekΓÇôEnglish Lexicon Keyed to Strong's Numbers.txt | 4,105 | OK | - |
| lexicons/BDB Glosses (Strong's).txt | 8,674 | OK | - |
| lexicons/Brown-Driver-Briggs Hebrew and English Lexicon (full).txt | 11,769 | OK | - |
| lexicons/C. H. Spurgeon's Morning and Evening - Daily Readings.txt | 366 | OK | - |
| lexicons/Codes dΓÇÖanalyse morphologique de Packard.txt | 3,072 | OK | - |
| lexicons/Codes dΓÇÖanalyse morphologique de Robinson.txt | 1,591 | OK | - |
| lexicons/Condensed Biblical Cyclopedia.txt | 57 | OK | - |
| lexicons/Dodson Greek-English Lexicon.txt | 5,408 | OK | - |
| lexicons/Easton's Bible Dictionary.txt | 3,963 | OK | - |
| lexicons/G. Abbott-Smith's A Manual Greek Lexicon (with Strongs) of the New Testament.txt | 11,394 | OK | - |
| lexicons/International Standard Bible Encyclopedia.txt | 9,349 | OK | - |
| lexicons/Klingon Language Version English to Klingon mapping lexicon.txt | 1,019 | OK | - |
| lexicons/Klingon Language Version Klingon to English mapping lexicon.txt | 808 | OK | - |
| lexicons/Liddell-Scott-Jones Greek-English Lexicon (full, biblical vocabulary).txt | 5,706 | OK | - |
| lexicons/Open Scriptures Hebrew Morphology.txt | 3,481 | OK | - |
| lexicons/Ordf├╢rklaringar och sakupplysningar.txt | 330 | OK | - |
| lexicons/Packard's Morphological Analysis Codes.txt | 3,072 | OK | - |
| lexicons/Robinson's Morphological Analysis Codes.txt | 1,591 | OK | - |
| lexicons/Smith's Bible Dictionary.txt | 4,637 | OK | - |
| lexicons/Strong's Greek Bible Dictionary.txt | 5,742 | OK | - |
| lexicons/Strong's Hebrew Bible Dictionary.txt | 8,675 | OK | - |
| lexicons/Translators Brief lexicon of Extended Strong's ΓÇö Greek.txt | 11,032 | OK | - |
| lexicons/Translators Brief lexicon of Extended Strong's ΓÇö Hebrew.txt | 11,682 | OK | - |
| translations/Open English Translation, Readers' Version [engOETrv].txt | 36,005 | OK | - |
| translations/Open English Translation, Literal Version [engOETlv].txt | 7,914 | OK | - |
| translations/Unlocked Dynamic Bible [engudb].txt | 30,767 | OK | - |
