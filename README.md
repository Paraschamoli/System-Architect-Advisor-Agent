<p align="center">
  <img src="https://raw.githubusercontent.com/getbindu/create-bindu-agent/refs/heads/main/assets/light.svg" alt="bindu Logo" width="200">
</p>

<h1 align="center">
  🏗️ System-Architect-Advisor-Agent
</h1>

<p align="center">
  <strong>🤖 AI-Powered System Design Assistant</strong><br>
  Transform natural language requirements into production-ready architecture recommendations
</p>

<p align="center">
  <a href="https://github.com/Paraschamoli/System-Architect-Advisor-Agent/actions/workflows/main.yml?query=branch%3Amain">
    <img src="https://img.shields.io/github/actions/workflow/status/Paraschamoli/System-Architect-Advisor-Agent/main.yml?branch=main" alt="Build status">
  </a>
  <a href="https://img.shields.io/github/license/Paraschamoli/System-Architect-Advisor-Agent">
    <img src="https://img.shields.io/github/license/Paraschamoli/System-Architect-Advisor-Agent" alt="License">
  </a>
  <a href="https://img.shields.io/badge/python-3.12+-blue.svg">
    <img src="https://img.shields.io/badge/python-3.12+-blue.svg" alt="Python 3.12+">
  </a>
  <a href="https://img.shields.io/badge/bindu-framework-orange">
    <img src="https://img.shields.io/badge/bindu-framework-orange" alt="Bindu Framework">
  </a>
</p>

<p align="center">
  <a href="#-quick-start">Quick Start</a> •
  <a href="#-usage">Usage</a> •
  <a href="#-api">API</a> •
  <a href="#-docker">Docker</a> •
  <a href="#-contributing">Contributing</a>
</p>

---

## 📖 Overview

