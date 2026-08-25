# CivicGuardian AI: An Agentic and Service-Oriented Framework for Autonomous Citizen Complaint Management

## Project Title

CivicGuardian AI: An Agentic and Service-Oriented Framework for Autonomous Citizen Complaint Management

## Team Members

| S. No. | Name | Roll Number |
| --- | --- | --- |
| 1 | Shalini . Ch | 2420030284 |
| 2 | M . J . U Harika | 2420030453 |
| 3 | K . Aneesha | 2420030589 |

## Supervisor

Supervisor Name: Dr. Srikanth Cherukuvada

## Abstract

CivicGuardian AI is an intelligent, service-oriented framework engineered to streamline and automate public grievance management. Traditional municipal grievance mechanisms depend on manual triage, siloed legacy interfaces, and static routing, which cause substantial response delays, classification errors, and opaque resolution lifecycles.

CivicGuardian AI transitions municipal triage from passive ticketing into an autonomous agentic pipeline using Large Language Models (OpenAI GPT / Google Gemini) orchestrated via LangChain. The framework automates natural language intent analysis, vector similarity deduplication, severity prioritization, dynamic municipal routing, and real-time SLA-driven escalations to ensure transparent and reliable civic governance.

## Objectives

* Ingest unstructured citizen complaints (text, geolocation, media) through a modern, responsive web interface.
* Automate semantic classification, department tagging, and priority assignment using LLM agents.
* Implement vector similarity matching to identify and cluster duplicate or co-located grievance reports.
* Build a decoupled, high-throughput service layer for secure request processing and status management.
* Provide dynamic SLA tracking, automated escalation pipelines, and real-time citizen status updates.
* Store complaint lifecycles, geospatial coordinates, and audit logs within a scalable NoSQL database.
* Deliver an end-to-end cloud-deployed architecture with automated CI/CD workflows.

## Technologies Used

* Frontend: React.js, Tailwind CSS
* Backend: FastAPI / Spring Boot, REST APIs, JSON Web Tokens (JWT)
* Agentic AI & LLMs: LangChain, OpenAI GPT, Google Gemini
* Database & Vector Store: MongoDB (NoSQL Document Store & Vector Indexing)
* DevOps & Hosting: Git, GitHub Actions, Vercel (Frontend), Render (Backend)
* Development Tools: VS Code, Postman

## Repository Structure


├── .gitignore
├── README.md
│
├── frontend/
│   └── React.js + Tailwind CSS client application
│
├── backend/
│   ├── src/                 # Application source code (FastAPI / Spring Boot)
│   ├── agents/              # LangChain reasoning and routing agents
│   └── config/              # Database and security configurations
│
├── docs/
│   ├── architecture/        # System design and workflow diagrams
│   └── Project documentation
│
├── data/
│   └── Vector database seed schemas and sample mock payloads
│
├── results/
│   └── Model evaluation metrics, routing logs, and test outputs
│
└── reports/
    └── Review reports and final project report

## Setup Instructions

### 1. Clone the Repository


git clone <REPOSITORY_URL>
cd CivicGuardian-AI

### 2. Configure Environment Variables

Create a .env file in the backend root directory (refer to .env.example):


OPENAI_API_KEY=your_openai_api_key
GEMINI_API_KEY=your_gemini_api_key
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key

### 3. Backend Setup

Navigate to the backend directory and install dependencies:


cd backend
pip install -r requirements.txt
python -m uvicorn main:app --reload

### 4. Frontend Setup

Navigate to the frontend directory, install packages, and start the development server:


cd ../frontend
npm install
npm run dev

## System Workflow

1. Multi-Modal Grievance Submission: Citizens submit reports containing text descriptions, media, and geo-coordinates via the React.js portal.
2. Authentication & Ingestion: The service layer validates JWT credentials and sanitizes request payloads.
3. Agentic Reasoning & Deduplication: LangChain agents query the LLM to categorize the grievance, assess severity, and

Shalini:
check MongoDB vector embeddings to cluster duplicate reports.
4. Automated Departmental Dispatch: The system triggers RESTful routing to assign the complaint to the appropriate municipal unit.
5. SLA Monitoring & Escalation: Active background workers track resolution timeframes, send real-time progress updates, and escalate overdue tickets autonomously.

## Current Phase Status

* Current Phase: Review 1
* Status: Project title, problem definition, objectives, architecture design, literature survey, innovation identification, feasibility analysis, and module structuring completed.

## Upcoming Work

* Set up database schemas and vector collections in MongoDB.
* Implement LangChain agent workflows for intent parsing and deduplication.
* Develop REST APIs for ticket state transitions and municipal routing.
* Construct the React.js dashboard with interactive map tagging and status timelines.
* Integrate continuous deployment via GitHub Actions, Vercel, and Render.
* Perform system testing, SLA validation, and prepare Review 2 deliverables.

## Project Deliverables

* Complete project documentation and API specifications
* Source code (Frontend, Backend, and Agentic Pipelines)
* Database schemas and vector configuration scripts
* Evaluation benchmarks (classification accuracy, routing latency)
* Hosted web application (Vercel & Render)
* Review presentations and final project report

## GitHub Contribution Policy

* All team members will contribute using their individual GitHub accounts to ensure transparent verification of work.
* The repository will maintain progressive commits with descriptive messages for all milestones.
* Formal phase releases will be tagged:
* review-1
* review-2
* final



## Important Note

The repository must not contain:

* Passwords, database credentials, or private certificates
* OpenAI, Google Gemini, or third-party API keys
* JWT secret keys
* Private civic or institutional data
* Local build artifacts and temporary cache directories

All private configuration keys must be stored in local .env files and excluded via .gitignore.

## Academic Year

2026–2027
