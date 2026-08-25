# CivicGuardian AI: An Agentic and Service-Oriented Framework for Autonomous Citizen Complaint Management

## Project Title

**CivicGuardian AI: An Agentic and Service-Oriented Framework for Autonomous Citizen Complaint Management**

## Team Members

| S. No. | Name            | Roll Number |
| ------ | --------------- | ----------- |
| 1      | Shalini Ch.     | 2420030284  |
| 2      | M. J. U. Harika | 2420030453  |
| 3      | K. Aneesha      | 2420030589  |

## Supervisor

**Dr. Srikanth Cherukuvada**

## Abstract

CivicGuardian AI is an intelligent, service-oriented framework designed to streamline and automate public grievance management. Traditional municipal grievance mechanisms depend on manual triage, siloed legacy interfaces, and static routing, resulting in response delays, classification errors, and limited visibility into the resolution lifecycle.

CivicGuardian AI transforms municipal grievance management from passive ticketing into an autonomous agentic pipeline using Large Language Models (OpenAI GPT / Google Gemini) orchestrated through LangChain. The framework automates natural language intent analysis, vector similarity-based deduplication, severity prioritization, dynamic municipal routing, and real-time SLA-driven escalation to support transparent and reliable civic governance.

## Objectives

* Ingest unstructured citizen complaints including text, geolocation, and media through a modern, responsive web interface.
* Automate semantic classification, department tagging, and priority assignment using LLM-based agents.
* Implement vector similarity matching to identify and cluster duplicate or co-located grievance reports.
* Build a decoupled, high-throughput service layer for secure request processing and complaint status management.
* Provide dynamic SLA tracking, automated escalation pipelines, and real-time citizen status updates.
* Store complaint lifecycles, geospatial coordinates, and audit logs within a scalable NoSQL database.
* Deliver an end-to-end cloud-deployed architecture with automated CI/CD workflows.

## Technologies Used

* **Frontend:** React.js, Tailwind CSS
* **Backend:** FastAPI / Spring Boot, REST APIs, JSON Web Tokens (JWT)
* **Agentic AI & LLMs:** LangChain, OpenAI GPT, Google Gemini
* **Database & Vector Store:** MongoDB with NoSQL document storage and vector indexing
* **DevOps & Hosting:** Git, GitHub Actions, Vercel, Render
* **Development Tools:** VS Code, Postman

## Repository Structure

```text
CivicGuardian-AI/
│
├── .gitignore
├── README.md
│
├── frontend/
│   └── React.js + Tailwind CSS client application
│
├── backend/
│   ├── src/                 # Application source code
│   ├── agents/              # LangChain reasoning and routing agents
│   └── config/              # Database and security configurations
│
├── docs/
│   ├── architecture/        # System design and workflow diagrams
│   └── project-docs/        # Project documentation
│
├── data/
│   └── sample-data/         # Sample payloads and database seed data
│
├── results/
│   └── evaluation/         # Model evaluation metrics and test outputs
│
└── reports/
    └── final-report/        # Review reports and final project report
```

## Setup Instructions

### 1. Clone the Repository

```bash
git clone <REPOSITORY_URL>
cd CivicGuardian-AI
```

### 2. Configure Environment Variables

Create a `.env` file in the backend directory using `.env.example` as a reference.

```env
OPENAI_API_KEY=your_openai_api_key
GEMINI_API_KEY=your_gemini_api_key
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
```

> **Note:** Never commit `.env` files or API keys to the repository.

### 3. Backend Setup

Navigate to the backend directory and install the required dependencies:

```bash
cd backend
pip install -r requirements.txt
python -m uvicorn main:app --reload
```

### 4. Frontend Setup

Open a new terminal, navigate to the frontend directory, install the required packages, and start the development server:

```bash
cd frontend
npm install
npm run dev
```

## System Workflow

1. **Multi-Modal Grievance Submission:** Citizens submit complaints containing text descriptions, media, and geographical coordinates through the React.js portal.
2. **Authentication & Ingestion:** The service layer validates JWT credentials and sanitizes incoming request data.
3. **Agentic Reasoning & Deduplication:** LangChain agents use LLM-based reasoning to categorize grievances, assess severity, and identify duplicate reports using MongoDB vector embeddings.
4. **Automated Departmental Dispatch:** RESTful services dynamically route complaints to the appropriate municipal department.
5. **SLA Monitoring & Escalation:** Background workers monitor resolution timelines, provide progress updates, and automatically escalate overdue complaints.

## Current Phase Status

* **Current Phase:** Review 1
* **Status:** Project title, problem definition, objectives, architecture design, literature survey, innovation identification, feasibility analysis, and module structuring completed.

## Upcoming Work

* Set up database schemas and vector collections in MongoDB.
* Implement LangChain agent workflows for intent parsing and duplicate detection.
* Develop REST APIs for complaint state transitions and municipal routing.
* Construct the React.js dashboard with interactive map tagging and status timelines.
* Integrate continuous deployment using GitHub Actions, Vercel, and Render.
* Perform system testing and SLA validation.
* Prepare Review 2 deliverables.

## Project Deliverables

* Complete project documentation and API specifications
* Frontend, backend, and agentic pipeline source code
* Database schemas and vector configuration scripts
* Evaluation benchmarks including classification accuracy and routing latency
* Hosted web application using Vercel and Render
* Review presentations and final project report

## GitHub Contribution Policy

* All team members will contribute using their individual GitHub accounts to ensure transparent verification of work.
* The repository will maintain progressive commits with descriptive messages for project milestones.
* Formal project phases will be tagged as:

```text
review-1
review-2
final
```

## Important Note

The repository must **not** contain:

* Passwords
* Database credentials
* Private certificates
* OpenAI, Google Gemini, or third-party API keys
* JWT secret keys
* Private civic or institutional data
* Local build artifacts
* Temporary cache directories

All private configuration keys must be stored in local `.env` files and excluded using `.gitignore`.

## Academic Year

**2026–2027**
