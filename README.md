# NeuralChat - Local AI Chat Interface

A local AI chat interface that runs in the browser, connected to Ollama.

![NeuralChat Preview](https://img.shields.io/badge/Status-Active-success)
![Python](https://img.shields.io/badge/Python-3.8+-blue)
![Flask](https://img.shields.io/badge/Flask-3.0-green)

## ✨ Features

- 🎨 **Futuristic Design** - Dark interface with cyan accents, glow effects, and smooth animations
- 🔄 **Streaming Response** - Watch AI responses appear in real-time
- 💬 **Markdown Support** - Format code, bold, italic with syntax highlighting
- ⚙️ **Flexible Settings** - Temperature, max tokens, system prompt
- 💾 **Auto-save** - Conversations saved to localStorage
- 📱 **Responsive** - Supports desktop, tablet, and mobile

## 🚀 Installation & Run

### 1. Install Ollama

**macOS/Linux:**
```bash
curl -fsSL https://ollama.com/install.sh | sh
```

**Windows:**
Download from https://ollama.com/download

### 2. Download AI Model

After installing Ollama, download the desired model:

```bash
# Light model (2GB) - for low-spec computers
ollama pull llama3.2:1b

# Medium model (4GB) - balanced performance
ollama pull llama3.2

# Large model (8GB) - best performance
ollama pull llama3.2:3b

# Other available models
ollama pull mistral
ollama pull codellama
ollama pull phi3
ollama pull gemma2
```

### 3. Run NeuralChat

```bash
# Install dependencies
pip install -r requirements.txt

# Start server
python app.py
```

### 4. Open in Browser

Open http://localhost:5000 in your browser.

## 📁 Project Structure

```
/workspace/project/
├── app.py              # Flask backend (Ollama API proxy)
├── index.html          # Frontend (HTML/CSS/JS)
├── requirements.txt    # Python dependencies
├── README.md           # Documentation
└── SPEC.md             # Design specification
```

## ⚙️ Settings

| Setting | Default | Description |
|---------|---------|-------------|
| Temperature | 0.7 | 0 = deterministic, 2 = random/creative |
| Max Tokens | 2048 | Maximum response length |
| System Prompt | - | Instructions for AI persona |
| Stream Response | On | Show responses in real-time |

## 🔧 Troubleshooting

### "Cannot connect to Ollama"

1. Make sure Ollama is running: `ollama serve`
2. Check if Ollama is listening on port 11434: `curl http://localhost:11434`
3. Make sure the model is downloaded: `ollama list`

### Server startup error

```bash
# If port 5000 is already in use
# Edit app.py and change port:
app.run(host="0.0.0.0", port=5001, ...)

# Or kill the process using that port
lsof -ti:5000 | xargs kill -9
```

### Model doesn't appear in dropdown

1. Make sure the model is downloaded: `ollama pull llama3.2`
2. Restart NeuralChat server
3. Refresh browser

## 🎯 Usage Tips

1. **Choose Model** - Use smaller models for simple tasks, larger models for complex tasks
2. **Adjust Temperature** - Lower to 0.3-0.5 for more consistent answers, raise to 1.0-1.5 for creativity
3. **Custom System Prompt** - Change AI personality as needed
4. **Clear Chat** - Trash button to start a new conversation

## 📝 License

MIT License - Free to use and modify.

---

Made with ❤️ using Flask + Vanilla JS