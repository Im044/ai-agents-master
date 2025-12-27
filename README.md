# AI Agents Master Repository

🤖 **Complete Collection of Autonomous AI Agents with Docker Support**

Welcome to the master repository for all AI agents! This repository serves as a centralized hub with comprehensive documentation, setup guides, and useful resources for all autonomous AI agents.

## 📚 Table of Contents

- [Overview](#overview)
- [All AI Agents](#all-ai-agents)
- [Quick Start](#quick-start)
- [Setup Instructions](#setup-instructions)
- [Docker Deployment](#docker-deployment)
- [Features](#features)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [Resources](#resources)

## 🎯 Overview

This master repository provides:
- **Complete list of all AI agents** with descriptions and capabilities
- **Docker automation** for containerized deployment
- **Step-by-step setup guides** for beginners
- **Deployment instructions** for production use
- **Configuration templates** for quick setup
- **Best practices** and troubleshooting guides

## 🤖 All AI Agents

### 1. **AI Chatbot LLM** 💬
**Repository:** [ai-chatbot-llm](https://github.com/Im044/ai-chatbot-llm)
- **Purpose:** Advanced conversational AI powered by LLMs
- **Features:** Real-time responses, conversation memory, custom prompts, REST API
- **Port:** 8001
- **Tech Stack:** Python, FastAPI, LangChain
- **Use Cases:** Customer support, automated conversations, Q&A systems

### 2. **AI Data Analyst Agent** 📊
**Repository:** [ai-data-analyst-agent](https://github.com/Im044/ai-data-analyst-agent)
- **Purpose:** Intelligent data analysis and visualization
- **Features:** Data analysis, visualization, insights generation, business intelligence
- **Port:** 8002
- **Tech Stack:** Python, Pandas, Matplotlib, Plotly
- **Use Cases:** Business analytics, data interpretation, report generation

### 3. **AI Research Agent** 🔬
**Repository:** [ai-research-agent](https://github.com/Im044/ai-research-agent)
- **Purpose:** Literature review and research synthesis
- **Features:** Research synthesis, knowledge discovery, RAG, knowledge graphs
- **Port:** 8003
- **Tech Stack:** Python, LLMs, Knowledge Graphs
- **Use Cases:** Research synthesis, knowledge discovery, academic research

### 4. **AI Code Assistant Agent** 💻
**Repository:** [ai-code-assistant-agent](https://github.com/Im044/ai-code-assistant-agent)
- **Purpose:** Intelligent code generation and debugging
- **Features:** Code generation, debugging, refactoring, documentation
- **Port:** 8004
- **Tech Stack:** Python, LLMs, Code Understanding
- **Use Cases:** Code generation, debugging, technical documentation

### 5. **AI Sales & Marketing Agent** 📈
**Repository:** [ai-sales-marketing-agent](https://github.com/Im044/ai-sales-marketing-agent)
- **Purpose:** Lead generation and campaign optimization
- **Features:** Lead generation, engagement, CRM integration, analytics
- **Port:** 8005
- **Tech Stack:** Python, LLMs, CRM APIs
- **Use Cases:** Sales automation, marketing campaigns, lead management

### 6. **AI Content Creator Agent** ✍️
**Repository:** [ai-content-creator-agent](https://github.com/Im044/ai-content-creator-agent)
- **Purpose:** Content generation and optimization
- **Features:** Content creation, optimization, multi-platform, RAG
- **Tech Stack:** Python, LLMs, Content Optimization
- **Use Cases:** Blog writing, social media content, marketing copy

### 7. **AI Image Generator** 🎨
**Repository:** [ai-image-generator](https://github.com/Im044/ai-image-generator)
- **Purpose:** AI-powered image generation
- **Features:** Image generation, style transfer, batch processing, GPU acceleration
- **Tech Stack:** Python, Stable Diffusion, DALL-E
- **Use Cases:** Content creation, design generation, image editing

## 🚀 Quick Start

### Option 1: Using Docker (Recommended)

```bash
# Clone the Docker automation repository
git clone https://github.com/Im044/ai-agents-docker-automation.git
cd ai-agents-docker-automation

# Run the automated setup
bash setup.sh

# All agents will start automatically
```

### Option 2: Individual Agent Setup

```bash
# Clone any agent repository
git clone https://github.com/Im044/ai-chatbot-llm.git
cd ai-chatbot-llm

# Install dependencies
pip install -r requirements.txt

# Run the agent
python main.py
```

## 📋 Setup Instructions

### System Requirements

- **OS:** Windows, macOS, or Linux
- **Python:** 3.9+
- **RAM:** 8GB minimum (16GB recommended)
- **Disk Space:** 20GB for all agents
- **Docker:** Optional but recommended

### Step 1: Install Python & Dependencies

```bash
# Install Python 3.11+
# Windows: Download from python.org
# macOS: brew install python@3.11
# Linux: sudo apt install python3.11

# Verify installation
python --version
```

### Step 2: Install Git

```bash
# Windows: Download from git-scm.com
# macOS: brew install git
# Linux: sudo apt install git
```

### Step 3: Clone This Repository

```bash
git clone https://github.com/Im044/ai-agents-master.git
cd ai-agents-master
```

### Step 4: Clone Individual Agents (if not using Docker)

```bash
# Clone all agents
git clone https://github.com/Im044/ai-chatbot-llm.git
git clone https://github.com/Im044/ai-data-analyst-agent.git
git clone https://github.com/Im044/ai-research-agent.git
git clone https://github.com/Im044/ai-code-assistant-agent.git
git clone https://github.com/Im044/ai-sales-marketing-agent.git
```

## 🐳 Docker Deployment

### Full Deployment (All Agents)

```bash
# Clone Docker automation repo
git clone https://github.com/Im044/ai-agents-docker-automation.git
cd ai-agents-docker-automation

# Run setup script
bash setup.sh

# Check running services
docker-compose ps

# View logs
docker-compose logs -f
```

### Single Agent Deployment

```bash
# Navigate to agent directory
cd ai-chatbot-llm

# Build Docker image
docker build -t ai-chatbot .

# Run container
docker run -p 8001:8001 ai-chatbot
```

### Access Agents

- **Chatbot:** http://localhost:8001
- **Data Analyst:** http://localhost:8002
- **Research Agent:** http://localhost:8003
- **Code Assistant:** http://localhost:8004
- **Sales & Marketing:** http://localhost:8005

## ✨ Features

✅ **Multiple Autonomous Agents** - 7 different AI agents for various tasks
✅ **Docker Support** - Complete containerization for easy deployment
✅ **Automated Setup** - One-command setup script
✅ **Production Ready** - Health checks, security, logging
✅ **Beginner Friendly** - Step-by-step documentation
✅ **Scalable Architecture** - Easily add more agents
✅ **REST APIs** - Easy integration with other systems
✅ **Configuration Files** - Environment-based setup
✅ **Comprehensive Docs** - Detailed guides for each agent

## 📁 Project Structure

```
ai-agents-master/
├── README.md                          # This file
├── SETUP_GUIDE.md                     # Detailed setup guide
├── AGENTS_OVERVIEW.md                 # Detailed agent descriptions
├── DOCKER_GUIDE.md                    # Docker deployment guide
├── API_DOCUMENTATION.md               # API reference
├── TROUBLESHOOTING.md                 # Common issues and solutions
├── CONFIGURATION.md                   # Configuration guide
├── REQUIREMENTS.md                    # System requirements
└── agents/
    ├── chatbot-llm/
    ├── data-analyst/
    ├── research/
    ├── code-assistant/
    ├── sales-marketing/
    ├── content-creator/
    └── image-generator/
```

## 🔧 Configuration

### Environment Variables

Create `.env` file in each agent directory:

```bash
# API Keys
OPENAI_API_KEY=your_key_here
ANTHROPIC_API_KEY=your_key_here

# Database
DATABASE_URL=postgresql://user:pass@localhost/db

# Redis Cache
REDIS_URL=redis://localhost:6379

# Logging
LOG_LEVEL=INFO
LOG_FILE=logs/agent.log
```

## 📖 Documentation

- **[SETUP_GUIDE.md](./SETUP_GUIDE.md)** - Step-by-step installation guide
- **[AGENTS_OVERVIEW.md](./AGENTS_OVERVIEW.md)** - Detailed descriptions of all agents
- **[DOCKER_GUIDE.md](./DOCKER_GUIDE.md)** - Docker deployment instructions
- **[API_DOCUMENTATION.md](./API_DOCUMENTATION.md)** - API reference and examples
- **[TROUBLESHOOTING.md](./TROUBLESHOOTING.md)** - Common issues and solutions
- **[CONFIGURATION.md](./CONFIGURATION.md)** - Configuration options

## 🆘 Troubleshooting

### Port Already in Use

```bash
# Find process using port
lsof -i :8001

# Kill process
kill -9 <PID>
```

### Module Not Found

```bash
# Install dependencies
pip install -r requirements.txt

# Update pip
pip install --upgrade pip
```

### Docker Issues

```bash
# Check Docker status
docker ps

# View logs
docker logs <container_id>

# Rebuild image
docker-compose down
docker-compose build --no-cache
```

## 🤝 Contributing

Contributions are welcome! Please:

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📚 Resources

- **[Official Documentation](./docs)** - Comprehensive guides
- **[API Reference](./API_DOCUMENTATION.md)** - Complete API docs
- **[Examples](./examples)** - Code examples and use cases
- **[FAQ](./FAQ.md)** - Frequently asked questions
- **[Best Practices](./BEST_PRACTICES.md)** - Tips and tricks

## 🔗 Related Repositories

- [ai-agents-docker-automation](https://github.com/Im044/ai-agents-docker-automation) - Docker automation
- [ai-agent-framework](https://github.com/Im044/ai-agent-framework) - Agent framework
- [awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) - LLM resources
- [ai-projects-collection](https://github.com/Im044/ai-projects-collection) - AI and ML projects with complete code
- [ai-games-collection](https://github.com/Im044/ai-games-collection) - AI-powered games using machine learning

## 📝 License

MIT License - Feel free to use this project for personal and commercial use.

## 👨‍💻 Author

**MOHD MUFFASIL**
- GitHub: [@Im044](https://github.com/Im044)
- Email: mdmuffasil893@gmail.com
- LinkedIn: [Profile](https://linkedin.com/in/mohd-muffasil-661191209)

## 📞 Support

Need help? 
- Check [TROUBLESHOOTING.md](./TROUBLESHOOTING.md)
- Open an [Issue](https://github.com/Im044/ai-agents-master/issues)
- Check [FAQ.md](./FAQ.md)

---

**Star ⭐ this repository if you find it helpful!**

*Last Updated: December 2025*
