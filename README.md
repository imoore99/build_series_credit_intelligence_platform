# Credit Intelligence Platform

An enterprise-grade AI system for credit risk analysis combining Retrieval-Augmented Generation (RAG), Model Context Protocol (MCP), and multi-agent orchestration.

[Live Demo](your-railway-url) | [Documentation](docs/) | [Tutorial Series](notebooks/)

## 🎯 What It Does

Automates credit memo generation by orchestrating multiple AI agents that:
- Research borrower financials via MCP tools
- Retrieve relevant credit policies via RAG
- Analyze risk factors systematically
- Generate structured credit recommendations
- Maintain audit trails and citations

**Demo:** Upload borrower info → Get complete credit memo in 30 seconds

## 🏗️ Architecture
```
User Input
    ↓
Streamlit Interface
    ↓
Multi-Agent Orchestrator
    ↓
├─→ Research Agent (MCP) → Financial data APIs
├─→ Analysis Agent (RAG) → Credit policies
├─→ Risk Agent → Systematic evaluation
└─→ Writer Agent → Structured memo
    ↓
Credit Memo Output
```

## 🚀 Quick Start

### Production Deployment
```bash
# Clone repository
git clone https://github.com/yourusername/credit-intelligence-platform.git
cd credit-intelligence-platform

# Install dependencies
pip install -r requirements.txt

# Configure environment
cp .env.example .env
# Add your API keys

# Run the application
streamlit run app/main.py
```

### Docker Deployment
```bash
docker build -t credit-intelligence .
docker run -p 8501:8501 --env-file .env credit-intelligence
```

### Railway Deployment

[![Deploy on Railway](https://railway.app/button.svg)](your-railway-template)

## 📚 Learning Path

Want to understand how this was built? Follow the [10-part tutorial series](notebooks/) that documents the complete build process from first API call to production deployment.

## 🛠️ Tech Stack

- **AI/ML:** Claude Sonnet 4.5, LangChain, Hugging Face Transformers
- **RAG:** ChromaDB, Sentence Transformers
- **MCP:** Custom tools for financial data integration
- **Frontend:** Streamlit
- **Deployment:** Railway, Docker
- **Language:** Python 3.11+

## 📊 System Capabilities

- **Document Processing:** Ingests credit policies, research reports, historical memos
- **Live Data:** Connects to financial APIs for real-time data
- **Multi-Agent:** Orchestrates 4 specialized agents
- **Structured Output:** Consistent JSON schema for downstream systems
- **Cost Tracking:** Built-in token usage monitoring
- **Audit Trail:** Full citation tracking and decision logging

## 🎬 Demo

[Include GIF or video showing the system in action]

## 📖 Documentation

- [Architecture Overview](docs/architecture.md)
- [Deployment Guide](docs/deployment.md)
- [API Reference](docs/api_reference.md)
- [Tutorial Series](notebooks/)

## 🧪 Testing
```bash
# Run test suite
pytest tests/

# Run with coverage
pytest --cov=src tests/
```

## 📈 Performance

- **Average analysis time:** 25-30 seconds
- **Token usage:** ~8,000 tokens per analysis
- **Cost per analysis:** ~$0.15
- **Accuracy:** Benchmarked against 100 historical credit decisions (metrics in docs/)

## 🔐 Security

- API keys managed via environment variables
- No sensitive data in version control
- Input validation on all user inputs
- Rate limiting on API calls

## 💰 Cost Estimate

**Development:** ~$15 over 10 months  
**Production:** ~$0.15 per credit analysis  
**Monthly (100 analyses):** ~$15

## 🤝 Contributing

This is a learning project documented publicly. See [notebooks/](notebooks/) for the complete build process.

## 📬 Contact

**Ian Moore**  
Analytics Manager | Credit Risk + AI  
[LinkedIn](link) | [Medium](link) | [Portfolio](link)

## 📝 License

MIT License - See [LICENSE](LICENSE) for details

---

**Built publicly over 10 months (Jan - Oct 2026)**  
Documented in a [10-part blog series](link) on Medium