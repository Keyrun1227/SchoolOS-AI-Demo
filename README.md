# 🎓 SchoolOS AI — Intelligent Academic Assessment & Learning Platform

<p align="center">
  <strong>From Assessment to Measurable Academic Progress</strong>
  <br>
  Transform student assessment data into meaningful insights, targeted revision, and continuous learning improvement.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/AI-Powered%20Learning-0F766E?style=for-the-badge" alt="AI-Powered Learning">
  <img src="https://img.shields.io/badge/Platform-Education-1D4ED8?style=for-the-badge" alt="Education Platform">
  <img src="https://img.shields.io/badge/Architecture-Full--Stack-334155?style=for-the-badge" alt="Full Stack">
  <img src="https://img.shields.io/badge/Focus-Academic%20Improvement-0D9488?style=for-the-badge" alt="Academic Improvement">
</p>

<p align="center">
  <a href="https://schoolos-ai-0z1k.onrender.com/">🌐 Live Website</a> •
  <a href="https://github.com/Keyrun1227/SchoolOS-AI-Assessment-Agent">💻 GitHub Repository</a>
</p>

---

## 🌟 Introduction

**SchoolOS AI** is an intelligent academic assessment and learning platform designed to help schools move beyond marks and traditional examination reports.

The platform focuses on turning assessment results into actionable learning insights. It aims to help educators identify learning gaps, plan targeted revision, conduct retests, and understand academic progress through a structured, evidence-driven workflow.

Rather than treating every assessment as an isolated event, SchoolOS AI connects the stages of teaching and learning into a continuous improvement cycle.

**Our mission:** Help schools make better academic decisions through meaningful assessment data and more focused learning support.

## 🎯 The Core Learning Cycle

<p align="center">
  <strong>📝 Assess → 🔍 Analyse → 📚 Revise → 🧪 Retest → 📈 Measure</strong>
</p>

| Stage | Purpose |
|---|---|
| 📝 Assess | Create or manage assessments and capture student performance. |
| 🔍 Analyse | Identify performance patterns, weak topics, and learning gaps using available assessment evidence. |
| 📚 Revise | Focus revision activities on the concepts students need to strengthen. |
| 🧪 Retest | Reassess learning using relevant follow-up questions or assessments. |
| 📈 Measure | Compare recorded results to understand progress and identify remaining learning needs. |

The objective is simple: **make assessment useful for the next teaching decision, not just the final report.**

---

## 🏫 Designed for the School Community

SchoolOS AI is organised around four key user roles.

### 👨‍💼 1. Principal Workspace

Designed to support school-level academic oversight.

- Review academic performance information available to the school.
- Understand class and subject performance patterns.
- Identify areas that may need additional academic attention.
- Support teacher follow-up and academic planning.
- Review available reports and performance summaries.

### 👩‍🏫 2. Teacher Workspace

Designed to support the day-to-day assessment and revision workflow.

- Create or manage assessments through supported workflows.
- Enter and review student marks.
- Analyse performance at question and topic levels where supported.
- Identify learning gaps using assessment evidence.
- Plan focused revision and follow-up assessments.
- Compare recorded assessment and retest results.

### 👨‍👩‍👧 3. Parent Workspace

Designed to help parents understand their linked children's academic progress.

- Review available assessment results.
- Understand subject-level performance.
- Follow learning priorities and recorded progress.
- Access reports permitted by the application's authorization rules.

### 🎒 4. Student Workspace

Designed to help students understand their own learning needs.

- Review permitted personal academic information.
- Understand areas requiring additional practice.
- Follow revision and retest activities where available.
- Track recorded progress across supported learning workflows.

*Available actions depend on the implemented features, account permissions, and configured data.*

---

## 🧠 Key Features

### 📊 Academic Assessment and Analysis

SchoolOS AI is built around structured assessment data and meaningful performance analysis.

- Assessment and marks-management workflows.
- Topic-level learning-gap identification where supported.
- Performance summaries based on available records.
- Data-driven revision recommendations.
- Before-and-after comparison of recorded assessment results.

### 📚 Targeted Revision

The platform's learning approach connects observed weaknesses to focused practice.

Instead of asking only, “What mark did the student score?”, the goal is to ask:

