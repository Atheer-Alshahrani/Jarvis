
### The Ultimate Cross-Platform Personal AI Assistant - By Atheer

> 

A real-time voice AI that can hear, see, speak, and control your computer — on any OS. Supports Windows, macOS, and Linux. Built on the Gemini Live API for native audio streaming, delivering zero subscriptions and total digital autonomy.

---

##  Overview

Jarvis gave the assistant a screen. **Jarvis lets you choose what runs it.**

Until now this was a Gemini assistant, and only that. If you had no quota left, no
connection, or a rule that says your microphone does not leave the building, you
had no assistant. Mark LVI adds a second way to hold the conversation — speech
recognition, a language model and a voice, assembled from parts you pick in
→ **ENGINE & PROVIDERS** — and a way to point the assistant's own background
requests at a different model without touching the voice at all.

The local model can be on your machine (Ollama, LM Studio, llama.cpp, vLLM) or
somebody else's API (OpenAI, Groq, DeepSeek, Mistral, xAI, OpenRouter, Together).
Both are the same setting, because all of them speak the same protocol.

**None of it costs anything if you do not use it.** On a default install the
`providers/` folder is never imported — not at startup, not on a tool call, not
when the settings drawer opens. Measured: the decision takes **0.16 ms** and
loads nothing. The folder can be deleted, and deleting it changes nothing.

Everything the assistant already does carries over untouched. A local engine
inherits the avatar, the lip-sync, the self-echo guard, push-to-talk, the wake
word, memory, undo, the confirmation gate and every action and plugin — because
it enters through the same door the Live session always did.

Jarvis also changes what the assistant is allowed to CLAIM. Every tool that
drives an application now answers with what it observed rather than with what it
attempted: `done` means it was checked, `unverified` means the request went out
and could not be confirmed — and the assistant says exactly that instead of
rounding it off to "done". Opening an app watches the process table for it.
Closing one asks the application politely, then checks whether it went.

It's not just an assistant — it's an extension of your digital life.

---

##  Capabilities

