# SchoolOS AI — production architecture proposal

## Product boundary

The single-file HTML in this bundle is a demo front end. Its login is client-side, all data is fictional, and changes are saved in one browser's local storage. Do not publish it as if it were the live multi-user service.

## Proposed production layers

1. **Responsive web app / PWA** — principal, teacher and parent portals; accessible UI; offline-friendly draft entry with explicit sync state.
2. **Identity and access** — managed identity provider, server-side sessions, MFA for administrators, role and school membership checks on every API request.
3. **Application API** — assessments, question banks, marks, topic mapping, interventions, reports, notifications and audit events. Validate all data on the server.
4. **Relational database** — PostgreSQL with tenant/school identifiers, foreign keys, unique constraints, transactions and row-level security as defence in depth.
5. **File storage** — private object storage for imported papers and generated reports; short-lived signed URLs; malware/type/size validation.
6. **Background workers** — paper extraction, PDF/Excel generation, import processing and optional AI tasks. Idempotent jobs, retries and dead-letter handling.
7. **AI gateway** — provider keys only on server, strict JSON schemas, bounded retries and token/cost limits. Teacher review before a generated question map, remedial plan or parent draft becomes approved content.
8. **Observability and operations** — structured logs without unnecessary child data, metrics, error reporting, backup monitoring, restore drills and incident runbooks.

## Core entities

- School, User, RoleMembership, Class, Subject, TeacherAssignment, Student, ParentGuardianLink.
- Assessment, AssessmentQuestion, Topic, QuestionTopicMapping, AssessmentStudent, MarkEntry, PublicationEvent.
- Intervention, InterventionActivity, Retest, ParentBrief, MessageApproval, MessageDelivery.
- AuditEvent, ImportJob, ReportJob, AIUsageRecord.

## Essential invariants

- Every school-owned record has a school ID and server-validated membership.
- A teacher can access only assigned classes/students unless explicitly granted additional scope.
- A parent can access only a child linked through a verified guardian relationship, and only approved fields.
- Mark values and totals are validated against question and assessment maxima; changes to published marks are audited.
- Draft messages are never sent automatically. Approval, destination and delivery status are auditable.
- Student progress changes are shown only when assessment comparability and underlying records are available; uncertain interpretations are labelled.
- Teacher workflow indicators are not converted into an automated performance score.

## Deployment stages

- Stage A: usability prototype with fictional data (this bundle).
- Stage B: single-school pilot with authenticated users and shared database; no AI claims; controlled imports.
- Stage C: add robust question mapping, report generation, audit logs and intervention evidence.
- Stage D: optional AI support and approved messaging integrations after privacy/security review.
- Stage E: multi-school SaaS after tenant-isolation tests, operational controls, support process and commercial validation.
