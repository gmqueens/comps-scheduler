# SKHS Comps Scheduler

A browser tool that builds the full timeline for a Science PhD comprehensive exam in the School of Kinesiology and Health Studies (SKHS) at Queen's University. Enter one start date. The tool sets every deadline in business days, following the *SKHS Comprehensive Exam Forms and Procedures (Science PhD)*, version of 2 November 2026.

**Use it online:** https://gmqueens.github.io/comps-scheduler/

## What it does

- Schedules the initial organizing meeting, the reminder to Examiners, exam packages to the Chair and final approved packages.
- Schedules each reading list release, memory aid deadline, written exam, 4-business-day break and response circulation.
- Offers a calendar for picking the oral exam date from the eligible days, 5 to 10 business days after the third written exam, and adds the examiner report deadline.
- Records the writer, topic area (i to v) and focus of each question, and checks the topic area rules.
- Stores the Chair's and Examiners' email addresses and writes a ready-to-copy email to the committee with the schedule and the proposed oral date.
- Shows a colour-coded month calendar with the breaks between exams highlighted.
- Downloads the dates as an `.ics` calendar file (committee dates, Candidate dates, the oral exam only, or every date) to attach to the committee email. Meeting, written exam and oral start times are optional; without them the events are all-day.

## Running it

No installation is needed. The whole tool is one file, `index.html`.

- **Online:** open the link above in any browser.
- **Offline:** download `index.html` and open it in a browser. It works without a connection, using system fonts in place of the web fonts.

It runs on Windows, macOS, Linux, iOS and Android.

## Scheduling rules

All intervals are business days: Monday to Friday, minus the days off listed below. As in the procedures, the first reading list is business day 1.

| Step | Timing |
|---|---|
| Organizing meeting | At least 25 business days before the start date |
| Exam packages to Chair | 10 business days before the start date, giving Examiners 15 business days after the meeting |
| Reminder email to Examiners | 5 business days before packages are due |
| Final approved packages to Chair | 5 business days before the start date |
| First reading list to Candidate | The start date (business day 1) |
| Each reading list to Candidate | 10 business days before its written exam |
| Memory aid for approval | At least 3 business days before each written exam |
| Break after each written exam | 4 business days |
| Next reading list | The business day after the break |
| Spacing of written exams | At least 14 business days between exams, so business days 11, 26 and 41 |
| Response circulated | Within 3 business days after each written exam |
| Examiner reports to Chair | At least 2 business days before the oral |
| Oral exam | 5 to 10 business days after the final written exam |

The organizing meeting and the start date are entered separately. The tool warns when the meeting is fewer than 25 business days before the start date, and offers to move either date.

## Topic areas

Each Candidate answers 3 distinct questions drawn from five areas: (i) General background, which is mandatory; (ii) Current developments; (iii) Current controversies; (iv) Methodological issues; and (v) Theoretical issues. Two questions may share an area if their content differs. The tool flags a missing General background question and asks for a focus line when two questions share an area.

## Non-working days

The tool skips weekends and these days off: New Year's Day, Family Day, Good Friday, Victoria Day, Canada Day, Civic Holiday, Labour Day, the National Day for Truth and Reconciliation, Thanksgiving, Christmas Day, Boxing Day and the Queen's winter closure (24 December to 1 January). Each can be switched off. Extra dates, such as committee travel, can be blocked. Confirm closure dates against the Queen's calendar each year.

## Privacy

Names, email addresses and settings are saved only in the local storage of the browser that entered them. The page sends no exam data to any server and never sends email itself. Its only outside request loads the Google Fonts typefaces.

## Changing the Chair

The Chair's name and email are entered in the Committee settings. The name defaults to Dr. Gerome Manson. To change that default, edit the `DEFAULT_CHAIR` line near the top of the script in `index.html`.

## Author

Gerome Manson, School of Kinesiology and Health Studies, Queen's University.