- Which concept needs attention?
- What evidence supports that conclusion?
- What revision activity would help?
- Did the follow-up assessment show improvement?

### 🤖 AI-Assisted Academic Support

AI can support interpretation, explanations, and learning guidance where the corresponding provider and integration are configured.

SchoolOS AI's intended approach is to combine AI assistance with reliable application logic. Marks, percentages, and progress calculations should be derived from actual records and deterministic calculations—not invented by a language model.

### 📈 Progress Tracking

Connect initial assessments and follow-up assessments to help educators understand:

- Previous performance.
- Identified learning needs.
- Follow-up assessment results.
- Recorded improvement.
- Concepts that still require attention.

Progress claims should always be supported by saved assessment evidence.

### 🎮 SchoolOS Learning Expedition

The Learning Expedition is an educational adventure concept that introduces the academic improvement cycle through interactive missions.

The planned mission sequence includes:

1. **Assessment Lab** — choose an appropriate assessment setup.
2. **Analysis Observatory** — interpret results and identify a learning gap.
3. **Revision Garden** — practise concepts through interactive activities.
4. **Retest Arena** — answer a follow-up challenge and compare results.

The learning experience uses fictional sample scenarios and is intended to complement—not replace—the core academic application.

### 🔐 Role-Based Academic Access

SchoolOS AI is designed around separate Principal, Teacher, Parent, and Student experiences.

Protected data must be enforced through backend authentication and authorization, including appropriate school, user, and student relationships. Hiding a screen in the frontend alone is not sufficient security.

---

## 🖥️ Technology Stack

The repository contains a full-stack web application. The following technologies are identified in the project architecture.

| Layer | Technology |
|---|---|
| Frontend | Next.js, React, TypeScript |
| Backend API | Python, FastAPI |
| Database | SQLite in the current backend configuration; PostgreSQL migration/reference files are also present |
| API communication | HTTP/REST |
| AI integration | Configurable AI provider integration |
| Testing | Python backend tests and frontend verification scripts |
| Deployment target | Render |

*Verify the current source and deployment configuration before describing any database, provider, or hosting setup as production-ready.*

---

## 🏗️ High-Level Architecture

```text
              SchoolOS AI
                   |
        ┌──────────┴──────────┐
        |                     |
   Web Frontend          User Interface
   Next.js / React       Four Role Workspaces
        |                     |
        └──────────┬──────────┘
                   |
              Backend API
               FastAPI
                   |
        ┌──────────┴──────────┐
        |                     |
   Academic Logic        AI Integration
        |                     |
        └──────────┬──────────┘
                   |
              Data Storage
          Current SQLite Setup
```

This is a conceptual architecture diagram, not a guarantee that every workflow or integration has been validated in a live deployment.

---

## 📂 Project Structure

The repository includes frontend, backend, database-related resources, and tests. The main areas are organised approximately as follows:

```text
SchoolOS-AI-Assessment-Agent/
│
├── backend/
│   ├── app/
│   │   └── main.py
│   ├── tests/
│   ├── requirements.txt
│   └── README.md
│
├── frontend/
│   ├── app/
│   ├── lib/
│   ├── tests/
│   └── package.json
│
├── database/
│   └── migrations/
│
├── docs/
│
├── .env.example
├── README.md
└── START-SCHOOLOS.bat
```

*Directory contents may vary by repository version. Refer to the actual source tree for the authoritative file list.*

---

## ⚙️ Getting Started

### Prerequisites

Install the following before starting local development:

- Python compatible with the backend's declared requirements.
- Node.js and npm compatible with the frontend dependencies.
- Git.
- An AI provider API key only if you want to test provider-dependent functionality.

### 1. Clone the Repository

```bash
git clone https://github.com/Keyrun1227/SchoolOS-AI-Assessment-Agent.git
cd SchoolOS-AI-Assessment-Agent
```

### 2. Set Up the Backend

```bash
python -m venv .venv
```

Activate the environment.

**Windows:**

```bash
.venv\Scripts\activate
```

**macOS / Linux:**

```bash
source .venv/bin/activate
```

Install backend dependencies:

```bash
pip install -r backend/requirements.txt
```

Configure the required environment variables using the project's `.env.example` and backend documentation. Do not commit API keys, credentials, or production secrets.

Start the API using the repository's documented startup command. For the FastAPI application, the entry point is `backend/app/main.py`; confirm the required working directory and environment before launching it.

