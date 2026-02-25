# 4_Formula 📋 — The \"Recipe\"

## 🧪 Step-by-Step Guides

### 1. Install Crush
**macOS:**
```bash
brew install charmbracelet/tap/crush
crush
```

**Windows (WSL):**
```bash
curl -fsSL https://raw.githubusercontent.com/charmbracelet/scoop-bucket/main/bucket/charm.json | scoop install
# or winget install charmbracelet.crush
```

### 2. Ollama + Qdrant Docker Compose
Create `docker-compose.yml`:
```yaml
services:
  ollama:
    image: ollama/ollama
    ports:
      - 11434:11434
  qdrant:
    image: qdrant/qdrant
    ports:
      - 6333:6333
    volumes:
      - qdrant_storage:/qdrant/storage

volumes:
  qdrant_storage:
```
`docker compose up -d`

### 3. Crush Config with Local
Edit `~/.config/crush/crush.json`:
```json
{
  \"providers\": {
    \"ollama\": {
      \"base-url\": \"http://localhost:11434\"
    }
  }
}
```

**Embeddings:** nomic-embed-text via Ollama.

## 🔗 Containerized Setup
See `5_Symbols/docker-compose.yml`