# Release notes

What each release changes, in a few lines, newest first. The desktop app's update window shows the newest entry and
links here. The app's About > Version history and `batch_rt_toolkit/CHANGELOG.md` hold the full detail.

## 0.6.3 (22 Nov 2026)

- Apply in Skyline shows its progress: a bar with Skyline's own percentage while it takes in the boundaries, and the
  time so far, with a Stop button (Apply works on a copy, so stopping leaves the document as it was). Export peak
  report and the results show it the same way.
- One results workbook, `results_<label>.xlsx` (raw areas, SERRF corrected, QC %CV summary and per molecule, About),
  in place of three. The SERRF input and the MetaboAnalyst file stay .csv files of their own.
- Sample groups: a one-line intro with a new Help section; Esc and Cancel close it, asking first when a Group was
  changed; "Fill in from file names again" no longer deletes the saved groups.
- Skyline Link tab: SERRF online or on this computer is chosen in the Results panel only (the line beside Export
  peak report shows which); the "by hand" steps are folded away. Log buttons are greyed out until there is a Log.
- Tutorial: "Pull the report and make the results" is now two shorter steps.
- Desktop app: the Full edition has its own icon (dark blue, teal peak), so it is easy to tell from the Researcher
  edition (blue, amber peak).

## 0.6.2 (19 Nov 2026)

- Desktop app updates fixed: the researcher edition now updates itself (0.6.0 and 0.6.1 copies were sent the lab
  installer). Install 0.6.2 by hand once; later releases update in the app.
- The update window shows what a release changes and links to these notes.
- Researcher edition: the technician-only options are hidden instead of greyed out.
- About: the release and Python first; the list of scripts is folded away (opens by itself if a part does not match).
  Shorter wording in the desktop app.

## 0.6.1 (18 Nov 2026)

- Desktop app: Check setup shows Skyline's command line and one line for the app's own Python and scripts; the
  Python and script folder fields are hidden.

## 0.6.0 (17 Nov 2026)

- Skyline Link tab: files for Skyline, Apply in Skyline, Sample groups, Open in Skyline and Export peak report in one
  place, then SERRF and the MetaboAnalyst file.
- Results as Excel tables with an About sheet; the SERRF input and the MetaboAnalyst file stay .csv.
- First desktop app (Windows): its own R and Python, installed without administrator rights.
