# El Pana IA — Web PWA + Proxy Max AI

Agente conversacional dominicano (jerga / español neutro) + conexión a **Max AI** vía proxy FastAPI seguro.

## Ver en vivo

- Repo: https://github.com/klkmax/el-pana-ia
- Local: `python3 -m http.server 8080` en esta carpeta

## Estructura

```
pana-ia/
├── index.html, css/, js/, sw.js, manifest.json, icons/
└── backend/
    ├── max_ai_proxy.py
    ├── requirements.txt
    └── README.md
```

## Backend

```bash
cd backend
pip install -r requirements.txt
export AGENT_TOKEN="secreto"
export MAX_AI_URL="http://127.0.0.1:11434"
uvicorn max_ai_proxy:app --host 0.0.0.0 --port 8000
```
