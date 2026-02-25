# 2_Environment 🛠 — The \"Context\"

## 🗺️ Roadmaps
1. **macOS**: Native brew install → Ollama Docker → Qdrant Docker → Crush config
2. **Windows**: WSL2/Ubuntu → brew equivalent (scoop/winget) → Docker Desktop → Crush

## ⚙️ Constraints
- API keys required for cloud models
- Docker Desktop license on Win (free for personal)
- Terminal: iTerm2 (Mac), Windows Terminal/WSL
- Hardware: &gt;16GB RAM for local models

## 📖 Setup Guides

### macOS
1. Install Homebrew if missing: `/bin/bash -c \"$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)\"`
2. `brew install charmbracelet/tap/crush`
3. Docker: `brew install --cask docker`
4. Ollama: `brew install --cask ollama`

### Windows
1. Install WSL2: `wsl --install -d Ubuntu`
2. In WSL: Install scoop/winget crush
3. Docker Desktop from MS Store
4. Ollama via exe or Docker

### AI Clients (Ollama/Claude)
- Ollama: `ollama serve`, `ollama pull llama3`
- Claude: API key in env

**Next:** Detailed steps in 4_Formula. 🔄