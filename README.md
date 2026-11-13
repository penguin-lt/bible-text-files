# bible-text-files

All legally obtainable Bible translations in English, Malayalam and the major
Latin-script languages, plus critical editions and lexicons/reference works, as plain text files —
generated from the verified SQLite library in [`penguin-lt/bible-dyb-repo`](https://github.com/penguin-lt/bible-dyb-repo)
(releases `bibles-lexicons-core` and `critical-editions`).

## Layout

```
translations/        137 translations: 87 English, 3 Malayalam, 36 major Latin-script languages, 4 public-domain Catholic Bibles, 7 Slavic-language Bibles (PD / CC BY-SA 4.0 / Unlicense)
critical-editions/   22 critical editions (Greek, Hebrew, Latin, Coptic, Syriac, Slavonic + English Brenton)
greek-nt/            3 Greek New Testament editions: Robinson-Pierpont Byzantine Textform 2018 (PD), Tischendorf 8th ed. 1869-72 (PD), SBLGNT 2010 (CC BY 4.0)
manuscripts/         978 Greek NT manuscript transcriptions (132 papyri, 158 uncials, 591 minuscules, 55 lectionaries, 42 other) — INTF Liste via gntcollations.com and IGNTP bulk zips, all CC BY 4.0
lexicons/            25 lexicons and reference works
SHA256SUMS.txt       sha256 of every file
VERIFICATION.md      per-file error-check report
```

## File format

One record per line. Header line, then one line per verse:

```
[Translation Name] [Year] [Abbreviation]
[Book] [Chapter]:[Verse] [Text]
```

Lexicon/reference files use the same header, then one line per entry:

```
[Work Name] [Year] [Abbreviation]
[Entry Key] [Entry Text]
```

Notes:
- Verse/entry texts are flattened to a single line (embedded newlines become spaces).
- Text is verbatim from the SQLite source of truth; two files contain
  markup-like characters inherited from their sources (OSEN footnotes, one
  `\` in SAWYER) — preserved deliberately and listed in VERIFICATION.md.
- Three critical editions (Peshitta, Sixtine Vulgate, Church Slavonic) have
  word-count-reconstructed verse boundaries, flagged `verse_references =
  approximate` in their SQLite `note` table.

## Verification

Every file was re-parsed after writing and compared row-for-row against its
SQLite source (book, chapter, verse, text), and each SQLite file passed
`integrity_check` (FTS row counts match on the DBs that carry an FTS index;
the 978 manuscript-corpus DBs omit FTS to keep the corpus small). **1167 files, 4,442,086 rows,
0 errors.** See `VERIFICATION.md` for the per-file table and `SHA256SUMS.txt`
to check any download.

## Licence

Every text here is public domain or openly licensed (PD / CC0 / Unlicense / CC BY / CC BY-SA; see each database's license field).
Copyrighted modern translations (NIV, ESV, NLT, NASB, NET, NA27/NA28, UBS, MLV, ALT…) are
deliberately **not** included. The SBLGNT is included because its own EULA
(sblgnt.com/license) is the full text of CC BY 4.0; the Greek NT manuscripts
are CC BY 4.0 (INTF / IGNTP).