### Core Features
| Feature | Description |
|---|---|
| Holographic Avatar | An animated human head in the HUD — real facial geometry, lit and drawn in software, no GPU or extra packages |
| Real Lip-Sync | ~50 mouth shapes a second from the audio's formants **and** the transcript — closures, spreads and rounds, not a volume meter |
| Language-Free Mouth | Articulation is derived by Unicode reduction, so Latin, Cyrillic and Greek scripts all work from one rule set — and scripts that hide pronunciation fall back cleanly |
| Facial Acting | Brows track the phrase, gaze saccades between fixations, natural blinking, a small nod on stressed syllables |
| Face as Status | Looks away while thinking, meets your eyes while listening, lids fall while asleep, glances down at new content |
| Push-to-Talk | Hold **Ctrl+Space** and the mic opens — closed the rest of the time. Truly global on Windows, window-scoped elsewhere |
| Self-Echo Guard | Never answers its own last sentence: the tail of its own voice is recognised and dropped without muting you |
| Runtime Self-Knowledge | Name, OS, abilities **and limits** are generated from the live system each session — rename it or add a plugin and it knows |
| Wake Word | Local **"Hey Jarvis"** detection — sleeps until called, auto-sleeps after 2 min of silence, and never streams audio while asleep |
| Instant Acknowledgment | Speaks a short, context-aware reply in **your language** the instant a longer task starts — no more silent waiting |
| Faster Live Engine | Runs on **Gemini 3.1 Flash Live** — roughly 2× faster time-to-first-word than the previous model |
| Self-Describing Skills | Every bundled skill declares its own `TOOL` dict + handler and is auto-discovered at launch — adding one is a single file |
| Recallable Memory | No size limit and nothing silently forgotten — the prompt carries what fits, the rest is looked up on demand from a local search |
| Memory Panel | See every fact JARVIS has stored about you, when it learned it, and delete any of it in one click |
| Undo | Take back what the assistant did — files it moved, renamed, created or wrote, and settings it changed |
| Real Confirmation | Shutdown, restart and WiFi wait for a button **you** press — the model cannot confirm its own irreversible actions |
| Audio Device Picker | Choose the microphone and speakers by name, filtered to the short list your OS shows — and measured, so every entry actually works |
| Session Continuity | A dropped connection, a voice change or a device change no longer wipes the conversation |
| Plugin System | Drop a single `.py` file into `plugins/` — JARVIS learns a new skill on next launch |
| Video on the HUD | Plays YouTube, a local file or any video URL **where the avatar sits** — starts muted, sound on request |
| Model Ladder | Nine Gemini models in one measured order — a quota, a timeout or an outage steps to the next rung instead of failing |
| Choose Your Engine | Gemini Live, or your own STT + LLM + TTS — picked in the UI, no file editing |
| Local & Third-Party Models | Ollama · LM Studio · llama.cpp · vLLM · OpenAI · Groq · DeepSeek · Mistral · xAI · OpenRouter — one setting, because they share a protocol |
| Local Speech | Whisper on your CPU for hearing, Piper for speaking — **~50 languages**, neural, entirely offline |
|  The Voice Follows You | Whisper hears which language you spoke; the answer comes back in that language's voice, switching mid-conversation |
|  Reasoning Stays Private | `<think>` blocks from qwen3, deepseek-r1 and their distills are never read aloud |
|  ElevenLabs Voice | One voice that speaks every language, streamed |
|  Tool Budget | A small model is given the tools that matter instead of all 45 — core-first, by count and by size |
|  Real-time Voice | Ultra-low latency conversation in any language via Gemini Live API |
|  Live Theming | Recolour the entire HUD from a hue wheel or hex — the avatar retints with it |
| Reactive HUD | Waveform pulses to real audio — your mic while listening, JARVIS while speaking |
| Voice Picker | Choose from 5 native Gemini voices and switch live from the UI — no restart |
|  Unlimited Sessions | Sliding-window context compression — one conversation can last for hours |
|  System Control | Launch apps, adjust volume/brightness, WiFi, shortcuts, power — all by voice |
|  Autonomous Tasks | High-level planning for complex multi-step goals via agent mode |
|  Visual Awareness | Screen capture and webcam vision piped into your main Gemini session, labelled by source |
|  Persistent Memory | Deeply remembers projects, preferences, and personal context across sessions |
|  Hybrid Input | Seamlessly switch between keyboard typing and voice commands |
|  Morning Briefing | On first boot: greets you, reads the time, recaps yesterday, and fetches live news |
|  Proactive 2.0 | Time-aware, context-aware check-ins — knows the time of day, your projects, and what you've been discussing |
|  Session Memory | Summarises each conversation and mentions it naturally next morning — consumed after use, never repeats |
|  Background Monitoring | User-configured topic watching — checks for new headlines once a day and alerts naturally |
|  Hardware Monitoring | Continuous CPU, RAM, GPU and temperature telemetry with localized voice alerts |
|  Weather Report | Live weather data for your city, personalized from memory |
|  Dynamic Content Panel | Scrollable display layer beneath the HUD that renders web results, news, and search data |
|  Multi-Mode Web Search | `news` / `research` / `price` / `compare` / `search` — Gemini Grounded first, DDG fallback |
|  Smart Reminders | OS-native scheduled notifications (Windows Task Scheduler / macOS LaunchAgent / Linux systemd) |
|  File Processor | Read, summarize, and answer questions about local files |
|  Browser Control | Open URLs, navigate tabs, and interact with the browser by voice |
|  Send Message | Compose and send messages through WhatsApp, Telegram, and more |
|  Desktop Control | Taskbar, window management, and desktop-level operations |
|  Silent Language Memory | Detects spoken language on first use — all future sessions adapt automatically |
|  Remote Dashboard | Control the assistant from your phone via QR code pairing |
|  Auto-Start on Boot | Registers with the OS startup system (registry / LaunchAgent / .desktop) |
|  Clipboard Intelligence | Copy any text → floating panel with Translate / Summarise / Explain / Fix |
|  It Says What It Checked | Every tool answers `done` / `unverified` / `failed` — a request that could not be confirmed is never spoken as a success |
|  Close an App by Name | Matched against what is running, asked politely so unsaved work survives, and the assistant's own processes are never a target |
|  Raise, Don't Duplicate | Opening something already running brings its window to the front instead of starting a second copy |
|  Untrusted Content Boundary | Web pages and documents reach the model wrapped as data — an instruction inside one is reported, not obeyed |
|  Platform Honesty | On Wayland, or a macOS without permissions, it says what this session will not let it do instead of narrating a click that never happened |
|  Per-Device Volume | The output slider belongs to the speaker you picked, not to whatever the system calls default |
|  Prove It Hears You | A TEST button with a live meter — the one check an automated probe on silence can never make |
| Assistant Customization | Change the assistant name, your name, voice, and colour from the UI — takes effect immediately |



## Quick Start

```bash


python setup.py        # installs deps for YOUR OS + the browser automation engine
python main.py
```

`setup.py` only ever installs what your operating system needs — the Windows-only libraries are skipped automatically on macOS and Linux, and vice-versa. It also checks your Python version up front, so a wrong interpreter fails with a sentence instead of a wall of pip output. Prefer to do it by hand? `pip install -r requirements.txt` works too.

> **Installation Note:** If you hit a `ModuleNotFoundError` for an OS-specific package, install it with `pip install <module_name>`. The optional **wake word** engine is *not* installed here — grab it in one click from **⚙ → WAKE WORD** inside the app.

---

##  Requirements

