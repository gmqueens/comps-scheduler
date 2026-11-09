# SKHS Comps Scheduler

A browser tool that builds the full timeline for a Science PhD comprehensive exam in the School of Kinesiology and Health Studies (SKHS) at Queen's University. Enter one start date. The tool sets every deadline in working days, following the *SKHS Comprehensive Exam Forms and Procedures (Science PhD)*, version of 2 November 2026.

**Use it online:** https://gmqueens.github.io/comps-scheduler/

## What it does

- Schedules the initial organizing meeting, exam packages to the Chair and final revised packages.
- Schedules each reading list release, memory aid deadline, written exam and response circulation.
- Proposes six oral exam dates, 5 to 10 working days after the third written exam, with the examiner report deadline for each.
- Records the writer, topic area (i to v) and focus of each question, and checks the topic area rules.
- Shows a month calendar and produces plain text of the schedule for email.

## Running it

No installation is needed. The whole tool is one file, `index.html`.

- **Online:** open the link above in any browser.
- **Offline:** download `index.html` and open it in a browser. It works without a connection, using system fonts in place of the web fonts.

It runs on Windows, macOS, Linux, iOS and Android.

## Scheduling rules

All intervals are working days.

| Step | Timing |
|---|---|
| Exam packages to Chair | 15 days after the organizing meeting |
| Final revised packages to Chair | 5 days after packages are due |
| First reading list to Candidate | 10 days after packages are due |
| Each reading list to Candidate | 10 days before its written exam |
| Memory aid for approval | 3 days before each written exam |
| Response circulated | Within 3 days after each written exam |
| Next written exam | At least 14 days after the previous one |
| Examiner reports to Chair | 2 days before the oral |
| Oral exam | 5 to 10 days after the final written exam |

The start date can be set as the organizing meeting, the package deadline or the first reading list.

## Topic areas

Each Candidate answers 3 distinct questions drawn from five areas: (i) General background, which is mandatory; (ii) Current developments; (iii) Current controversies; (iv) Methodological issues; and (v) Theoretical issues. Two questions may share an area if their content differs. The tool flags a missing General background question and asks for a focus line when two questions share an area.

## Non-working days

The tool skips weekends and these days off: New Year's Day, Family Day, Good Friday, Victoria Day, Canada Day, Civic Holiday, Labour Day, the National Day for Truth and Reconciliation, Thanksgiving, Christmas Day, Boxing Day and the Queen's winter closure (24 December to 1 January). Each can be switched off. Extra dates, such as committee travel, can be blocked. Confirm closure dates against the Queen's calendar each year.

## Privacy

Names and settings are saved only in the local storage of the browser that entered them. The page sends no exam data to any server. Its only outside request loads the Google Fonts typefaces.

## Changing the Chair

The Chair is set to Dr. Gerome Manson. To use a different Chair, edit the `CHAIR` line near the top of the script in `index.html`.

## Author

Gerome Manson, School of Kinesiology and Health Studies, Queen's University.
