
<!-- CAPSULE-RENDER HEADER -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,50:2d2d44,100:3d3d5c&fontColor=6b7280&descColor=4b5563&height=220&section=header&text=Agentic%20AI%20System&fontSize=55&desc=Legacy+Multi-Agent+System+(Archived)&animation=fadeIn" />

<!-- ARCHIVED WARNING BANNER -->
<div align="center">

> ### ⚠️ THIS PROJECT IS ARCHIVED ⚠️
> **This repository is no longer maintained.** It is preserved for historical reference only.
> For the actively developed successor, see **[AI-MultiColony-Ecosystem](https://github.com/mulkymalikuldhrs/AI-MultiColony-Ecosystem)**.

<br/>

![ARCHIVED](https://img.shields.io/badge/STATUS-ARCHIVED-6b7280?style=for-the-badge&labelColor=374151&color=6b7280)
![NO LONGER MAINTAINED](https://img.shields.io/badge/NO%20LONGER-MAINTAINED-991b1b?style=for-the-badge&labelColor=450a0a)
![SEE AI-MULTICOLONY](https://img.shields.io/badge/SUCCESSOR-AI--MultiColony--Ecosystem-7c3aed?style=for-the-badge&labelColor=3b0764)

</div>

<!-- TYPING SVG -->
<div align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3000&pause=1000&color=6B7280&center=true&vCenter=true&width=600&lines=Archived+%7C+Legacy+Project;Python+%2B+Flask+Multi-Agent+System;Superseded+by+AI-MultiColony-Ecosystem;Preserved+for+Reference+Only" alt="Typing SVG" />
  </a>
</div>

<br/>

<!-- BADGES -->
<div align="center">

[![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org/)
[![Flask](https://img.shields.io/badge/Flask-3.x-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![Archived](https://img.shields.io/badge/Status-Archived-64748B?style=for-the-badge)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](./LICENSE)

</div>

---

> **This project is ARCHIVED.** It is no longer maintained and is preserved for historical reference only. For the current, actively developed version, see [AI-MultiColony-Ecosystem](https://github.com/mulkymalikuldhrs/AI-MultiColony-Ecosystem).

---

## Overview

**Agentic AI System** is a **legacy, archived** multi-agent AI system built with Python and Flask. This was an earlier iteration of a multi-agent architecture that has since been superseded by the [AI-MultiColony-Ecosystem](https://github.com/mulkymalikuldhrs/AI-MultiColony-Ecosystem) project.

This repository is preserved for reference, historical context, and educational purposes. It is **no longer actively maintained**.

---

## Visual Architecture

### 1. Legacy Architecture - Original Simple Multi-Agent Flow

```mermaid
graph TB
    subgraph LEGACY["Agentic AI System - Legacy Architecture"]
        direction TB

        subgraph WEB["Web Layer"]
            FlaskApp["Flask Server<br/>:5000"]
            WSHandler["WebSocket Handler<br/>Real-time Events"]
            Templates["Jinja2 Templates<br/>Dashboard / Agents / Workflows"]
        end

        subgraph AGENT["Agent Layer"]
            Coordinator["Agent Coordinator<br/>Task Distribution"]
            BaseAgent["Base Agent Class<br/>Lifecycle Management"]
            Specialist["Specialist Agents<br/>Configurable Behaviors"]
            Profiles["Agent Profiles<br/>JSON Configuration"]
        end

        subgraph CORE["Core Engine"]
            Memory["Memory Manager<br/>In-Memory State"]
            Planning["Planning Engine<br/>Task Decomposition"]
            Comms["Communication Protocol<br/>Inter-Agent Messaging"]
            Tools["Tool/Function Framework<br/>Agent Actions"]
        end

        subgraph DATA["Data"]
            Config["Config Files<br/>YAML / JSON"]
            Sessions["Session State<br/>In-Memory Only"]
        end
    end

    FlaskApp --> Coordinator
    WSHandler --> Coordinator
    Templates --> FlaskApp

    Coordinator --> BaseAgent
    Coordinator --> Specialist
    BaseAgent --> Profiles

    BaseAgent --> Memory
    BaseAgent --> Planning
    BaseAgent --> Comms
    Specialist --> Tools

    Coordinator --> Config
    Coordinator --> Sessions

    style FlaskApp fill:#374151,stroke:#6b7280,color:#9ca3af
    style Coordinator fill:#374151,stroke:#6b7280,color:#9ca3af
    style BaseAgent fill:#374151,stroke:#6b7280,color:#9ca3af
    style Memory fill:#7f1d1d,stroke:#dc2626,color:#fca5a5
    style Sessions fill:#7f1d1d,stroke:#dc2626,color:#fca5a5
```

### 2. Migration Path - How This Evolved into AI-MultiColony-Ecosystem

```mermaid
flowchart LR
    subgraph PHASE1["Phase 1 - Agentic AI System"]
        Flask["Flask<br/>Monolith"]
        SimpleAgents["Simple<br/>Agent Profiles"]
        InMemory["In-Memory<br/>State"]
        BasicWS["Basic<br/>WebSocket"]
        TaskQ["Simple<br/>Task Queue"]
    end

    subgraph PHASE2["Phase 2 - Transition"]
        Migration["Migration<br/>Period"]
        DesignReview["Architecture<br/>Review"]
        RequirementScale["Scaling<br/>Requirements"]
    end

    subgraph PHASE3["Phase 3 - AI-MultiColony-Ecosystem"]
        FastAPI["FastAPI<br/>Async"]
        ColonyAgents["Colony-Based<br/>Agents"]
        Postgres["PostgreSQL<br/>+ Redis"]
        FullWS["Full Real-Time<br/>Event System"]
        SkillEngine["Skill<br/>Engine"]
        MultiLLM["Multi-LLM<br/>9 Providers"]
        Docker["Docker<br/>Compose"]
    end

    Flask --> Migration
    SimpleAgents --> Migration
    InMemory --> Migration
    BasicWS --> Migration
    TaskQ --> Migration

    Migration --> DesignReview
    DesignReview --> RequirementScale

    RequirementScale --> FastAPI
    RequirementScale --> ColonyAgents
    RequirementScale --> Postgres
    RequirementScale --> FullWS
    RequirementScale --> SkillEngine
    RequirementScale --> MultiLLM
    RequirementScale --> Docker

    style Flask fill:#374151,stroke:#6b7280,color:#9ca3af
    style SimpleAgents fill:#374151,stroke:#6b7280,color:#9ca3af
    style InMemory fill:#374151,stroke:#6b7280,color:#9ca3af
    style BasicWS fill:#374151,stroke:#6b7280,color:#9ca3af
    style TaskQ fill:#374151,stroke:#6b7280,color:#9ca3af

    style FastAPI fill:#065f46,stroke:#10b981,color:#fff
    style ColonyAgents fill:#065f46,stroke:#10b981,color:#fff
    style Postgres fill:#065f46,stroke:#10b981,color:#fff
    style FullWS fill:#065f46,stroke:#10b981,color:#fff
    style SkillEngine fill:#065f46,stroke:#10b981,color:#fff
    style MultiLLM fill:#065f46,stroke:#10b981,color:#fff
    style Docker fill:#065f46,stroke:#10b981,color:#fff

    style Migration fill:#92400e,stroke:#f59e0b,color:#fff
    style DesignReview fill:#92400e,stroke:#f59e0b,color:#fff
    style RequirementScale fill:#92400e,stroke:#f59e0b,color:#fff
```

### 3. Comparison - Old vs New Architecture Side by Side

```mermaid
graph TB
    subgraph OLD_SYS["Agentic AI System - OLD"]
        direction TB
        OldFlask["Flask Server<br/>Synchronous"]
        OldAgents["Flat Agent List<br/>No Colony Concept"]
        OldMemory["In-Memory Only<br/>Lost on Restart"]
        OldWS["Basic WebSocket<br/>No Event System"]
        OldLLM["Single LLM<br/>No Fallback"]
        OldDeploy["Manual Deploy<br/>No Containerization"]
        OldScale["Single Process<br/>No Scaling"]
        OldState["Session-Based<br/>No Persistence"]
    end

    subgraph NEW_SYS["AI-MultiColony-Ecosystem - NEW"]
        direction TB
        NewFast["FastAPI + Next.js 16<br/>Async + Modern UI"]
        NewColony["Colony-Based Agents<br/>Specialized Roles"]
        NewPersist["PostgreSQL + Redis<br/>Persistent State"]
        NewEvents["Full Event System<br/>Real-time Updates"]
        NewLLM["9-Provider LLM Router<br/>Priority Fallback"]
        NewDocker["Docker Compose<br/>Nginx + Monitoring"]
        NewScale["Multi-Container<br/>Horizontally Scalable"]
        NewAudit["Full Audit Trail<br/>Decision Provenance"]
    end

    OldFlask -.->|"Replaced by"| NewFast
    OldAgents -.->|"Evolved into"| NewColony
    OldMemory -.->|"Upgraded to"| NewPersist
    OldWS -.->|"Replaced by"| NewEvents
    OldLLM -.->|"Expanded to"| NewLLM
    OldDeploy -.->|"Upgraded to"| NewDocker
    OldScale -.->|"Solved by"| NewScale
    OldState -.->|"Replaced by"| NewAudit

    style OldFlask fill:#374151,stroke:#6b7280,color:#9ca3af
    style OldAgents fill:#374151,stroke:#6b7280,color:#9ca3af
    style OldMemory fill:#7f1d1d,stroke:#dc2626,color:#fca5a5
    style OldWS fill:#374151,stroke:#6b7280,color:#9ca3af
    style OldLLM fill:#374151,stroke:#6b7280,color:#9ca3af
    style OldDeploy fill:#374151,stroke:#6b7280,color:#9ca3af
    style OldScale fill:#7f1d1d,stroke:#dc2626,color:#fca5a5
    style OldState fill:#7f1d1d,stroke:#dc2626,color:#fca5a5

    style NewFast fill:#065f46,stroke:#10b981,color:#fff
    style NewColony fill:#065f46,stroke:#10b981,color:#fff
    style NewPersist fill:#065f46,stroke:#10b981,color:#fff
    style NewEvents fill:#065f46,stroke:#10b981,color:#fff
    style NewLLM fill:#065f46,stroke:#10b981,color:#fff
    style NewDocker fill:#065f46,stroke:#10b981,color:#fff
    style NewScale fill:#065f46,stroke:#10b981,color:#fff
    style NewAudit fill:#065f46,stroke:#10b981,color:#fff
```

---

## Features (Historical)

### Multi-Agent Architecture
- Multiple specialized agents with distinct roles and capabilities
- Agent communication protocol for inter-agent messaging
- Task distribution and coordination engine
- Basic agent lifecycle management (spawn, execute, terminate)

### Flask API Server
- RESTful API for agent interaction and control
- WebSocket support for real-time agent communication
- Authentication and session management
- Admin dashboard for monitoring agent activity

### Agent Capabilities
- Configurable agent behaviors via JSON profiles
- Tool/function calling framework for agent actions
- Memory and context management per agent
- Basic planning and task decomposition

---

## Honest Notes

> **Before you explore this codebase:**

- **Archived/Legacy** — This project is archived and no longer maintained. It may contain outdated dependencies, known bugs, and architectural decisions that have been improved upon in later projects.
- **See AI-MultiColony-Ecosystem Instead** — The concepts and architecture from this project have been evolved and significantly improved in the [AI-MultiColony-Ecosystem](https://github.com/mulkymalikuldhrs/AI-MultiColony-Ecosystem). For active development, use that project instead.
- **Not Production Ready** — Even in its active period, this was a research prototype. Do not use this for production systems.
- **Dependencies May Be Outdated** — Python packages and Flask extensions referenced may have newer versions with breaking changes. Pin versions if you need to run this.
- **No Security Audits** — This code was never audited for security. Do not expose the Flask server to the internet.

---

## Quick Start (For Reference Only)

### Prerequisites
- Python 3.11+
- pip

### Installation

```bash
git clone https://github.com/mulkymalikuldhrs/Agentic-AI-System_OLD.git
cd Agentic-AI-System_OLD
pip install -r requirements.txt  # May require version pinning
```

### Running

```bash
python app.py
```

The Flask server will start at `http://localhost:5000`.

---

## Project Structure

```
Agentic-AI-System_OLD/
├── app.py               # Flask application entry point
├── agents/
│   ├── base.py          # Base agent class
│   ├── coordinator.py   # Agent coordination logic
│   ├── specialist/      # Specialized agent implementations
│   └── profiles/        # Agent configuration profiles
├── api/
│   ├── routes/          # API endpoint definitions
│   └── websocket.py     # WebSocket handler
├── core/
│   ├── memory/          # Agent memory management
│   ├── planning/        # Task planning engine
│   └── communication/   # Inter-agent messaging
├── config/              # Configuration files
└── tests/               # Test suites (may be incomplete)
```

---

## Migration Guide

If you're looking to build on the concepts from this project, here's how the architecture evolved:

| Agentic AI System (OLD) | AI-MultiColony-Ecosystem |
|--------------------------|--------------------------|
| Single Flask server | Modular microservices (FastAPI + Next.js) |
| Basic agent profiles | Colony-based agent ecosystems |
| Simple task queue | Advanced orchestration engine |
| In-memory agent state | Persistent state (PostgreSQL + Redis) |
| Basic WebSocket | Full real-time event system |
| Single LLM provider | 9-provider LLM router with fallback |
| No containerization | Docker Compose + Nginx |
| No monitoring | Prometheus + Grafana |
| Session-based auth | Proper auth + audit trails |

---

## Contributing

This project is **archived and not accepting contributions**. Please direct all efforts to the [AI-MultiColony-Ecosystem](https://github.com/mulkymalikuldhrs/AI-MultiColony-Ecosystem) instead.

---

## Disclaimer

This is archived legacy code preserved for reference. It is not maintained, may contain security vulnerabilities, and should not be used in production. For the current version of this concept, see [AI-MultiColony-Ecosystem](https://github.com/mulkymalikuldhrs/AI-MultiColony-Ecosystem).

---

## License

**MIT License** — see [LICENSE](./LICENSE) for details.

---

## Author

<div align="center">

**Mulky Malikul Dhaher**

[![GitHub](https://img.shields.io/badge/GitHub-mulkymalikuldhrs-181717?style=flat-square&logo=github)](https://github.com/mulkymalikuldhrs)
[![Email](https://img.shields.io/badge/Email-mulkymalikudhr@mail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:mulkymalikudhr@mail.com)

</div>

---

<!-- FOOTER BANNER -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,50:2d2d44,100:3d3d5c&fontColor=6b7280&descColor=4b5563&height=120&section=footer&text=&fontSize=0" />
