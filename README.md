# 🎓 SchoolOS AI — Intelligent Academic Assessment & Learning Platform

<p align="center">
  <strong>From Assessment to Measurable Academic Progress</strong>
  <br>
  Transform assessment results into meaningful insights, targeted revision, and continuous learning improvement.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/AI-Assisted%20Learning-0F766E?style=for-the-badge" alt="AI-Assisted Learning">
  <img src="https://img.shields.io/badge/Platform-Education-1D4ED8?style=for-the-badge" alt="Education Platform">
  <img src="https://img.shields.io/badge/Architecture-Full--Stack-334155?style=for-the-badge" alt="Full Stack">
  <img src="https://img.shields.io/badge/Focus-Academic%20Improvement-0D9488?style=for-the-badge" alt="Academic Improvement">
</p>

<p align="center">
  <a href="https://schoolos-ai-0z1k.onrender.com/">🌐 Live Website</a>
  &nbsp;•&nbsp;
  <a href="mailto:chitturidurgasatyasaikiran@gmail.com">📩 Contact Us</a>
</p>

---

## 🌟 Introduction

**SchoolOS AI** is an intelligent academic assessment and learning platform designed to help schools move beyond marks and traditional examination reports.

The platform focuses on transforming assessment results into actionable learning insights. It aims to help educators identify learning gaps, plan targeted revision, conduct follow-up assessments, and understand academic progress through a structured, evidence-driven workflow.

Rather than treating every assessment as an isolated event, SchoolOS AI connects the stages of teaching and learning into a continuous improvement cycle.

### 🎯 Our Mission

To help schools make better academic decisions through meaningful assessment data, focused learning support, and evidence-based progress tracking.

### 💡 Our Vision

A learning environment where every assessment helps educators understand what students have learned, what they need to improve, and what to do next.

---

## 🎯 The SchoolOS AI Learning Cycle

<p align="center">
  <strong>📝 Assess → 🔍 Analyse → 📚 Revise → 🧪 Retest → 📈 Measure</strong>
</p>

| Stage | Description |
|---|---|
| 📝 Assess | Create or manage assessments and capture student performance. |
| 🔍 Analyse | Identify performance patterns, weak topics, and learning gaps from available evidence. |
| 📚 Revise | Focus learning activities on concepts that need additional attention. |
| 🧪 Retest | Evaluate learning through appropriate follow-up assessments. |
| 📈 Measure | Compare recorded results to understand progress and remaining learning needs. |

**The goal is simple: make assessment useful for the next teaching decision, not just the final report.**

---

## 🏫 Designed for the School Community

SchoolOS AI is organised around four important user roles.

### 👨‍💼 1. Principal Workspace

Designed to support school-level academic oversight and planning.

- Review available academic performance information.
- Understand class and subject performance patterns.
- Identify areas requiring additional academic attention.
- Support teacher follow-up and academic planning.
- Review available reports and performance summaries.
- Use recorded evidence to support school-level decisions.

### 👩‍🏫 2. Teacher Workspace

Designed to support the day-to-day assessment and learning improvement workflow.

- Create or manage assessments through supported workflows.
- Enter and review student marks.
- Analyse performance at question and topic levels where supported.
- Identify learning gaps using assessment evidence.
- Plan targeted revision activities.
- Create or manage follow-up assessments where available.
- Compare recorded assessment and retest results.

### 👨‍👩‍👧 3. Parent Workspace

Designed to help parents understand their linked children's academic progress.

- Review available assessment results.
- Understand subject-level performance.
- Follow learning priorities and recorded progress.
- Access reports permitted by the application's authorization rules.
- Support their children's learning with better academic visibility.

### 🎒 4. Student Workspace

Designed to help students understand their own learning needs.

- Review permitted personal academic information.
- Understand areas requiring additional practice.
- Follow revision and retest activities where available.
- Track recorded progress across supported learning workflows.
- Develop a more focused approach to learning and improvement.

*Available actions depend on the implemented features, account permissions, and configured data.*

---

## 🧠 Key Features

### 📊 Academic Assessment and Analysis

SchoolOS AI focuses on structured assessment data and meaningful performance analysis.

- Assessment and marks-management workflows.
- Topic-level learning-gap identification where supported.
- Performance summaries based on available records.
- Evidence-based revision recommendations.
- Comparison of recorded assessment and follow-up results.

### 📚 Targeted Revision

The platform's learning approach connects observed weaknesses to focused practice.

Instead of asking only, “What mark did the student score?”, the goal is to ask:

- Which concept needs attention?
- What evidence supports that conclusion?
- Which revision activity is appropriate?
- Did the follow-up assessment show improvement?
- What should the teacher focus on next?

