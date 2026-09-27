# El Pana IA

Web PWA + proxy FastAPI (Max AI) + RAG semántico + voz + Telegram + herramientas.

## Repo
https://github.com/klkmax/el-pana-ia

## Netlify (front estático)
Proyecto: https://app.netlify.com/projects/el-pana-ia  
URL: https://el-pana-ia.netlify.app  
(Sube la carpeta `pana-ia` o el ZIP en Deploys.)

## Local
```bash
# Front
cd pana-ia && python3 -m http.server 8080

# Proxy
cd pana-ia/backend
pip install -r requirements.txt
export AGENT_TOKEN=secreto
uvicorn max_ai_proxy:app --host 0.0.0.0 --port 8000

# Telegram (opcional)
export TELEGRAM_BOT_TOKEN=...
export AUTHORIZED_USER_ID=...
python telegram_bot.py
```

## Features
- Chat streaming + Max AI
- RAG híbrido (léxico + embeddings)
- Voz (mic + TTS)
- Web search + sandbox Python
- Telegram
