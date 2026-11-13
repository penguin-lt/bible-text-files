# Verification report

- files: **1167** (137 translations, 22 critical editions, 25 lexicons/reference works, 3 Greek NT editions, 978 Greek NT manuscript transcriptions)
- verse/entry rows total: **4,442,086**
- files with ERRORS: **0** | files with warnings: 5

Checks run on every file:

1. SQLite source: `PRAGMA integrity_check`, FTS row count == verse/entry count, no empty texts.
2. The written .txt is re-parsed line-by-line and compared row-for-row against the SQLite source (book, chapter, verse, text) — any mismatch is an error.
3. Leftover USFM/XML markup scan (`\marker`, `<tag>`, `strong=`): occurrences are preserved verbatim (the SQLite text is the source of truth) and reported as warnings.
4. One record per line: embedded newlines in source texts are flattened to spaces.

| file | rows | errors | warnings |
|---|---|---|---|
| greek-nt/Robinson-Pierpont Byzantine Textform 2018 (Greek New Testament, Majority Text) [grcByzRP2018].txt | 7,953 | OK | - |
| greek-nt/SBL Greek New Testament (SBLGNT, 2010) [grcSBLGNT].txt | 7,927 | OK | - |
| greek-nt/Tischendorf's Greek New Testament, 8th edition (Editio Octava, 1869-72) [grcTisch8].txt | 7,939 | OK | - |
| greek-nt/Robinson-Pierpont Byzantine Textform 2018 (Greek New Testament, Majority Text) [grcByzRP2018].txt | 7,953 | OK | - |
| greek-nt/SBL Greek New Testament (SBLGNT, 2010) [grcSBLGNT].txt | 7,927 | OK | - |
| greek-nt/Tischendorf's Greek New Testament, 8th edition (Editio Octava, 1869-72) [grcTisch8].txt | 7,939 | OK | - |
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
| translations/Bailey's Malayalam New Testament 1829 [malbailey1829].txt | 7,739 | OK | 125 verses contain markup-like characters (`<lb/>`, `<lg ...>` unconverted from the 1829 .SFM source; preserved verbatim) |
| translations/Malayalam Sathyavedapusthakam 1910, Contemporary Orthography (2015) [mal2015].txt | 31,098 | OK | - |
| translations/Sathyavedapusthakam 1910 (Malayalam Bible) [malsvp1910].txt | 31,098 | OK | - |
| translations/Bib La 1985 (Haitian Creole Bible) [hat].txt | 31,102 | OK | - |
| translations/Bibelen på Norsk 1930 (Norwegian Bible) [Norsk1930].txt | 31,101 | OK | - |
| translations/Bibla Shqiptare (Albanian Bible) [Alb].txt | 31,102 | OK | - |
| translations/Bible Kralická 1613 (Czech Bible) [ces1613].txt | 31,172 | OK | - |
| translations/Biblia 1776 (Finnish Bible) [FinBiblia].txt | 35,445 | OK | - |
| translations/Biblia Gdańska 1881 (Polish Bible) [PolGdanska].txt | 31,073 | OK | - |
| translations/Biblia Liberă (Romanian New Testament, Latin script) [ronbl].txt | 7,952 | OK | - |
| translations/Biblia Takatifu 1850 (Swahili New Testament) [swh1850].txt | 7,853 | OK | - |
| translations/Bíblia NVA (Portuguese Bible) [PorNVA].txt | 31,094 | OK | - |
| translations/Danish Bible OT 1871 NT 1907 (original orthography) [DaOT1871NT1907].txt | 31,063 | OK | - |
| translations/Diodati Bibbia 1885 (Italian Bible) [ita1885].txt | 31,095 | OK | - |
| translations/Elberfelder Bibel 1905 (German Bible) [deuelo].txt | 31,102 | OK | - |
| translations/Kinh Thánh 1934 (Vietnamese Bible) [vie1934].txt | 31,102 | OK | - |
| translations/Károli Biblia 1908 (Hungarian Bible) [HunKar].txt | 31,126 | OK | - |
| translations/Latviešu Bible, Glück 8th edition (Latvian Bible) [LvGluck8].txt | 31,102 | OK | - |
| translations/Londona Biblio 1910 (Esperanto Bible) [epo].txt | 31,102 | OK | - |
| translations/Louis Segond 1910 (French Bible) [fraLSG].txt | 31,170 | OK | - |
| translations/Lutherbibel 1912 (German Bible) [deu1912].txt | 31,102 | OK | - |
| translations/Petrus Canisiusvertaling 1939 (Dutch Catholic Bible) [nld1939].txt | 35,335 | OK | - |
| translations/Reina-Valera 1909 (Spanish Bible) [spaRV1909].txt | 31,084 | OK | - |
| translations/Riveduta Bibbia 1927 (Italian Bible) [ita1927].txt | 31,102 | OK | - |
| translations/Statenvertaling 1917 (Dutch Bible) [nld].txt | 31,102 | OK | - |
| translations/Stritarjeva Biblija 1882 (Slovenian Bible) [SloStritar].txt | 10,474 | OK | - |
| translations/Svenska Bibeln 1917 (Swedish Bible) [Swe1917].txt | 35,350 | OK | - |
| translations/Sveta Biblija (Croatian Bible, Šarić) [hrv].txt | 35,448 | OK | - |
| translations/Tagalog Bible 1905 (Philippine Bible Society) [TagAngBiblia].txt | 31,102 | OK | - |
| translations/Unlocked Literal Bible (Cebuano) [cebulb].txt | 31,103 | OK | - |
| translations/Unlocked Literal Bible (French) [frulb].txt | 7,958 | OK | - |
| translations/Unlocked Literal Bible (Hausa) [haulb].txt | 7,959 | OK | - |
| translations/Unlocked Literal Bible (Ilocano) [iloulb].txt | 31,090 | OK | - |
| translations/Unlocked Literal Bible (Indonesian) [idulb].txt | 7,945 | OK | 2 verses contain markup-like characters (preserved verbatim from source) |
| translations/Unlocked Literal Bible (Portuguese, Brazil) [ptbrulb].txt | 31,097 | OK | - |
| translations/Unlocked Literal Bible (Spanish, Latin America) [es419ulb].txt | 31,099 | OK | - |
| translations/Unlocked Literal Bible (Swahili) [swulb].txt | 31,101 | OK | - |
| translations/Unlocked Literal Bible (Tagalog) [tlulb].txt | 31,103 | OK | - |
| translations/Unlocked Literal Bible (Vietnamese) [viulb].txt | 31,073 | OK | - |
| translations/Biblia Platense (Straubinger) 1958 (Spanish Catholic Bible) [SpaPlatense].txt | 35,791 | OK | - |
| translations/Katholische Bibelübersetzung Rießler-Storr (Grünewaldbibel 1924, German Catholic Bible) [GerGruenewald].txt | 30,956 | OK | - |
| translations/La Bible Crampon 1923 (French Catholic Bible) [FreCrampon].txt | 35,486 | OK | 1 verse contains markup-like characters (preserved verbatim from source) |
| translations/Statenvertaling met apocriefen (Dutch Catholic Bible) [DutSVVA].txt | 36,939 | OK | - |
| critical-editions/Elizabeth Bible 1751 (Church Slavonic) [chuEliz1751].txt | 36,000 | OK | - |
| translations/Russian Freedom Bible (Bibliia svobody) [rusfb].txt | 25,324 | OK | - |
| translations/Russian Synodal Bible (Synodalnyi perevod) [russyn].txt | 31,169 | OK | - |
| translations/Serbian Bible, Daničić-Karadžić (Cyrillic, 1868) [srp1868].txt | 31,111 | OK | - |
| translations/Serbian Bible, Vuk Karadžić (Latin script, 1865) [srp1865].txt | 31,111 | OK | - |
| translations/Ukrainian Bible, Kulish translation 1905 (Biblia Kulisha) [ukr1871].txt | 31,082 | OK | - |
| translations/Ukrainian Freedom Bible (Biblia svobody) [ukrfb].txt | 31,082 | OK | - |
| translations/Unlocked Literal Bible (Russian, New Testament) [ruulb].txt | 7,954 | OK | - |


