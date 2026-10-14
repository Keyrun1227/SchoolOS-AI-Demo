# SchoolOS AI — buyer-led acceptance checklist

This is the acceptance plan for the prototype and the next production milestone. It distinguishes the implemented browser demo from requirements that need a backend.

## Prototype workflows included

- [x] Login screen with demo credentials for one principal, one school admin, three teachers, and a parent preview.
- [x] Role-specific navigation; parent preview sees one fictional child only.
- [x] Principal overview: assessment activity, open actions, falling-result signals, intervention status.
- [x] Teacher directory and individual profiles: classes, subjects, assessment completion, marking indicator, recent activity, student progress evidence, gaps and support notes.
- [x] Student profile: assessment history, latest-vs-previous comparison, attendance context, intervention history.
- [x] Create assessment record; enter question-wise marks; calculate totals; publish results; export marks CSV.
- [x] Assign interventions; set due dates, responsible teacher, baseline, status and retest score; compare baseline with retest.
- [x] Parent meeting brief draft is editable and can be copied or printed. No message is sent.
- [x] Principal reports and CSV exports for student, teacher and intervention registers.
- [x] Mobile responsive navigation with a More menu for secondary sections.
- [x] Browser-local persistence and reset demo data action.
- [x] Explicit fictional-data and production-readiness warnings.

## Manual acceptance scenarios before sharing

1. Sign in as `principal@schoolos.demo` / `Principal123!`. Open Action centre and navigate from a task to its source record.
2. Open Teachers → Ananya Reddy → Assessment work, Student progress, and Context & support. Edit support notes and confirm they remain after reload in the same browser.
3. Open Students → Ishaan Varma. Confirm latest and previous percentages and the intervention history are visible.
4. Create an assessment. Add an available student row, edit question marks, save and publish. Export the marks CSV.
5. Assign an intervention to Ishaan. Edit its status and retest score. Confirm the baseline-to-retest change is shown.
6. Generate a parent meeting brief. Edit it, save it as a draft and verify the UI states that nothing was sent.
7. Sign out and sign in as each teacher. Confirm the teacher workspace does not show the principal's Teachers directory or school-wide action centre.
8. Sign in as `parent@schoolos.demo` / `Parent123!`. Confirm only the single demo child's approved-style progress view is presented.
9. Test on a 390px-wide phone viewport and desktop. Confirm the Teachers destination remains available, secondary destinations are under More, and tables scroll horizontally.
10. Reset demo data and verify the initial sample state returns.

## Production acceptance gates — not implemented in this static HTML

- [ ] Server-side authentication with secure password/session handling, recovery and account lifecycle.
- [ ] Server-enforced role-based access control; no trust in client-side role state.
- [ ] Multi-tenant school isolation at the database/API layer; automated cross-tenant denial tests.
- [ ] Shared database and real cross-device persistence; backups, restore drills and retention policies.
- [ ] Immutable audit trail for mark changes, publication, intervention completion, report generation and parent communication approvals.
- [ ] Input validation: marks cannot be negative or exceed question/assessment maximum; totals and rounding rules verified.
- [ ] Assessment blueprint, question-to-topic mapping review and support for imported state papers. AI-generated mappings must be teacher-approved.
- [ ] Actual student/class/subject roster imports with duplicate and identity-resolution safeguards.
- [ ] Privacy review for child data, consent and retention; least-privilege parent access; data export/deletion workflow.
- [ ] Real PDF/Excel report generation tested with Indian school formats and Unicode fonts.
- [ ] AI calls run through a server-side gateway with secrets protected, schema validation, cost limits, retries, and teacher review for generated materials.
- [ ] Email/WhatsApp delivery is optional, opt-in, logged, approved and retry-safe; no auto-send from an unreviewed AI draft.
- [ ] Accessibility, keyboard navigation, mobile-browser tests, performance checks and security review.
- [ ] Pilot with at least one school; measure workflow completion, correction rates, time spent and intervention/retest participation before making outcome claims.

## Fairness requirements

- Do not generate a single AI teacher score or leaderboard from student marks.
- Low marks are a prompt for review, not proof of teaching quality.
- Show assessment comparability, prior performance, attendance and syllabus coverage only when recorded and verifiable; identify missing data clearly.
- Separate workflow completion from student outcomes and from formal HR evaluation.
- Make teacher support needs visible and actionable, with a human review step.
- Parent-facing communication is a draft until a responsible staff member reviews and approves it.

## Release definition

The current release is a **functional local-data demo** suitable for product feedback and guided demonstrations. It is not a secure multi-user production application and must not be used to store real student records.
