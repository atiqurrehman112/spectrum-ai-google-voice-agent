# Spectrum AI Google Voice Agent

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Inter&weight=700&size=28&duration=2800&pause=700&color=0EA5E9&center=true&vCenter=true&width=900&lines=Realtime+AI+Google+Voice+Automation;Live+STT+%2B+LLM+%2B+TTS+Calling+Agent;FastAPI+Dashboard+%2B+Windows+Desktop+App;Built+for+24%2F7+Outbound+Calling+Workflows" alt="Typing SVG" />

<br><br>

<img src="https://komarev.com/ghpvc/?username=atiqurrehman112&label=Repository%20Views&color=0ea5e9&style=for-the-badge" />
<img src="https://img.shields.io/github/stars/atiqurrehman112/spectrum-ai-google-voice-agent?style=for-the-badge&color=22c55e" />
<img src="https://img.shields.io/github/forks/atiqurrehman112/spectrum-ai-google-voice-agent?style=for-the-badge&color=f59e0b" />
<img src="https://img.shields.io/github/license/atiqurrehman112/spectrum-ai-google-voice-agent?style=for-the-badge&color=64748b" />

<br><br>

<img src="https://skillicons.dev/icons?i=python,fastapi,selenium,js,html,css,powershell,githubactions,windows,git,vscode" />

<br><br>

### Realtime AI-powered outbound calling automation using Google Voice, Selenium, Groq, STT, TTS, FastAPI, and Windows desktop deployment.

</div>

---

# Overview

Spectrum AI Google Voice Agent is a realtime AI outbound calling system that transforms Google Voice into an AI-powered dispatch and sales automation platform.

The project combines:

* Google Voice browser automation
* Realtime speech recognition
* AI-generated responses
* Text-to-speech playback
* Voicemail detection
* CRM logging
* FastAPI dashboard
* Windows desktop deployment

Everything works together as a practical outbound calling workflow capable of long-running automated operations.

---

# Features

* Realtime AI outbound calling
* Google Voice browser automation
* Selenium DOM control
* FastAPI operator dashboard
* Realtime speech-to-text
* AI-generated voice replies
* Voicemail detection system
* Automated CRM logging
* Call recordings & transcripts
* Persistent Chrome profiles
* Windows EXE packaging
* Virtual audio routing
* Safe ringing protection
* Intelligent call-state management
* Batch contact calling
* Local-first architecture
* Audio diagnostics tools
* Desktop & Startup shortcuts
* Automated tests

---

# Tech Stack

| Layer              | Technology            |
| ------------------ | --------------------- |
| Language           | Python                |
| Web Framework      | FastAPI               |
| Browser Automation | Selenium              |
| AI Provider        | Groq                  |
| Speech Recognition | Groq STT              |
| Text To Speech     | Edge TTS              |
| Audio Routing      | VB-CABLE              |
| Frontend           | HTML, CSS, JavaScript |
| Packaging          | PyInstaller           |
| Testing            | pytest                |
| OS                 | Windows               |

---

# Architecture

```text
Spectrum-AI-Google-Voice-Agent/
│
├── src/
│   ├── main.py
│   ├── google_voice.py
│   ├── conversation_loop.py
│   ├── voicemail_detector.py
│   ├── ai_groq.py
│   ├── realtime_tts.py
│   ├── audio_capture.py
│   ├── audio_routing.py
│   ├── crm.py
│   ├── web_app.py
│   └── desktop_app.py
│
├── tests/
├── scripts/
├── packaging/
├── installer/
├── logs/
├── chrome_profiles/
└── requirements.txt
```

---

# Core Capabilities

### Google Voice Automation

Controls Google Voice directly through Chrome using Selenium automation and persistent browser profiles.

### Realtime AI Conversations

Captures live audio, converts speech to text, generates AI replies using Groq, and speaks responses back in realtime.

### Safe Call-State Handling

Implements intelligent ringing protection and prevents the AI from speaking before confirmed call pickup.

### Voicemail Detection

Detects voicemail greetings and transitions into voicemail playback workflows automatically.

### FastAPI Dashboard

