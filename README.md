Version history (newest first):

2.0.0-rc.6  (2026-10-13)
  - Fixed: Android app: the Gradle sync failed ("Unresolved reference: util" in the setting that finds PoDoFo).

2.0.0-rc.5  (2026-10-13)
  - Added: Android app: PoDoFo, the PDF engine of the Windows program, linked into the app when it is built with it (android/tools/podofo); About shows it. The print screens come next.

2.0.0-rc.4  (2026-10-13)
  - Fixed: the Windows build stopped at once (MSB4092, the condition that reads the commit count).

2.0.0-rc.3  (2026-10-13)
  - Changed: the number after the version is the count of the commits of its source (v2.0.0-rc.3.cmt.61), the same on every PC that builds the same commit, instead of a count of the builds of each PC; the window title, the versioned exe, About and the published releases show it.
  - Note: a build from a shallow clone or without git shows cmt.0 (unknown) and is not published.

2.0.0-rc.2  (2026-10-13)
  - Fixed: the Windows build: the statistics window did not compile (a header of its chart was missing).

2.0.0-rc.1  (2026-10-13)
  - Changed: the database format: the tables, triggers and indexes of the program inside a database are named "_dbt_..." and its refusals "DBT:..." (they carried the name of the program SQLite DB Tools came from). A database made by a version 1.x is converted when it is first opened (Windows and Android, also a database to merge): the file as it was is kept next to it as <name>.format1.bak, the only one the versions 1.x can open; the records do not change. A file that cannot be written is not converted and says so.
  - Note: a database converted cannot be opened by the versions 1.x (use the .format1.bak copy there); the sample databases are of the new format.
  - Changed: everything of version 1.1.0-rc.1 to rc.15 (below) is part of this version.

1.1.0-rc.15  (2026-10-13)
  - Changed: the PDFs carry the mark of SQLite DB Tools (its icon: "D B" in yellow over "Tools" in blue, the stripes and titles in its colours) instead of the mark of another program.
  - Fixed: a PDF with a character its font does not have (Chinese, Japanese, Hindi ... with Arial) was not written at all: each character now comes from the first font that has it (on Windows Nirmala UI, Microsoft YaHei, Yu Gothic, Meiryo, Malgun Gothic, Segoe UI Symbol), else it is printed as "?".
  - Added: the fonts of the PDFs can be given by the program (PdfOut::setFonts): the Android app will use the fonts of the device.
  - Changed: a file of another program's environments dropped on the window is no longer named as such: it is one of the files the program cannot open.

1.1.0-rc.14  (2026-10-13)
  - Added: Android app: Merge, as in Windows: another database of the app or of the device (with its passphrase and login), its table into a table here or a new one, the plan of every column (filled from, name, the value of empty values and of the records here), Merge with each conflict asked (skip, overwrite, keep both, for all), Copy Several Tables, and the preview: every incoming record edited, left out or chosen, value by value, before Apply.
  - Changed: the notes of the merge plan, the preview of a new table named like one here, which values differ, "taking a value overwrites" and the counts of the preview are in the engine (Merger), the same for both apps.

1.1.0-rc.13  (2026-10-13)
  - Added: Android app: a warning counts down before the automatic lock, as in Windows; from the third wrong login the next one waits (up to 10 s).
  - Changed: Android app: the automatic lock is on by default after 10 minutes, as in Windows.
  - Fixed: Android app: the lock no longer rebuilds the screens under it, so what was typed and not saved is kept.
  - Changed: the wait after wrong logins, the default time of the automatic lock and when its warning starts are in the engine (Lock), the same for both apps.

1.1.0-rc.12  (2026-10-13)
  - Added: Android app: Users and Access (switch the accounts on, a new account, change its level, lock / unlock it, a new password), Change My Password and Switch User; Home shows the level by its name.

1.1.0-rc.11  (2026-10-13)
  - Added: Android app: Lock Now and the automatic lock after a time without a touch (also in the background): the screens keep their work, the password of the account or the passphrase unlocks, from the third wrong try the next one waits; close and discard from the lock screen.
  - Changed: who can unlock, the password check and the wait after wrong tries are in the engine (Lock), the same for both apps.

1.1.0-rc.10  (2026-10-13)
  - Fixed: the messages of the record and column limits no longer speak of a license (the program is free, its limits are fixed: Home shows them).
  - Added: Android app: SQL query (read only) and the operations log, with the history of a record; texts that spoke of a computer, windows or tabs say device and screens there.

1.1.0-rc.9  (2026-10-13)
  - Added: Statistics over time (Made of): the records active in each period (start and end dates: staff, contracts, rentals), the last record up to each period carried forward (a price list, readings), and the past values of a column rebuilt from the operations log (a price history); every day, week, month, quarter or year from the first date (or From) to today (or To); the first group splits them.
  - Changed: Statistics chart: series are stacked only when the measure adds up (a count, a sum); over time a price, an average or a minimum is one line per series; twelve colours.

