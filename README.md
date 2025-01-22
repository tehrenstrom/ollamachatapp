# Ollama Chat Desktop

A sleek desktop chat application for interacting with Ollama models, built with Electron and React.

## Features
- 🌓 Dark/Light mode support
- 💻 Native desktop app experience
- ✨ Code syntax highlighting
- 📋 One-click copy for messages and code blocks
- ✍️ Full Markdown support
- 🔒 Secure local execution

## Prerequisites

Before installing Ollama Chat, you need:

1. **Ollama**
   ```bash
   # Visit https://ollama.ai and install Ollama
   # Then pull your preferred model:
   ollama pull llama2
   ```

2. **Start Ollama Server**
   ```bash
   ollama serve
   ```

## Installation

### macOS
1. Download the latest `.dmg` from [Releases](https://github.com/tehrenstrom/ollamachatapp/releases)
2. Open the `.dmg` file
3. Drag Ollama Chat to your Applications folder
4. Launch from Applications

### From Source
```bash
# Clone the repository
git clone https://github.com/tehrenstrom/ollamachatapp.git
cd ollamachatapp

# Install dependencies
npm install

# Run in development mode
npm run electron:dev

# Or build the app
npm run electron:build
```

## Development

### Requirements
- Node.js 18+
- npm 8+
- Ollama installed and running

### Setup
```bash
# Install dependencies
npm install

# Start in development mode
npm run electron:dev
```

### Building
```bash
# Create production build
npm run electron:build
```

## Troubleshooting

### Connection Issues
If you see "Connection Error":
```bash
# Verify Ollama is running
curl http://localhost:11434/api/tags

# If needed, restart Ollama
ollama serve
```

### Model Issues
If the model isn't responding:
1. Check Ollama logs
2. Verify model is downloaded: `ollama list`
3. Try pulling the model again: `ollama pull llama2`

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Built with [Electron](https://www.electronjs.org/)
- Powered by [Ollama](https://ollama.ai)
- UI components by [React](https://reactjs.org/)