## Greek NT manuscript transcriptions (added 2026-10-29)

978 manuscript transcriptions (INTF Liste via gntcollations.com v2.0.0 and IGNTP
bulk zips, both CC BY 4.0) in `manuscripts/`, one file per witness. The same four
checks ran on every file: SQLite `integrity_check` = ok, no empty verse texts,
the written .txt re-parsed and compared row-for-row against the SQLite source
(0 mismatches across all 978 files), and a leftover-markup scan (0 hits).
The manuscript DBs omit the FTS index (corpus size); the 3 Greek NT edition
DBs in `greek-nt/` carry it, with FTS row count == verse count.

| category | files | rows | errors |
|---|---|---|---|
| papyri | 132 | 8,047 | 0 |
| uncials | 158 | 87,950 | 0 |
| minuscules | 591 | 536,727 | 0 |
| lectionaries | 55 | 53,724 | 0 |
| other (IGNTP supplement sigla) | 42 | 2,812 | 0 |
| **total** | **978** | **689,260** | **0** |

Spot checks: P75 Luke 3:18 = «μεν ουν και ετερα παρακαλων ευηγγελιζετο τον λαον·»;
Codex Sinaiticus (01) Matt 1:1 = «βιβλος γενεσεως ιυ χυ υιου δαδ υιου αβρααμ» (nomina
sacra kept in uncial spelling); RP2018 Matt 1:1 = «βιβλος γενεσεως ιησου χριστου υιου δαυιδ
υιου αβρααμ»; SBLGNT Matt 1:1 = «Βίβλος γενέσεως Ἰησοῦ χριστοῦ υἱοῦ Δαυὶδ υἱοῦ Ἀβραάμ.»;
Tischendorf 8th Matt 1:1 accented likewise. Lacuna-only verses are omitted and
counted in each DB's `edition` field; `<app>` readings resolve to the orig/first
hand reading.


