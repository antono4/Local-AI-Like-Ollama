# NeuralChat Web - AI Chat Interface

A beautiful, free AI chat interface that runs entirely in your browser. No server needed!

🌐 **Live Demo**: https://antono4.github.io/Local-AI-Like-Ollama/

## ✨ Features

- 🤖 **Multiple AI Providers** - OpenAI, Claude, Groq, Cohere, Gemini, or Local Ollama
- 💬 **Beautiful UI** - Dark futuristic theme with smooth animations
- 💾 **Auto-save** - Conversations saved locally in your browser
- ⚙️ **Customizable** - Temperature, max tokens, system prompt
- 📱 **Responsive** - Works on desktop, tablet, and mobile
- 🔒 **Privacy First** - API keys stored locally in your browser

## 🚀 Getting Started

### 1. Open the Web Version

Visit: **https://antono4.github.io/Local-AI-Like-Ollama/**

### 2. Select AI Provider

Choose from these providers:

| Provider | Models | Free Tier |
|----------|--------|-----------|
| **OpenAI** | GPT-4o, GPT-4o-mini, GPT-3.5 | ❌ Paid |
| **Claude** | Opus, Sonnet, Haiku | ❌ Paid |
| **Groq** | Llama, Mixtral, Gemma | ✅ Free (limited) |
| **Cohere** | Command R+, Command | ✅ Free tier |
| **Gemini** | Gemini 2.0, 1.5 | ✅ Free |
| **Local** | Any Ollama model | ✅ Free (needs Ollama) |

### 3. Get API Key

#### Free Options:

**Groq** (Recommended - Fast & Free):
1. Go to https://console.groq.com/
2. Sign up for free
3. Get your API key
4. Enter in NeuralChat

**Gemini** (Generous Free Tier):
1. Go to https://aistudio.google.com/
2. Sign in with Google
3. Get free API key
4. Enter in NeuralChat

**Cohere** (Free Trial):
1. Go to https://dashboard.cohere.com/
2. Sign up for free
3. Get trial API key

#### Paid Options:

**OpenAI**:
- https://platform.openai.com/api-keys

**Claude**:
- https://console.anthropic.com/

### 4. Start Chatting!

Select a model, enter your API key, and start chatting!

## 📁 Project Structure

```
/
├── index.html          # Main app (runs in browser)
├── README.md          # This file
└── SPEC.md            # Design specification

# For local Ollama version, see parent directory
```

## 🔧 Local Development

To run locally:

```bash
# Simply open index.html in your browser
# Or use a local server:
python -m http.server 8000
# Then visit http://localhost:8000
```

## 💡 Tips

### Groq (Fastest Free Option)
- Uses Llama 3.1 models
- Very fast inference
- Great for development/testing

### Gemini (Most Generous)
- 1.5 million free tokens/month
- Supports long contexts
- Great value

### Local Ollama
- Completely free
- Runs on your computer
- No data leaves your machine
- Install Ollama, download models, and select "Local" provider

## 📝 License

MIT License - Free to use and modify.

---

Made with ❤️ using Vanilla JS