1.1.0-rc.8  (2026-10-13)
  - Added: Android app: a table or chart that scrolls inside a page has a button that brings it in front, full screen, where only it scrolls (back puts it back).
  - Added: Android app: Settings > Screen orientation - as the device, the best for this screen (upright on a phone, sideways on a tablet), always upright, always sideways, turning even when the device's rotation is locked, or locked as it is; the screen's size and density shown with the advice.
  - Fixed: Android app: what is typed in a form, a table's structure, a statistic, a search, an import or an export is kept when the app is rebuilt (a change of language, Android closing it in the background); an entry being edited is no longer replaced by a reload.

1.1.0-rc.7  (2026-10-13)
  - Changed: Statistics chart: grouped by a date, columns in time order ("Oct 2025") with an optional line; grouped by anything else, bars with the largest first; a scale with gridlines; one colour (negative values in red).
  - Added: Statistics chart: with a second group, its values stacked (or side by side when some are negative) with a legend.
  - Changed: Statistics: every row is in the chart, which scrolls (sideways for columns, down for bars) instead of leaving rows out; the mouse (a tap on Android) shows the exact values; the chart starts on the first measure.
  - Fixed: Statistics (Windows): the table is as wide as its columns, so every measure is in view.

1.1.0-rc.6  (2026-10-13)
  - Fixed: Android app, Statistics on a phone: the Sort by choice was squeezed to nothing by the descending switch; the buttons wrap to a second line instead of breaking Functions...

1.1.0-rc.5  (2026-10-13)
  - Added: Android app: Home shows every function of the Windows program; those not in the app yet are marked with a clock (Lock, Edit Database, Merge, SQL, print profiles, operations log, accounts and protection), Open Attachment Folder is crossed out (not possible on Android); a tap explains.

1.1.0-rc.4  (2026-10-13)
  - Changed: Android app: needs Android 10 (2019) or newer.
  - Note: Android app: emulators from a 2019 phone to the newest Android, a tablet and a foldable, downloaded by Gradle for the automatic tests.

1.1.0-rc.3  (2026-10-13)
  - Added: Android app: Statistics (Home > Statistics...) with everything of the Windows tab - groups, the six measures, conditions, shown as, formulas of the measures, saved statistics, the bar chart, the result shared as CSV; the definition beside the result on a tablet.

1.1.0-rc.2  (2026-10-13)
  - Added: Statistics: up to six measures (M1 ... M6); new functions Count of different values, Median, Standard deviation and Variance (of a sample or of all), Product, First / Last value.
  - Added: Statistics: "Only when" - a condition per measure (as SUMIF / COUNTIF / AVERAGEIF of a spreadsheet).
  - Added: Statistics: "Shown as" - % of the total, running total, rank, difference and change (%) from the row before.
  - Added: Statistics: Formula of the measures - a calculation on the other measures of the row ({M1} / {M2}, or by their headings), also on the totals.
  - Added: formulas: comparisons, and / or / not, if(), and functions of numbers, texts and dates (mod, power, sqrt, roundup, left, right, replace, find, months, addmonths, eomonth...); Statistics > Functions... lists them all.
  - Fixed: Statistics: the minimum / maximum of a date or a text is shown as it is, no longer as a number.

1.1.0-rc.1  (2026-10-12)
  - Added: Arabic translation, with the windows laid out right to left.
  - Added: Database > Attachment Folder Location: relative to the database, to the program, or any folder (a folder outside the database's own is used once confirmed on each computer); the files already attached moved, copied or left.
  - Added: Database > Check Attachments: the records whose files are missing, with a Fix button for each missing file.
  - Added: the name of a new attached file chosen per column: table, record number, values of other columns, the column's name.
  - Added: sample databases Calibration, Shop and Library (Help > Sample Databases), with a chapter of the manual each.
  - Added: Merge > Preview: every incoming record editable before it is written; for a record already here, the value kept chosen cell by cell.
  - Added: Merge > Copy Several Tables, with their relations and automations; a table with the same name renamed (the copy or the existing one) or replaced.
  - Added: a triple click on a row of the records starts editing it.
  - Changed: Help > Version Info shows its text selectable and scrolled, like About.
  - Changed: the third-party notices listed component by component; the license names D. Richard Hipp, the author of SQLite.
  - Note: translations of every new text and of the manual in all the languages.

1.0.0-rc.1  (2026-10-09)
  - Added: SQLite databases, plain or encrypted (admin password + recovery key, or passphrase; every SQLite3 Multiple Ciphers / SQLCipher format), one per window - several copies may run side by side.
  - Added: Home tab with every action, enabled when it can run; every table, form, search, query, statistics and log in its own tab.
  - Added: tables and columns with types, rules, defaults and templates; references, relations, indexes and automations between the tables of the database.
  - Added: import from CSV / text / Excel (xlsx, xls) / OpenDocument (ods), also by dropping files; export to SQL, CSV, JSON and database copies; merge of databases.
  - Added: read-only SQL, statistics, prints and PDF, accounts with levels, operations log, attachments next to the database.
  - Added: translations and manuals in English, Italian, French, German, Russian, Spanish, Portuguese, Chinese, Hindi and Japanese.
  - Note: free of charge, no license key; up to 255 tables of 255 columns and 522,003 records per database (a database beyond them opens read-only).