Provides a complete operator console for:

* live runs
* audio diagnostics
* logs
* leads
* CRM
* recordings
* settings
* preflight checks

### Windows Desktop Deployment

Supports:

* PyInstaller EXE builds
* Desktop shortcuts
* Windows startup launch
* Portable ZIP release

---

# Why This Project Exists

Most AI calling projects rely on expensive telephony APIs.

Spectrum AI Google Voice Agent focuses on a more practical real-world approach by automating Google Voice directly through the browser.

The difficult engineering problems are:

* call-state detection
* voicemail handling
* browser DOM reliability
* audio routing
* realtime AI latency
* long-running stability
* unattended operation

This project is built specifically to solve those real-world workflow challenges.

---

# Installation

## Requirements

* Windows 10/11
* Python 3.10+
* Google Chrome
* Google Voice account
* VB-CABLE
* Groq API key

---

# Install Dependencies

```powershell
python -m pip install -r requirements.txt
```

---

# Setup Environment

```powershell
Copy-Item .env.example .env
Copy-Item dialer_config.example.json dialer_config.json
```

Edit `.env`:

```env
GROQ_API_KEY=your_key_here
GOOGLE_VOICE_URL=https://voice.google.com/u/0/calls
CHROME_PROFILE_DIR=chrome_profiles/sales_profile
PLAYBACK_DEVICE=CABLE Input
CAPTURE_DEVICE=default
CALLBACK_NUMBER=your_callback_number
```

---

# Run The Project

## Start Preflight

```powershell
python -m src.main --preflight
```

---

## Safe Test Call

```powershell
python -m src.main --safe-test +15551234567
```

---

## Start Full Calling Agent

```powershell
python -m src.main
```

---

## Start FastAPI Dashboard

```powershell
python -m src.web_app
```

Open:

```text
http://127.0.0.1:8000
```

---

# Build Windows EXE

```powershell
powershell -ExecutionPolicy Bypass -File .\scripts\build_windows_exe.ps1
```

Output:

```text
dist\IndusDispatchConsole.exe
```

---

# Audio Routing

## Recommended VB-CABLE Setup

| Purpose           | Device                       |
| ----------------- | ---------------------------- |
| Agent Playback    | CABLE Input                  |
| Chrome Microphone | CABLE Output                 |
| Capture Device    | Default / Dedicated Loopback |

---

# Testing

## Run Tests

```powershell
python -m pytest tests -q
```

---

## Compile Check

```powershell
python -m compileall src tests
```

---

# Repository Topics

`ai`
`google-voice`
`automation`
`voice-ai`
`selenium`
`fastapi`
`speech-to-text`
`text-to-speech`
`python`
`crm`
`calling-agent`
`desktop-app`

---

# Recommended Workflow

1. Login to Google Voice
2. Run preflight checks
3. Test audio routing
4. Start safe test call
5. Verify voicemail handling
6. Start outbound automation
7. Monitor logs & dashboard

---

# Runtime Data

These files are intentionally excluded:

```gitignore
.env
.venv/
logs/
chrome_profiles/
dist/
build/
release/
connected_calls/
failed_calls/
voicemail_calls/
audio/voicemails/
audio/scripts/
__pycache__/
.pytest_cache/
```

---

# Future Improvements

* Deepgram realtime STT
* Silero VAD
* Langfuse tracing
* OpenTelemetry metrics
* Smarter voicemail classification
* Docker deployment
* Multi-agent orchestration
* Advanced analytics dashboard

---

# Disclaimer

This project can place real outbound calls.

You are responsible for:

* legal compliance
* consent
* caller ID rules
* recording disclosure
* anti-spam laws
* Do Not Call regulations
* Google Voice terms of service

---

# Repository

GitHub Repository:

```text
https://github.com/atiqurrehman112/spectrum-ai-google-voice-agent
```

---

<div align="center">

## Spectrum AI Google Voice Agent

Realtime AI calling automation built for practical outbound workflows, intelligent conversations, reliable call-state handling, and scalable Windows deployment.

### Built by Atiq ur Rehman

</div>
