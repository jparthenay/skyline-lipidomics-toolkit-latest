# Release notes

What each release changes, in a few lines, newest first. The desktop app's update window shows the newest entry and
links here. The app's About > Version history and `batch_rt_toolkit/CHANGELOG.md` hold the full detail.

## 0.6.9 (25 Nov 2026)

- Phospholipid Method Package SST: pick the Class ID or the Fatty Acid Composition SST. Each has its own standards
  (Class ID 10, Fatty Acid all 25 IS transitions) and Run IDs end -CID or -FA.
- Both save to one SST history and tracker, marked in a new SST column, so the shared transitions share their
  trends. A Show switch (All / Class ID / Fatty Acid) filters the report's trends and the tracker's summary and charts.
- SST: Run ID fills in for more file names, Skyline gets a 5 min RT window per standard, and the Skyline comparison
  shows the viewer's %CV beside Skyline's.
- Updates: the install progress window shows again (from the next update after this one).

## 0.6.8 (24 Nov 2026)

- Updates: the "available" label opens the updater directly, the app checks again every few hours while open, and
  the update windows open on the app's screen.
- SST: the area change comes from the last run in the SST history (the Previous SST results field is gone); each run
  writes its own Skyline transition list of the ticked standards; Run ID refreshes with a new folder; a WIS prep date
  after the run is flagged; Save to SST history always says where it saved.
- SST tracker workbook: Run IDs of digits only no longer leave the summary tabs empty (rebuild the tracker).
- Saturated peaks: one reading at the detector limit no longer inflates the area (TG_D5 %CV now close to Skyline's).
- The four Baker internal standards are annotation level 1. Dropdowns close when clicked again.

## 0.6.7 (24 Nov 2026)

- SST: a run whose standards elute late or early (e.g. after a blockage) is now found and measured where the peaks
  are, with the RT shift flagged; a peak cut off by its acquisition window is flagged and never passes.
- SST: sync integration copies a guide to every injection again (it used to blank injections it found no peak in).
- SST: the dashboard follows the Peak viewer areas / Skyline's areas switch, so the %CV and pass/fail can be on
  either. The SST settings fold away (Checks; areas in Skyline, watching and batch label).

## 0.6.6 (24 Nov 2026)

- System suitability (SST), Full edition only: one SST for the Baker method and the Phospholipid Method Package,
  with pass/fail as the FM-00063 form (area %CV and mean tailing factor per standard). The tailing factor, RT and
  areas were checked against LabSolutions Insight.
- Drop in the injections as they come off the instrument; test injections are shown with an IS mix check and kept
  out of the stats. Drag an integration guide and the SST is recalculated at once.
- Each method keeps its SST history in its own folder on the PC: save a run, copy its rows for the form online,
  pick the standards saved, remove runs. The Report tab shows peak area over time and trends.
- The Phospholipid Method Package SST also checks the Fatty Acid list's internal standard transitions, for the
  head groups that saturate.

## 0.6.5 (23 Nov 2026)

- Desktop app: the app window now always opens after the start-up window. It used to wait for Windows to report the
  page ready, and could stay on "Opening the window". It now opens once the page has loaded, or after 30 seconds at
  the latest. A window position saved on a screen that is no longer connected is placed again, and a page that does
  not load is tried again.

## 0.6.4 (23 Nov 2026)

- Skyline Link tab: it shows only the run that has just finished, or the earlier results you opened with Open
  previous results (the same run as the Report tab). Until then it is empty, with a short note saying so; it no
  longer fills in the document, files or fields of an earlier run. Opening earlier results chooses that batch's
  newest Skyline document (the adjusted copy, when Apply in Skyline made one). Before a run is loaded or finished,
  Sample groups opens empty with a note saying why, and the tab's buttons say the same.
- Desktop app: while an update installs, a small "Installing release ..." window stays on screen with a moving bar
  and the time so far. The install runs in the background and takes a few minutes (Windows unpacks and checks the
  app's own R and Python), and until it finishes the app's shortcut does not work. The window closes once the app is
  running again. If the app was closed with an update waiting, it says when to start the app again.
- The window first appears with the update after this one: the update to 0.6.4 itself still installs the old way.

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
