# 🔧 OpsRunbook AI
**Powered by LangGraph + OpenAI**


> **Turn chaotic incidents into a deterministic runbook flow. Classify incidents, retrieve runbooks, generate mitigation steps, and summarize risk—all in one view, in seconds.** ⚡

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Next.js](https://img.shields.io/badge/Next.js-16-black.svg)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.2-61DAFB.svg)](https://react.dev/)
[![LangGraph](https://img.shields.io/badge/LangGraph-AI_Agents-purple.svg)](https://langchain-ai.github.io/langgraph/)
[![Railway](https://img.shields.io/badge/Deploy-Railway-blueviolet.svg)](https://railway.app/)

---

## ✨ What It Does

OpsRunbook AI is an intelligent incident response assistant that uses a **deterministic LangGraph workflow** to:

1. **Classify Incidents** — Automatically categorize by type, severity, and affected services using GPT-4.1
2. **Retrieve Runbooks** — Fetch relevant runbooks and procedures from your knowledge base
3. **Generate Mitigation** — Create step-by-step actionable mitigation plans with verification criteria
4. **Assess Risk** — Produce comprehensive risk analysis covering blast radius and business impact
5. **Draft Status Updates** — Generate professional, customer-facing status page updates

All in a single, beautiful interface with real-time pipeline visualization.

---

## 🎯 Core Features

### 🤖 **AI-Powered Incident Response**
- **Real OpenAI Integration** — GPT-4.1-mini for intelligent, contextual analysis
- **Deterministic Workflow** — LangGraph orchestrates 5 sequential nodes
- **Structured Output** — Consistent, parseable results every time
- **Context-Aware** — Incorporates runbooks and previous context

### 📊 **Rich Pipeline Visualization**
- **Graph Visualization** — Animated flow diagram showing pipeline execution
- **Step-by-Step Progress** — Watch each node complete with live updates
- **Severity Badges** — Color-coded incident severity with pulse animations
- **Live Typing Animation** — Streaming AI responses character-by-character

### 🎨 **Modern UI/UX (2025 Standards)**
- **Single-Page Architecture** — Smooth state-driven transitions
- **Dark/Light Mode** — Beautiful theme with system preference support
- **Mobile-First** — Responsive design with 44px+ touch targets
- **Micro-Animations** — Delightful interactions throughout

### 📱 **Enterprise Feature Set**
| Feature | Description |
|---------|-------------|
| 🎯 **Incident Classification** | Type, severity, service, region detection |
| 📈 **Risk Assessment** | Blast radius, business & technical impact |
| 🔧 **Mitigation Steps** | Numbered, actionable steps with verification |
| 📋 **Status Updates** | Professional customer-facing drafts |
| 🎤 **Voice Input** | Speak your incident description |
| 📄 **Export Options** | PDF, Markdown, JSON report downloads |
| 🔔 **Sound Effects** | Optional audio feedback |
| 📊 **Analytics Dashboard** | Track incident patterns and response times |
| 🔗 **Webhook Integration** | Connect to Slack, PagerDuty, and more |
| 👥 **Collaboration** | Real-time session sharing |
| 📚 **Incident Templates** | Pre-built scenarios for common incidents |
| 🌐 **Multi-Language** | 6 languages supported (EN, ES, FR, DE, PT, JA) |
| 📝 **Runbook Editor** | Create and manage custom runbooks |
| 🔌 **System Status** | Real-time service connectivity monitoring |

---

## 🏗️ Tech Stack

### **Frontend** ⚛️
| Technology | Purpose |
|------------|---------|
| **Next.js 16** | React 19.2 with App Router |
| **TypeScript** | Type-safe development |
| **Tailwind CSS** | Utility-first styling |
| **shadcn/ui** | Beautiful component library |
| **Lucide Icons** | Modern icon set |
| **next-themes** | Dark/Light mode |

### **Backend** 🐍
| Technology | Purpose |
|------------|---------|
| **FastAPI** | High-performance Python API |
| **LangGraph** | Multi-agent AI orchestration |
| **OpenAI GPT-4.1** | Intelligent analysis |
| **Pydantic** | Data validation |

### **Data & Cache** 💾
| Technology | Purpose |
|------------|---------|
| **Supabase** | PostgreSQL persistence |
| **Upstash Redis** | Job queue & caching |

### **Deployment** 🚀
| Platform | Service |
|----------|---------|
| **Vercel** | Frontend hosting |
| **Railway** | Backend API |

---

## 🔄 How It Works

```
┌─────────────────────────────────────────────────────────────┐
│                    INCIDENT INPUT                           │
│         Description + Context + Affected Services           │
└─────────────────────┬───────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│                 LANGGRAPH WORKFLOW                          │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐      │
│  │  Classifier  │  │   Runbook    │  │  Mitigation  │      │
│  │    Node      │──│   Fetcher    │──│  Generator   │      │
│  │  (OpenAI)    │  │  (Supabase)  │  │  (OpenAI)    │      │
│  └──────────────┘  └──────────────┘  └──────┬───────┘      │
│                                             │               │
│            ┌───────────────┐       ┌────────▼────────┐      │
│            │    Status     │◀──────│     Risk        │      │
│            │   Updater     │       │    Summary      │      │
│            │   (OpenAI)    │       │   (OpenAI)      │      │
│            └───────────────┘       └─────────────────┘      │
└─────────────────────────────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│                       OUTPUT                                │
│  • Classification (Type, Severity, Service, Region)         │
│  • Mitigation Steps (Numbered, actionable, verified)        │
│  • Risk Assessment (Blast radius, impact, stakeholders)     │
│  • Status Update (Professional, customer-facing draft)      │
└─────────────────────────────────────────────────────────────┘
```

---

## 📖 User Guide

### Getting Started

1. **Enter Incident Description** — Describe the incident with service name, symptoms, error rates
2. **Optional: Use Voice Input** — Click the microphone to speak your description
3. **Optional: Use Templates** — Select from pre-built incident scenarios
4. **Run Pipeline** — Watch the AI analyze and process your incident
5. **Review Results** — Classification, mitigation steps, risk assessment, status update
6. **Export Results** — Download as PDF, Markdown, or JSON

### Understanding Your Results

| Section | What It Shows |
|---------|---------------|
| **Classification** | Incident type, severity level, affected service, region |
| **Mitigation Steps** | Numbered actions with verification criteria |
| **Risk Assessment** | Blast radius, business impact, technical impact, recommendations |
| **Status Update** | Professional, customer-facing communication draft |

### Pro Tips

- **Be specific** with error codes, metrics, and affected regions
- **Include context** like recent deployments or changes
- **Use templates** for common incident patterns
- **Export reports** for post-incident reviews
- **Check System Status** to verify all services are connected

---

## 🎨 Customization

### Theme Options
- ☀️ **Light Mode** — Clean, professional interface
- 🌙 **Dark Mode** — Default theme, easy on the eyes
- 🖥️ **System** — Follows OS preference

### Language Support
- 🇺🇸 English
- 🇪🇸 Español
- 🇫🇷 Français
- 🇩🇪 Deutsch
- 🇧🇷 Português
- 🇯🇵 日本語

---

## 📊 Performance

| Metric | Value |
|--------|-------|
| Analysis Time | ~15-25 seconds |
| First Contentful Paint | < 1.5s |
| Lighthouse Score | 85+ |
| Mobile Ready | ✅ Yes |
| PWA Ready | ✅ Yes |

---

## 🛡️ Security

- ✅ Backend-only Supabase access (schema not exposed)
- ✅ RPC functions for secure database operations
- ✅ API rate limiting
- ✅ CORS protection for API endpoints
- ✅ Environment variables for all secrets
- ✅ Input validation with Pydantic

---

## 👨‍💻 Creator

**Derril Filemon**

[![GitHub](https://img.shields.io/badge/GitHub-derril--tech-181717?logo=github)](https://github.com/derril-tech)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin)](https://www.linkedin.com/in/derril-filemon-a31715319)

This project demonstrates proficiency in:
- 🤖 **AI/ML Integration** — LangGraph multi-agent workflows, OpenAI GPT-4.1
- ⚛️ **Modern React** — Next.js 16, React 19.2, Server Components
- 🐍 **Python Backend** — FastAPI, async/await, Pydantic
- 🎨 **UI/UX Design** — Responsive design, animations, accessibility
- ☁️ **Cloud Architecture** — Supabase, Redis, Railway, Vercel
- 🔧 **DevOps** — CI/CD, environment management, monitoring
- 📱 **Mobile Development** — Mobile-first responsive design
- 🌐 **Internationalization** — Multi-language support

---

## 🙏 Acknowledgments

- **[LangGraph](https://langchain-ai.github.io/langgraph/)** — Multi-agent orchestration
- **[OpenAI](https://openai.com/)** — GPT-4.1-mini API
- **[Supabase](https://supabase.com/)** — Database & auth
- **[Upstash](https://upstash.com/)** — Redis caching
- **[Railway](https://railway.app/)** — Backend deployment
- **[Vercel](https://vercel.com/)** — Frontend hosting
- **[shadcn/ui](https://ui.shadcn.com/)** — Beautiful components
- **[Lucide](https://lucide.dev/)** — Icon library

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

**⭐ Star this repo if you find it useful!**

Made with ❤️ and ☕ by [Derril Filemon](https://github.com/derril-tech)

</div>