🚀 **System-Architect-Advisor-Agent** is an intelligent system design assistant that transforms natural language project requirements into production-ready architecture recommendations. Built on the [Bindu Agent Framework](https://github.com/getbindu/bindu), it leverages a dual-model reasoning pipeline to deliver comprehensive technical solutions.

### ✨ Key Features

- 🏗️ **System Architecture Design** - Create scalable, maintainable architectures
- 📊 **Infrastructure Planning** - Design cloud infrastructure and deployment strategies
- 🔒 **Security Strategy** - Develop comprehensive security frameworks and compliance plans
- 🗺️ **Implementation Roadmaps** - Generate detailed technical implementation plans
- 📝 **Technical Documentation** - Produce structured architecture documents and specifications

### 🤖 Multi-Model Architecture

| Component | Model | Purpose |
|-----------|--------|---------|
| **Reasoning Engine** | 🧠 DeepSeek R1 | Structured analysis & JSON specification generation |
| **Drafting Engine** | ✍️ Claude 3.5 Sonnet | Professional technical documentation & reports |
| **Memory Integration** | 💾 Mem0 | Contextual conversation history & learning |

---

## 🚀 Quick Start

### 📋 Prerequisites

- **Python 3.12+**
- **[uv](https://github.com/astral-sh/uv)** package manager
- **OpenRouter API Key** (required)
- **Mem0 API Key** (optional, for memory features)

### ⚡ Installation

```bash
# 🍴 Clone the repository
git clone https://github.com/Paraschamoli/System-Architect-Advisor-Agent.git
cd System-Architect-Advisor-Agent

# 📦 Install dependencies using uv
uv sync

# ⚙️ Configure environment
cp .env.example .env
```

### 🔑 Configuration

Edit `.env` and add your API keys:

| Key | Get It From | Required |
|-----|-------------|----------|
| `OPENROUTER_API_KEY` | [OpenRouter](https://openrouter.ai/keys) | ✅ Yes |
| `MEM0_API_KEY` | [Mem0 Dashboard](https://app.mem0.ai/dashboard/api-keys) | ⚪ Optional |

### 🎯 Run the Agent

```bash
# 🚀 Start the agent
uv run python -m system_architect_advisor_agent

# 🌐 Agent will be available at http://localhost:3773
```

### 🐙 GitHub Setup

```bash
# 📝 Initialize git repository and commit your code
git init -b main
git add .
git commit -m "Initial commit"

# 🚀 Create repository on GitHub and push
gf repo create Paraschamoli/System-Architect-Advisor-Agent --public --source=. --remote=origin --push
```

---

## 💡 Usage Examples

### 🎯 Example Queries

```bash
# 🛒 E-commerce Architecture
"Design a microservices architecture for an e-commerce platform handling 1M users daily, with real-time inventory and payment processing"

# 💳 FinTech System
"Create a system design for a fintech payment processing system that must handle PCI compliance and process 10K transactions/second"

# ☁️ Cloud Migration
"Plan the migration strategy for a legacy monolithic application to a cloud-native microservices architecture"

# 💬 Real-time Chat
"Design a real-time chat application with video calling, supporting 100K concurrent users with sub-second latency"
```

### 📝 Input Formats

#### **Plain Text:**
```
Design a scalable architecture for a social media platform with 10M users, real-time messaging, and content recommendation engine
```

#### **JSON:**
```json
{
  "project_type": "e-commerce",
  "scale": "enterprise",
  "users": "1000000",
  "requirements": ["real-time inventory", "payment processing", "recommendations"],
  "constraints": ["PCI compliance", "99.9% uptime", "global deployment"],
  "tech_stack": ["python", "react", "postgresql"]
}
```

### 📤 Output Structure

The agent returns comprehensive output with:

- 🏗️ **Architecture Diagrams** - System overview, component interactions, data flow
- 📋 **Technical Specifications** - API designs, database schemas, service definitions
- 🌐 **Infrastructure Plans** - Cloud deployment, networking, scaling strategies
- 🔒 **Security Framework** - Authentication, authorization, compliance guidelines
- 🗺️ **Implementation Roadmap** - Phased deployment, resource requirements, timelines

---

## 🔌 API Usage

🌐 **RESTful API Endpoint**: `http://localhost:3773`

### 📚 API Documentation

For complete API documentation, request/response formats, and examples:

� **[Bindu API Reference - Send Message to Agent](https://docs.getbindu.com/api-reference/all-the-tasks/send-message-to-agent)**

### 🔗 Additional Resources

- 📖 [Full API Documentation](https://docs.getbindu.com/api-reference/all-the-tasks/send-message-to-agent)
- 📦 [Postman Collections](https://github.com/GetBindu/Bindu/tree/main/postman/collections)
- 🔧 [API Reference](https://docs.getbindu.com)

---

## 🎯 Skills & Capabilities

### 🏗️ System-Architect-Advisor-Agent (v1.0.0)

#### 🎯 Primary Capabilities
- Transform natural language requirements into structured system architecture recommendations
- Generate comprehensive infrastructure planning and security strategies
- Create detailed implementation roadmaps and technical documentation

#### ⭐ Key Features
- **🔄 Multi-Pattern Architecture** - Microservices, serverless, event-driven, DDD designs
- **☁️ Cloud-Agnostic Planning** - AWS, Azure, GCP, and multi-cloud strategies
- **🔒 Security-First Design** - Authentication, authorization, encryption, compliance frameworks
- **📈 Scalability Analysis** - Performance modeling and capacity planning
- **📚 Technical Documentation** - Architecture Decision Records (ADRs), API specs, deployment guides

#### 🎯 Best Use Cases
- **🚀 Startup Architecture Planning** - MVP design and technology stack selection
- **🏢 Enterprise Modernization** - System modernization and cloud migration strategies
- **🔍 Technical Due Diligence** - Architecture review processes
- **👥 Team Training** - Architectural best practices dissemination

#### ⚠️ Limitations
- Provides recommendations, not actual implementation
- Requires clear and detailed requirements
- Cannot access proprietary internal systems
- Recommendations based on general best practices

#### 📊 Performance Metrics
| Metric | Value |
|--------|-------|
| **Processing Time** | ~30-90 seconds per architecture design |
| **Concurrent Requests** | 10 |
| **Memory per Request** | ~512MB |
| **Supported Scales** | Startup to Enterprise level |
| **Reasoning Model** | deepseek/deepseek-r1 |
| **Drafting Model** | anthropic/claude-3.5-sonnet |

---

## 🐳 Docker Deployment

### 🏠 Local Docker Setup

```bash
# 🐳 Build and run with Docker Compose
docker-compose up --build

# 🌐 Agent will be available at http://localhost:3773
```

### ⚙️ Docker Configuration

The agent runs on port `3773` and requires:
- 🔑 `OPENROUTER_API_KEY` environment variable
- 💾 `MEM0_API_KEY` environment variable

> **💡 Tip**: Configure these in your `.env` file before running.

### 🚀 Production Deployment

```bash
# 🏭 Use production compose file
docker-compose -f docker-compose.prod.yml up -d
```

---

## 🌐 Deploy to bindus.directory
------------------------------

🌍 **Make your agent discoverable worldwide and enable agent-to-agent collaboration.**

### 🔐 Setup GitHub Secrets

```bash
# 🔑 Authenticate with GitHub
gf auth login

# 🔐 Set deployment secrets
gf secret set BINDU_API_TOKEN --body "<your-bindu-api-key>"
gf secret set DOCKERHUB_TOKEN --body "<your-dockerhub-token>"
```

#### 📍 Get Your Keys:
- **🔑 Bindu API Key**: [bindus.directory](https://bindus.directory) dashboard
- **🐳 Docker Hub Token**: [Docker Hub Security Settings](https://hub.docker.com/settings/security)

### 🚀 Deploy

```bash
# 📤 Push to trigger automatic deployment
git push origin main
```

#### 🔄 GitHub Actions will automatically:
1. 🔨 Build your agent
2. 🐳 Create Docker container
3. 📤 Push to Docker Hub
4. 🌐 Register on bindus.directory

---

## 🛠️ Development
--------------

### 📁 Project Structure

```
System-Architect-Advisor-Agent/
├── 📦 system_architect_advisor_agent/
│   ├── 🎯 skills/
│   │   └── 🏗️ system_architect_advisor_agent/
│   │       ├── 📋 skill.yaml          # Skill configuration
│   │       └── 📄 __init__.py
│   ├── 📄 __init__.py
│   ├── 🚀 __main__.py
│   ├── 💻 main.py                     # Agent entry point
│   └── ⚙️ agent_config.json           # Agent configuration
├── 🧪 tests/
│   └── 📄 test_main.py
├── 📝 .env.example
├── 🐳 docker-compose.yml
├── 🐳 Dockerfile.agent
└── 📦 pyproject.toml
```

### 🧪 Running Tests

```bash
make test              # 🧪 Run all tests
make test-cov          # 📊 With coverage report
```

### ✨ Code Quality

```bash
make format            # 🎨 Format code with ruff
make lint              # 🔍 Run linters
make check             # ✅ Format + lint + type check + test
```

### 🪝 Pre-commit Hooks

```bash
# 🔧 Install pre-commit hooks
uv run pre-commit install

# 🔨 Run manually
uv run pre-commit run -a
```

### 🔄 Development Workflow

```bash
# 1️⃣ Make your changes
git add .

# 2️⃣ Run quality checks (automatically runs pre-commit hooks)
make check

# 3️⃣ Run tests
make test

# 4️⃣ Commit your changes
git commit -m "feat: add amazing feature"

# 5️⃣ Push to trigger CI/CD
git push origin main
```

---

## 🤝 Contributing

🎉 **Contributions are welcome!** Please follow these steps:

1. 🍴 **Fork the repository**
2. 🌿 **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. 📝 **Commit your changes**: `git commit -m 'Add amazing feature'`
4. 📤 **Push to the branch**: `git push origin feature/amazing-feature`
5. 🔃 **Open a Pull Request**

📖 See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

---

## 📄 License

📜 This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Powered by Bindu

🚀 **Built with the [Bindu Agent Framework](https://github.com/getbindu/bindu)**

### ✨ Why Bindu?
- 🌐 **Internet of Agents** - A2A, AP2, X402 protocols for agent collaboration
- ⚡ **Zero-config setup** - From idea to production in minutes
- 🛠️ **Production-ready** - Built-in deployment, monitoring, and scaling

### 🚀 Build Your Own Agent
```bash
uvx cookiecutter https://github.com/getbindu/create-bindu-agent.git
```

---

## 📚 Resources

- 📖 [Full Documentation](https://Paraschamoli.github.io/System-Architect-Advisor-Agent/)
- 💻 [GitHub Repository](https://github.com/Paraschamoli/System-Architect-Advisor-Agent/)
- 🐛 [Report Issues](https://github.com/Paraschamoli/System-Architect-Advisor-Agent/issues)
- 💬 [Join Discord](https://discord.gg/3w5zuYUuwt)
- 🌐 [Agent Directory](https://bindus.directory)
- 📚 [Bindu Documentation](https://docs.getbindu.com)

---

<p align="center">
  <strong>🌷 Built with 💛 by the team from Amsterdam</strong>
</p>

<p align="center">
  <a href="https://github.com/Paraschamoli/System-Architect-Advisor-Agent">⭐ Star this repo</a> •
  <a href="https://discord.gg/3w5zuYUuwt">💬 Join Discord</a> •
  <a href="https://bindus.directory">🌐 Agent Directory</a>
</p>

#   S y s t e m - A r c h i t e c t - A d v i s o r - A g e n t 
 
 