### 🤖 AI-Assisted Academic Support

AI can support interpretation, explanations, and learning guidance where the corresponding provider and integration are configured.

SchoolOS AI aims to combine AI assistance with reliable application logic. Marks, percentages, rankings, and progress calculations should be derived from actual records and deterministic calculations—not invented by a language model.

### 📈 Academic Progress Tracking

Connecting initial assessments with follow-up assessments can help educators understand:

- Previous performance.
- Identified learning needs.
- Follow-up assessment results.
- Recorded improvement.
- Concepts that still require attention.

Progress claims should always be supported by saved assessment evidence.

### 🎮 SchoolOS Learning Expedition

The Learning Expedition introduces the academic improvement cycle through an interactive educational adventure.

Its mission sequence is designed around four learning stations:

1. **Assessment Lab** — choose an appropriate assessment setup.
2. **Analysis Observatory** — interpret results and identify a learning gap.
3. **Revision Garden** — practise concepts through interactive activities.
4. **Retest Arena** — solve a follow-up challenge and compare results.

The experience uses fictional learning scenarios and is intended to complement—not replace—the core academic application.

### 🔐 Role-Based Academic Access

SchoolOS AI is designed around separate Principal, Teacher, Parent, and Student experiences.

Sensitive academic data must be protected through backend authentication and authorization, including appropriate school, user, and student relationships. Hiding a screen in the frontend alone is not sufficient security.

---

## 🖥️ Technology Stack

The project architecture includes the following technologies.

| Layer | Technology |
|---|---|
| Frontend framework | Next.js |
| UI library | React |
| Frontend language | TypeScript |
| Backend API | Python, FastAPI |
| Current backend database configuration | SQLite |
| Database reference resources | PostgreSQL migration and schema files |
| API communication | HTTP/REST |
| AI integration | Configurable provider integration |
| Backend testing | Python test suite |
| Frontend verification | Typecheck, build, and frontend test scripts |
| Deployment target | Render |

*The presence of a technology or configuration file does not by itself establish that its integration is production-ready. Refer to the current source and deployment configuration for verified details.*

---

## 🏗️ High-Level Architecture

```text
                    SCHOOLOS AI
                         |
             ┌───────────┴───────────┐
             |                       |
        Frontend                 User Roles
     Next.js / React       Principal / Teacher
                           Parent / Student
             |                       |
             └───────────┬───────────┘
                         |
                    Backend API
                      FastAPI
                         |
             ┌───────────┴───────────┐
             |                       |
      Academic Logic            AI Services
             |                       |
             └───────────┬───────────┘
                         |
                    Data Storage
                  SQLite Configuration
```

This is a conceptual architecture diagram. It does not imply that every integration, role workflow, or deployment configuration has been independently verified.

---

## 📂 Project Structure

The repository contains frontend, backend, database-related resources, and tests.

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

*This is a representative structure. Refer to the actual repository version for the complete and authoritative file inventory.*

---

## ⚙️ Getting Started

### Prerequisites

Install the following tools before starting local development:

- Python compatible with the backend requirements.
- Node.js and npm compatible with the frontend dependencies.
- Git.
- An AI provider API key if you intend to test provider-dependent functionality.

### 1. Obtain the Source Code

The source repository is private. To request access, contact:

📩 **chitturidurgasatyasaikiran@gmail.com**

Include your name, organization (if applicable), and the purpose of your request. Repository access is subject to approval.

Once access has been granted, clone the repository:

```bash
git clone https://github.com/Keyrun1227/SchoolOS-AI-Assessment-Agent.git
cd SchoolOS-AI-Assessment-Agent
```

### 2. Set Up the Backend

Create a Python virtual environment:

```bash
python -m venv .venv
```

Activate it.

**Windows:**

```bash
.venv\Scripts\activate
```

**macOS / Linux:**

```bash
source .venv/bin/activate
```

Install the backend dependencies:

```bash
pip install -r backend/requirements.txt
```

Configure the required environment variables using the project's `.env.example` and backend documentation.

**Never commit API keys, passwords, tokens, or production secrets.**

Start the backend using the startup command documented for the current repository version. The FastAPI application entry point is `backend/app/main.py`; confirm the required working directory and environment configuration before launching it.

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

Use the actual backend port configured for your local environment.

Start the frontend development server:

```bash
npm run dev
```

### 4. Open the Application

Open the local URL printed by the Next.js development server.

To access the deployed website, visit:

**🌐 https://schoolos-ai-0z1k.onrender.com/**

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

### Recommended Verification Areas

