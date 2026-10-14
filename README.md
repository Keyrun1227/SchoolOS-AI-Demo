# SchoolOS AI — End-to-end workflow demo

A responsive single-file concept prototype for demonstrating principal/admin and teacher workflows. It is designed for GitHub Pages and local browser testing.

## Demo sign-in

- Principal: `principal@schoolos.demo` / `Principal123!`
- School admin: `admin@schoolos.demo` / `Admin123!`
- Parent preview: `parent@schoolos.demo` / `Parent123!` (fictional child record only)
- Teacher Ananya Reddy: `ananya@schoolos.demo` / `Teacher123!`
- Teacher Ravi Kumar: `ravi@schoolos.demo` / `Teacher123!`
- Teacher Meena Lakshmi: `meena@schoolos.demo` / `Teacher123!`

These credentials are intentionally public demo credentials, not secure authentication.

## Run

Open `index.html` in a modern browser, or host it with GitHub Pages. It is mobile responsive. For GitHub Pages, put `index.html` at the repository root and choose `main` / `/(root)` under Settings → Pages.

## Included workflows

- Role-specific sign-in and role-specific navigation for principal, school admin, three teachers and a limited parent preview.
- Principal overview and action centre.
- Teacher directory and individual teacher profiles with assigned classes/subjects, assessment status, student evidence, remaining gaps, attendance/syllabus context and support needs.
- Student profile, latest-vs-previous performance, attendance context, intervention history and parent-meeting draft.
- Assessment creation, question-wise mark entry, calculated totals, publication status and CSV export.
- Learning gap review and intervention assignment, completion status, baseline/retest entry and comparison.
- Reports, printable drafts and CSV exports.
- Local browser persistence and reset-to-demo-data action.
- Mobile navigation with high-frequency destinations and a More menu.

## Important limitations

This is a functional **local-data prototype**, not a production system. Changes are stored in that browser only and do not synchronise across devices. Authentication is simulated client-side and can be bypassed; it must never protect real data. There is no shared database, backend API, secure tenant isolation, server-side audit log, backup, live AI paper extraction/mapping, email or WhatsApp delivery, billing, or production monitoring. All names and records are fictional. Do not enter real student data.

Before a paid school pilot, implement server-side authentication and role-based access control, a shared database with school-level row isolation, audit logs, backups, secure deployment, privacy/data-retention controls, and acceptance testing with a school. Verify all calculations and topic mappings with actual teacher-reviewed records.