## Greek NT manuscript transcriptions (added 2026-10-29)

978 manuscript transcriptions (INTF Liste via gntcollations.com v2.0.0 and IGNTP
bulk zips, both CC BY 4.0) in `manuscripts/`, one file per witness. The same four
checks ran on every file: SQLite `integrity_check` = ok, no empty verse texts,
the written .txt re-parsed and compared row-for-row against the SQLite source
(0 mismatches across all 978 files), and a leftover-markup scan (0 hits).
The manuscript DBs omit the FTS index (corpus size); the 3 Greek NT edition
DBs in `greek-nt/` carry it, with FTS row count == verse count.

| category | files | rows | errors |
|---|---|---|---|
| papyri | 132 | 8,047 | 0 |
| uncials | 158 | 87,950 | 0 |
| minuscules | 591 | 536,727 | 0 |
| lectionaries | 55 | 53,724 | 0 |
| other (IGNTP supplement sigla) | 42 | 2,812 | 0 |
| **total** | **978** | **689,260** | **0** |

Spot checks: P75 Luke 3:18 = «μεν ουν και ετερα παρακαλων ευηγγελιζετο τον λαον·»;
Codex Sinaiticus (01) Matt 1:1 = «βιβλος γενεσεως ιυ χυ υιου δαδ υιου αβρααμ» (nomina
sacra kept in uncial spelling); RP2018 Matt 1:1 = «βιβλος γενεσεως ιησου χριστου υιου δαυιδ
υιου αβρααμ»; SBLGNT Matt 1:1 = «Βίβλος γενέσεως Ἰησοῦ χριστοῦ υἱοῦ Δαυὶδ υἱοῦ Ἀβραάμ.»;
Tischendorf 8th Matt 1:1 accented likewise. Lacuna-only verses are omitted and
counted in each DB's `edition` field; `<app>` readings resolve to the orig/first
hand reading.
