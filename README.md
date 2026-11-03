# My Personal AI — AURA

A free-first personal AI starter with an expressive holographic face, spoken responses, browser voice input, customizable personality, local SQLite memories, and a coding helper.

## Run locally
Requires Python 3.10+ and optionally Ollama (https://ollama.com).

1. Create a virtual environment: python -m venv .venv
2. Activate it: source .venv/bin/activate (Windows: .venv\\Scripts\\Activate.ps1)
3. Install dependencies: pip install -r requirements.txt
4. Copy .env.example to .env.
5. Install a local model: ollama pull llama3.2
6. Start Ollama, then run: uvicorn backend.main:app --reload
7. Open http://127.0.0.1:8000

Without Ollama, the interface still loads and explains how to connect a model. No paid API key is required.

## Features
- Animated cyan holographic face with mood expressions and mouth movement while speech synthesis is playing.
- Browser speech input/output when supported.
- Local conversation history and user-controlled SQLite memories.
- Editable personality settings.
- Chat and coding modes; coding suggestions are not automatically executed.
- Responsive dark UI.

## Hologram reality check
This is a stylized animated 2D holographic interface. It can be displayed on a monitor or used with a physical Pepper's Ghost reflector. Software alone cannot make an image float in empty air; a physical illusion needs suitable display and reflector hardware.

## Privacy and safety
Data is stored locally by default. Do not expose the server to the public internet without authentication and HTTPS. The coding helper does not run shell commands or silently change files.

Configuration: OLLAMA_URL, OLLAMA_MODEL, DATABASE_PATH, ASSISTANT_NAME.
