# bible-text-files

All legally obtainable English Bible translations, critical editions, and
lexicons/reference works, as plain text files — generated from the verified
SQLite library in [`penguin-lt/bible-dyb-repo`](https://github.com/penguin-lt/bible-dyb-repo)
(releases `bibles-lexicons-core` and `critical-editions`).

## Layout

```
translations/        84 English Bible translations
critical-editions/   21 critical editions (Greek, Hebrew, Latin, Coptic, Syriac, Slavonic + English Brenton)
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
`integrity_check` with FTS row counts matching. **130 files, 2,219,998 rows,
0 errors.** See `VERIFICATION.md` for the per-file table and `SHA256SUMS.txt`
to check any download.

## Licence

Every text here is public domain or an openly licensed PD-equivalent source
(see the `license` column in the source databases). Copyrighted modern
translations (NIV, ESV, NLT, NASB, NET, SBLGNT, NA28, UBS, MLV, ALT…) are
deliberately **not** included.