### 3. Set Up the Frontend

Open a second terminal:

```bash
cd frontend
npm install
```

Configure the frontend API base URL using the supported environment variable:

```env
NEXT_PUBLIC_API_BASE_URL=http://localhost:8000
```

Run the development server:

```bash
npm run dev
```

Use the actual backend port and environment configuration for your local setup.

### 4. Open the Application

Visit the local frontend URL displayed by the Next.js development server.

For the deployed website, visit:

**https://schoolos-ai-0z1k.onrender.com/**

Live availability, authentication, and deployed features depend on the current deployment configuration.

---

## 🧪 Testing and Verification

Run the checks supported by the current repository.

### Backend Tests

```bash
pytest backend/tests -v
```

### Frontend Typecheck

```bash
cd frontend
npm run typecheck
```

### Frontend Production Build

```bash
npm run build
```

A successful build is an important quality gate, but it does not independently prove authorization, data isolation, download correctness, or production readiness.

Important areas to verify before release:

- Login, logout, and session expiry.
- Role and school-level authorization.
- Assessment creation and marks validation.
- Topic analysis and revision recommendations.
- Retest linkage and result comparisons.
- Authorized downloads and rejection of unauthorized requests.
- Database persistence and backup/restore.
- Responsive layouts and keyboard accessibility.
- Learning Expedition mission progression and fictional-data isolation.

Document the actual results for the version being tested. Do not treat historical test results as proof that a newer version passes.

---

## 🔒 Security and Privacy

SchoolOS AI is intended to handle sensitive educational information, so security is a core requirement.

- Keep API keys and secrets on the server.
- Enforce authorization in backend endpoints.
- Scope parent access to explicitly linked children.
- Restrict students to their permitted personal records.
- Prevent cross-school access.
- Protect reports and file downloads.
- Keep public previews and educational game scenarios separate from real school records.
- Avoid including private school data or credentials in source archives.
- Use synthetic data for public demonstrations and isolated tests.

**Important:** Do not use the platform for real student records until authentication, authorization, data isolation, persistence, and deployment security have been adequately verified.

---

## 🚀 Deployment

The project has a public Render deployment target.

Before deploying an updated version:

1. Preserve the current working release.
2. Review the source changes and environment variables.
3. Run backend tests and the frontend production build.
4. Verify authentication and protected downloads.
5. Test the academic workflow using isolated test data.
6. Confirm database persistence and recovery arrangements.
7. Test role-based access and public demo isolation.
8. Deploy through the intended release process.
9. Verify the deployed application and retain a rollback option.

A local source update does not automatically update the live website.

---

## 🗺️ Product Roadmap

The following are ongoing engineering priorities, not claims that every item is already complete.

- [ ] Complete end-to-end verification of all four role workflows.
- [ ] Verify authenticated report downloads and export permissions.
- [ ] Verify parent-child and school-level data isolation.
- [ ] Validate the full assessment-to-retest cycle against saved records.
- [ ] Complete frontend build and browser regression testing.
- [ ] Validate database backup and restore procedures.
- [ ] Finish and verify all Learning Expedition interactions.
- [ ] Validate deployment configuration and operational monitoring.
- [ ] Improve accessibility and responsive behaviour across workspaces.

---

## 🤝 Contributing

Contributions, bug reports, and suggestions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Make a focused change.
4. Add or update relevant tests.
5. Run the available checks.
6. Submit a pull request describing the change and its verification results.

Please avoid submitting secrets, private student data, or production database files.

---

## 📌 Project Status

SchoolOS AI is an evolving education technology project focused on academic assessment, learning-gap analysis, targeted revision, and progress measurement.

Its intended value is to connect the work teachers already do with clearer evidence about what students should learn next.

**The long-term vision:** Every assessment should help inform the next learning action.

---

## 👨‍💻 Maintainer and Links

- **Project:** SchoolOS AI
- **Repository:** https://github.com/Keyrun1227/SchoolOS-AI-Assessment-Agent
- **Website:** https://schoolos-ai-0z1k.onrender.com/

---

<p align="center">
  <strong>🎓 SchoolOS AI</strong>
  <br>
  <em>Assess better. Teach smarter. Help every learner progress.</em>
</p>
