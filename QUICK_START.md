# Quick Start Guide - AI Agents Master

## 🚀 Get Started in 5 Minutes

This guide will help you get up and running with AI Agents in just 5 minutes!

### Prerequisites

- Git installed
- Docker installed (recommended) or Python 3.9+
- Internet connection

### Option 1: Docker (Fastest - Recommended)

```bash
# Step 1: Clone the Docker automation repo
git clone https://github.com/Im044/ai-agents-docker-automation.git
cd ai-agents-docker-automation

# Step 2: Run setup (this will install everything and start all agents)
bash setup.sh

# Step 3: Wait 2-3 minutes for services to start

# Step 4: Access agents:
# Chatbot: http://localhost:8001
# Data Analyst: http://localhost:8002
# Research: http://localhost:8003
# Code Assistant: http://localhost:8004
# Sales/Marketing: http://localhost:8005
```

### Option 2: Python Direct (No Docker)

```bash
# Step 1: Clone individual agent
git clone https://github.com/Im044/ai-chatbot-llm.git
cd ai-chatbot-llm

# Step 2: Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Step 3: Install dependencies
pip install -r requirements.txt

# Step 4: Run agent
python main.py

# Step 5: Access at http://localhost:8001
```

### Option 3: Clone All Agents

```bash
# Clone all agents at once
for repo in ai-chatbot-llm ai-data-analyst-agent ai-research-agent ai-code-assistant-agent ai-sales-marketing-agent; do
  git clone https://github.com/Im044/"$repo".git
done

# Install and run each (in separate terminals)
cd ai-chatbot-llm && pip install -r requirements.txt && python main.py
cd ai-data-analyst-agent && pip install -r requirements.txt && python main.py
# ... and so on
```

## ✨ Next Steps

1. **Explore Agents**: Visit http://localhost:8001-8005
2. **Read Documentation**: Check [README.md](./README.md)
3. **Try Examples**: Look at agent-specific examples
4. **Configure**: Set up `.env` files with your API keys
5. **Integrate**: Use REST APIs in your application

## 🆘 Common Issues

### Port Already in Use
```bash
# Windows
netstat -ano | findstr :8001
taskkill /PID <PID> /F

# Linux/Mac
lsof -i :8001
kill -9 <PID>
```

### Module Not Found
```bash
pip install --upgrade pip
pip install -r requirements.txt --force-reinstall
```

### Docker Issues
```bash
docker-compose down
docker-compose build --no-cache
docker-compose up -d
```

## 📚 Learn More

- **[Detailed Setup Guide](./SETUP_GUIDE.md)** - In-depth installation
- **[Agent Details](./AGENTS_DETAILED.md)** - Learn about each agent
- **[Docker Guide](./DOCKER_GUIDE.md)** - Docker deployment
- **[Troubleshooting](./TROUBLESHOOTING.md)** - Common problems

## 💡 Tips

- Docker is the easiest way to get started
- Each agent runs on a different port
- Default port range: 8001-8005
- Check logs for any errors: `docker-compose logs -f`
- Use `.env` files for configuration

Happy coding! 🚀