| Requirement | Details |
| --- | --- |
| **OS** | Windows 10/11, macOS, or Linux |
| **Linux display server** | Everything works on **X11**. On **Wayland** — the default on Ubuntu 22.04+, Fedora and current GNOME/KDE — the system does not permit any program to type, click, capture the screen or raise another window, so those features are unavailable and JARVIS says so at startup instead of pretending. Voice, memory, files, the web and opening applications are unaffected. Log out and pick an Xorg session to get the rest |
| **macOS permissions** | Accessibility (to type and click) and Screen Recording (to see the screen), both under System Settings → Privacy & Security. Until granted, those actions silently do nothing — the OS reports success either way |
| **Python** | 3.11, 3.12 or 3.13 |
| **Microphone** | Required for voice interaction (and for the "Hey Jarvis" wake word) |
| **Speakers** | Required for voice replies |
| **API Key** | Free Gemini API key (entered on first launch → `config/api_keys.json`). Only for the Gemini engine — a fully local setup needs no key and no account |
| **GPU** | **Not required, anywhere.** The avatar and HUD video are rendered in software; local speech recognition and the neural voice both run on the CPU by default |
| **YouTube on the HUD** | `yt-dlp`, installed by `setup.py`. Without it, local files and direct URLs still play and YouTube links open in the browser with an explanation |
| **Wake word** *(optional)* | One-click download from  → WAKE WORD (`openwakeword`, a few MB, fully local) |
| **A different engine** *(optional)* | Nothing extra.  → ENGINE & PROVIDERS talks to any local or hosted model over HTTP using a library the app already has |
| **Local speech recognition** *(optional)* | `faster-whisper`, installed from the same panel. **CPU is the default** — a GPU is an option, never a requirement |
| **Local voice** *(optional)* | `piper-tts` for a neural voice in ~50 languages, one click from the panel — or nothing at all, and it uses the voices your OS already has |

---

##  Project Structure

