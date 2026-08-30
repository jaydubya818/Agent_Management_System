# 🚀 AMS (Agent Management System)

## 🎯 Project Overview

AMS (Agent Management System) is a comprehensive B2B SaaS platform designed to be the definitive command and control layer for enterprise AI agent fleet management. This repository contains both the **AMS platform codebase** and a sophisticated collection of **134+ specialized AI development agents** for collaborative software development.

### 🏗️ Dual-Purpose Repository

1. **🏢 AMS Platform**: Enterprise agent fleet management and observability platform
2. **🤖 AI Agent Collection**: 134+ specialized development agents with multi-agent orchestration

> **Looking for just the subagents?** The maintained, standalone collection lives in
> **[governed-claude-subagents](https://github.com/jaydubya818/governed-claude-subagents)**
> — 116 subagents for Claude Code, installable on their own with no platform attached.
> This repository is the platform; the agents bundled here exist to exercise it.

## 📁 Repository Structure

```
/backend                    # FastAPI backend service
  /api                     # API endpoints and routing
  /core                    # Core business logic
  /models                  # Database models and schemas
  /services                # Business services and integrations
  /tests                   # Backend tests
/frontend                  # React TypeScript frontend
  /src                     # Source code
  /public                  # Static assets
/infra                     # Infrastructure and deployment
  /docker                  # Docker configurations
  /k8s                     # Kubernetes manifests
  /terraform               # Infrastructure as Code
/docs                      # Documentation
  /api                     # API documentation
  /architecture            # System architecture docs
  /deployment              # Deployment guides
/Open-SWE-With-Agents/     # 134+ AI Development Agents Collection
  /development/            # 24 Development & Architecture agents
  /quality/                # 15 Quality Assurance & Testing agents
  /devops/                 # 13 DevOps & Infrastructure agents
  /product/                # 9 Product & Business agents
  /design/                 # 7 Design & User Experience agents
  /marketing/              # 7 Marketing & Growth agents
  /documentation/          # 6 Documentation & Communication agents
  /orchestration/          # 5 Orchestration & Management agents
  /operations/             # 5 Operations agents
  /data-ai/                # 4 Data & AI Engineering agents
  /security/               # 4 Security & Compliance agents
  /specialized/            # 9 Specialized & Utility agents
/.taskmaster/              # Task Master AI project management
```

## Development Setup

1. **Prerequisites**
   - Node.js 18+ 
   - Python 3.11+
   - Docker and Docker Compose
   - PostgreSQL 15+
   - Redis 7+

2. **Quick Start**
   ```bash
   # Clone the repository
   git clone https://github.com/jaydubya818/Agent_Management_System.git
   cd Agent_Management_System
   
   # Start development environment
   docker-compose up -d
   
   # Backend setup
   cd backend
   pip install -r requirements.txt
   python main.py
   
   # Frontend setup (new terminal)
   cd frontend
   npm install
   npm run dev
   ```

3. **Environment Variables**
   Copy `.env.example` to `.env` and configure:
   ```bash
   # Database
   DATABASE_URL=postgresql://user:pass@localhost:5432/ams_dev
   
   # Redis
   REDIS_URL=redis://localhost:6379
   
   # JWT
   JWT_SECRET_KEY=your-secret-key
   
   # External APIs
   ANTHROPIC_API_KEY=your-anthropic-key
   OPENAI_API_KEY=your-openai-key
   ```

## Features

### Core Observability & Command Center
- Fleet Command Dashboard with agent heatmap
- Distributed Trace Explorer for agent execution paths
- Real-time alerting engine with webhook integration
- AI briefings for daily/weekly fleet summaries

### Agent Lifecycle Management
- First-class agent identity and profile management
- Champion/Challenger A/B testing framework
- Automated canary deployments and rollbacks
- Agent lifecycle automation and deprecation recommendations

### Governance & Safety
- Policy engine for spend caps and action controls
- Immutable audit trail for all agent actions
- Role-based access control (RBAC)
- Emergency stop functionality for fleet-wide control

### FinOps & Optimization
- Meta-Agent for autonomous cost optimization
- Model performance analysis and recommendations
- Self-healing capabilities for common errors
- Automated A/B testing for cost optimization

### Developer Platform
- Python SDK for LangGraph agent integration
- OAuth-based integrations (Jira, GitHub, Slack)
- Public REST API for programmatic control
- Comprehensive documentation and examples

## Technology Stack

- **Backend**: FastAPI, SQLAlchemy, Celery, Redis
- **Frontend**: React, TypeScript, Tailwind CSS, Chart.js
- **Database**: PostgreSQL, ClickHouse (events/logs)
- **Infrastructure**: Docker, Kubernetes, AWS/GCP
- **Observability**: OpenTelemetry, LangSmith
- **Agent Framework**: LangGraph

## Development Workflow

This project uses [Task Master AI](https://github.com/TaskMaster-AI/TaskMaster) for project management:

```bash
# View current tasks
tm list

# See next task to work on
tm next

# View specific task details
tm show <task-id>

# Update task progress
tm update-subtask --id=<subtask-id> --prompt="Progress update"

# Mark tasks complete
tm set-status --id=<task-id> --status=done
```

## Contributing

1. Check the current sprint tasks with `tm list`
2. Pick up the next available task with `tm next`
3. Create a feature branch from main
4. Implement the task following the detailed requirements
5. Update task progress using Task Master AI
6. Submit a pull request with comprehensive testing

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤖 AI Development Agents Collection

This repository includes a comprehensive collection of **134+ specialized AI agents** designed for collaborative software development. Each agent is a domain specialist with standardized communication protocols, enabling seamless collaboration across complex development workflows.

### 📊 Agent Categories & Capabilities

| Category | Count | Purpose | Key Agents |
|----------|-------|---------|------------|
| 🎯 **Orchestration & Management** | 5 | Project coordination and multi-agent management | `agent-organizer`, `context-manager`, `tech-lead-orchestrator` |
| 🏗️ **Development & Architecture** | 24 | Software development, frameworks, and system design | `react-pro`, `backend-architect`, `python-pro`, `nextjs-pro` |
| 🎨 **Design & User Experience** | 7 | UI/UX design, visual systems, and user research | `ui-designer`, `ux-designer`, `brand-guardian` |
| 🔧 **Quality Assurance & Testing** | 15 | Code review, testing, performance optimization | `code-reviewer`, `test-automator`, `qa-expert` |
| 🔒 **Security & Compliance** | 4 | Security auditing, compliance, incident response | `security-auditor`, `incident-responder` |
| 📊 **Data & AI Engineering** | 4 | Data pipelines, machine learning, AI systems | `data-engineer`, `ml-engineer`, `prompt-engineer` |
| ☁️ **DevOps & Infrastructure** | 13 | Cloud architecture, deployment, infrastructure | `cloud-architect`, `deployment-engineer` |
| 📝 **Documentation & Communication** | 6 | Technical writing, API docs, content creation | `api-documenter`, `documentation-expert` |
| 🎯 **Product & Business** | 9 | Product management, sprint coordination, analytics | `ai-scrum-master`, `product-manager` |
| 📈 **Marketing & Growth** | 7 | Growth hacking, social media, content strategy | `growth-hacker`, `marketing-writer` |
| 🏢 **Operations** | 5 | Analytics, finance, legal compliance, support | `analytics-reporter`, `finance-tracker` |
| 🎭 **Specialized & Utility** | 9 | Specialized tools, workflow optimization | `workflow-optimizer`, `tool-evaluator` |

### 🌟 Featured Agent Capabilities

#### 🎯 **Master Orchestration**
- **`agent-organizer`**: Master orchestrator for complex, multi-agent tasks with intelligent delegation
- **`context-manager`**: Central nervous system for agent coordination and project state awareness
- **`ai-scrum-master`**: Automated Scrum Master with 3-hour standup cycles and continuous sprint management

#### 🏗️ **Development Specialists**
- **`react-pro`**: Expert React developer with modern patterns, performance optimization, and testing
- **`backend-architect`**: System design, API architecture, database design, and scalability
- **`python-pro`**: Expert Python developer for backend and data applications with clean architecture
- **`nextjs-pro`**: Next.js specialist for full-stack React applications with SSR/SSG optimization

#### 🔒 **Security & Quality**
- **`security-auditor`**: Senior application security auditor with penetration testing capabilities
- **`code-reviewer`**: Expert code review specialist with quality assessment and security review
- **`performance-engineer`**: Application performance optimization with bottleneck identification

#### ☁️ **Infrastructure & DevOps**
- **`cloud-architect`**: Multi-cloud architecture with cost optimization and security design
- **`deployment-engineer`**: CI/CD pipeline and deployment automation with Kubernetes orchestration

### 🔄 Agent Communication Protocol

All agents follow a standardized three-phase communication protocol:

1. **Context Acquisition**: Query `context-manager` for project state
2. **Solution Implementation**: Execute specialized tasks
3. **Activity Reporting**: Report completion back to context-manager

### 🚀 Agent Usage Examples

#### Single Agent Invocation
```bash
@react-pro Create a responsive dashboard component with real-time data
@security-auditor Audit authentication system for vulnerabilities
@cloud-architect Design scalable AWS infrastructure for microservices
```

#### Multi-Agent Orchestration
```bash
@agent-organizer Build a complete e-commerce platform with payment integration
# Automatically selects and coordinates: backend-architect, react-pro, security-auditor, api-documenter
```

#### Continuous Sprint Management
```bash
@ai-scrum-master Set up automated sprint management for development team
# Establishes 3-hour standup cycles with sub-agent coordination
```

### 🛠️ Agent Setup & Configuration

#### Quick Setup
```bash
# Navigate to agents directory
cd Open-SWE-With-Agents

# Run setup script
./setup_claude_agents.sh

# Optimize agents
./optimize_agents.sh

# Validate setup
./.claude/validate_agents.sh
```

#### Agent Integration
- **MCP Servers**: context7, magic, sequential-thinking, playwright
- **Development Tools**: Git, Docker, testing frameworks
- **Cloud Platforms**: AWS, Azure, GCP
- **Communication**: Slack, Teams, Discord

For detailed agent specifications and capabilities, see [Open-SWE-With-Agents/AGENTS_DETAILED_README.md](Open-SWE-With-Agents/AGENTS_DETAILED_README.md).

## Contact

- **Project Lead**: [Your Name](mailto:your.email@example.com)
- **GitHub**: [Agent Management System](https://github.com/jaydubya818/Agent_Management_System)
- **Task Management**: Powered by Task Master AI
- **AI Agents**: 134+ specialized development agents included