- Login, logout, and session expiry.
- Role-based and school-level authorization.
- Assessment creation and marks validation.
- Topic analysis and revision recommendations.
- Retest linkage and result comparisons.
- Authorized downloads and rejection of unauthorized requests.
- Database persistence and backup/restore.
- Responsive layouts and keyboard accessibility.
- Learning Expedition mission progression and fictional-data isolation.

Record actual test results for the version being released. Historical results must not be treated as proof that a newer version passes.

---

## 🔒 Security and Privacy

SchoolOS AI is intended to support workflows involving sensitive educational information. Security and privacy must be considered throughout development and deployment.

- Keep API keys and secrets on the server.
- Enforce authorization in backend endpoints.
- Restrict parent access to explicitly linked children.
- Restrict students to their permitted personal records.
- Prevent cross-school data access.
- Protect reports and file downloads.
- Keep public previews and educational game scenarios separate from real school records.
- Avoid including private school data or credentials in source archives.
- Use synthetic data for public demonstrations and isolated tests.
- Verify database backups and recovery procedures.

**Important:** Do not use the platform for real student records until authentication, authorization, data isolation, persistence, and deployment security have been adequately verified.

---

## 🚀 Deployment

The project has a public Render deployment target.

Before deploying an updated version:

1. Preserve the current working release.
2. Review the source changes and environment variables.
3. Run backend tests and the frontend production build.
4. Verify authentication and protected downloads.
5. Test academic workflows using isolated test data.
6. Confirm database persistence and recovery arrangements.
7. Test role-based access and public demo isolation.
8. Deploy through the intended release process.
9. Verify the deployed application and retain a rollback option.

A local source update does not automatically update the live website.

---

## 🗺️ Product Roadmap

The following items represent engineering priorities and verification goals. They should not be interpreted as claims that every item is already complete.

- [ ] Complete end-to-end verification of all four role workflows.
- [ ] Verify authenticated report downloads and export permissions.
- [ ] Verify parent-child and school-level data isolation.
- [ ] Validate the assessment-to-retest cycle against saved records.
- [ ] Complete frontend build and browser regression testing.
- [ ] Validate database backup and restore procedures.
- [ ] Complete verification of all Learning Expedition interactions.
- [ ] Validate deployment configuration and operational monitoring.
- [ ] Improve accessibility and responsive behaviour across workspaces.

---

## 🤝 Contributing

Suggestions, bug reports, and collaboration enquiries are welcome.

For contributions or technical discussions, please contact:

📩 **chitturidurgasatyasaikiran@gmail.com**

If you are granted repository access:

1. Create a feature branch.
2. Make a focused change.
3. Add or update relevant tests.
4. Run the available checks.
5. Document your changes and verification results.
6. Submit a pull request according to the project's contribution process.

Please do not submit secrets, private student data, or production database files.

---

## 📌 Project Status

SchoolOS AI is an evolving education technology project focused on academic assessment, learning-gap analysis, targeted revision, and progress measurement.

Its core objective is to connect assessment results with practical learning actions, helping educators identify what students need to strengthen and evaluate follow-up performance.

The actual readiness of individual features depends on the current implementation and verification results.

**Our long-term vision:** Every assessment should help inform the next learning action.

---

## 🌐 Live Demo & Source Code Access

### 🚀 Explore SchoolOS AI

Experience the platform through our live website:

🔗 **Live Website:** https://schoolos-ai-0z1k.onrender.com/

### 🔒 Private Source Code Repository

The SchoolOS AI source code is maintained in a private GitHub repository and is not publicly accessible.

Access to the source code is available upon request and is subject to approval.

For source code access, technical discussions, project demonstrations, collaboration opportunities, or further information, please contact us by email.

📩 **Email:** [chitturidurgasatyasaikiran@gmail.com](mailto:chitturidurgasatyasaikiran@gmail.com)

Please include your name, organization (if applicable), and purpose of your request.

*Repository access is granted only with the repository owner's approval.*

---

## 👨‍💻 Maintainer and Project Links

- **Project:** SchoolOS AI — Intelligent Academic Assessment & Learning Platform
- **Live Website:** https://schoolos-ai-0z1k.onrender.com/
- **Source Code:** Private GitHub repository
- **GitHub Owner:** [Keyrun1227](https://github.com/Keyrun1227)
- **Contact Email:** [chitturidurgasatyasaikiran@gmail.com](mailto:chitturidurgasatyasaikiran@gmail.com)

---

<p align="center">
  <strong>🎓 SchoolOS AI</strong>
  <br>
  <em>Assess better. Teach smarter. Help every learner progress.</em>
  <br><br>
  🌍 Built to support better academic decisions and more focused learning.
</p>