```
Mark LVI/
├── main.py                   # Core loop — Gemini Live session, audio I/O, viseme extraction, tool dispatch
├── ui.py                     # PyQt6 HUD — avatar canvas, waveform, log panel, settings drawer, camera feed
├── setup.py                  # OS-aware installer (skips wrong-OS dependencies, checks your Python)
├── .gitignore                # Keeps your API key, TLS key and memories out of the repository
├── providers/                # OPTIONAL — delete it and the assistant runs on Gemini,
│                             #   exactly as it did before this folder existed.
│                             #   Never imported unless a provider is configured.
│   ├── base.py               # The contract: Engine / LLM / STT / TTS, caps, Live-shaped events
│   ├── registry.py           # Discovery and construction — imports one module, on demand
│   ├── schema.py             # Tool declarations: Gemini <-> OpenAI <-> Anthropic, and the budget
│   ├── audio.py              # Rates and formats — 16 kHz in, 24 kHz out, everything between
│   ├── llm_openai.py         # Every /v1/chat/completions endpoint: local servers and hosted APIs
│   ├── stt_whisper.py        # faster-whisper on the CPU, or a transcription API
│   ├── tts_piper.py          # Neural voice here, ~50 languages, follows the one you speak
│   ├── tts_system.py         # Windows SAPI / macOS say / Linux espeak-ng — nothing to download
│   ├── tts_elevenlabs.py     # One voice, every language, streamed
│   ├── engine_pipeline.py    # STT -> LLM -> TTS, wearing the Live session's interface
│   ├── _tests.py             # `python -m providers._tests` — no network, no key needed
│   └── voices/               # Piper voices, downloaded on demand (git-ignored)
├── plugins/                  # OPTIONAL skills — delete any file and it is simply gone
│   │                         #   next launch. This is where anything that is NOT
│   │                         #   about driving the computer lives; see actions/.
│   ├── _template.py          # Copy this to write a new skill — one file, drop in, done
│   │                         #   A file starting with _ is a shared driver, not a skill:
│   │                         #   the loader skips it, and the skills beside it import it.
│   ├── _whatsapp_core.py     # Shared WhatsApp driver — desktop app or Web, all three OSes
│   ├── whatsapp_call.py      # Place and end WhatsApp voice / video calls
│   ├── whatsapp_guard.py     # Answer, decline or auto-reply to INCOMING WhatsApp calls
│   ├── telegram_remote.py    # Drive JARVIS from anywhere over Telegram
│   ├── chat_takeover.py      # Reads an on-screen chat and replies in it
│   ├── screen_agent.py       # Looks at the screen and works it, step by step
│   ├── gmail_control.py      # Read, search, send and draft email
│   ├── calendar_control.py   # Read and create calendar events
│   ├── obsidian_vault.py     # Read and write notes in an Obsidian vault
│   ├── document_review.py    # Review a document and report what should change
│   ├── excel_writer.py       # Spreadsheet output
│   ├── code_helper.py        # Write and run small programs
│   ├── dev_agent.py          # Multi-file project work
│   ├── image_generator.py    # Generate images
│   ├── upload_video.py       # Upload the video on your Desktop to YouTube
│   ├── youtube_video.py      # Search, summarise and fetch transcripts
│   ├── printer_control.py    # 3D printers, over MQTT
│   ├── home_assistant.py     # Smart-home devices
│   ├── game_updater.py       # Update or install games through their launcher
│   ├── flight_finder.py      # Flight search
│   ├── shopping_list.py      # Shopping list
│   ├── pomodoro.py           # Pomodoro timer
│   ├── water_reminder.py     # Hydration reminders with intake tracking
│   ├── quiz.py               # Spoken quizzes
│   ├── spaced_repetition.py  # Flashcard review
│   ├── calorie_counter.py    # Food through the webcam
│   └── pushup_counter.py     # Counts pushups through the webcam
├── actions/                  # Bundled skills — each self-describes via a TOOL dict + handler
│                             #   Everything here drives the COMPUTER, which is what decides
│                             #   whether a new skill belongs in this folder at all.
│   ├── web_search.py         # Gemini + DDG parallel search (news, research, price, compare)
│   ├── screen_processor.py   # Screen & webcam capture for vision
│   ├── background_monitor.py # User-configured topic watching — daily DDG check
│   ├── proactive.py          # Proactive 2.0 — time/context/rotation-aware check-ins
│   ├── reminder.py           # OS-native scheduled notifications
│   ├── system_monitor.py     # CPU / RAM / GPU / temperature telemetry
│   ├── computer_settings.py  # Volume, brightness, WiFi, power (per-OS)
│   ├── computer_control.py   # Keyboard shortcuts, mouse, window management
│   ├── open_app.py           # Application launcher (per-OS name map)
│   ├── browser_control.py    # Web browser control
│   ├── file_controller.py    # File system operations
│   ├── file_processor.py     # Document reading and summarization
│   ├── send_message.py       # Messaging integration
│   ├── weather_report.py     # Live weather data
│   ├── video_player.py       # Plays video on the HUD, where the avatar normally is
│   └── desktop.py            # Desktop and taskbar control
├── memory/
│   ├── memory_manager.py     # Load/save long_term.json — sessions, monitors, identity
│   ├── config_manager.py     # api_keys.json access — key, OS, name, voice, colour, toggles
│   └── long_term.json        # Persistent store — created on first run
├── dashboard/                # Phone control — paired by QR code, one-time key
│   ├── server.py             # FastAPI + uvicorn; HTTP by default, HTTPS opt-in
│   └── static/               # The phone page and its login screen
├── core/
│   ├── outcome.py            # What a tool tells the model: done / unverified / failed /
│   │                         #   ask / started, plus the untrusted-content wrapper
│   ├── appidentity.py        # Which applications are running, which one the user named,
│   │                         #   and which processes are the assistant's own (never a target)
│   ├── lazyimport.py         # Heavy third-party imports paid only if they are used
│   ├── platform_support.py   # What THIS machine permits — Wayland, macOS permissions —
│   │                         #   reported to the user and to the model, never guessed at
│   ├── gemini.py             # One place for every one-shot Gemini call — model ladder, timeouts,
│   │                         #   cooldowns, and the configured provider as one more rung
│   ├── prompt.txt            # All prompt wording — {tokens} are filled from the live system at startup
│   ├── avatar.py             # Avatar renderer — lighting, pose, expression, mouth (QPainter)
│   ├── avatar_mesh.py        # Head geometry — loads the face, generates skull/neck/rigs
│   ├── face_model.obj        # The face itself (MediaPipe canonical model, Apache-2.0, 25 KB)
│   ├── viseme.py             # Transcript → mouth shapes, fused with the audio's timing
│   ├── echo.py               # Tells your voice from the assistant's own echo; self-calibrating
│   ├── hotkey.py             # Push-to-talk chord — global on Windows, windowed fallback elsewhere
│   ├── undo.py               # One shared undo stack — actions register how to reverse themselves
│   ├── confirm.py            # Irreversible-action gate — the token is issued by the UI, not the model
│   ├── audio_devices.py      # Microphone / speaker list — filtered, measured, resolved by name
│   ├── plugin_loader.py      # Plugin engine — discovery, validation, crash isolation
│   ├── action_loader.py      # Bundled-action engine — the built-in twin of plugin_loader
│   └── wake_word.py          # Local "Hey Jarvis" detector — own thread, offline, opt-in
└── config/
    ├── api_keys.json         # API key, name, voice, colour, toggles — created on first launch (git-ignored)
    └── certs/                # Self-signed TLS pair for the phone dashboard — generated locally (git-ignored)
```
