# aichat
## aichat is a complete aichat CLI agent for Termux/Android 16 that replaces every Google reference with open-source and free-tier alternatives.
Built this comprehensive AI chat agent for Termux.

# ✅ Complete — aichat 2.0 is Ready for Termux/Android 16

# a full-featured AI chat agent CLI called aichat that replaces every Google reference with free, open alternatives. ## Here's what's included:

---

# 📁 Project Structure (33 files)

```
aichat/
├── aichat/                       # Core Python package
│   ├── __main__.py               # Entry point: python -m aichat
│   ├── chat.py                   # Main REPL with 25+ slash commands
│   ├── config.py                 # Hierarchical settings (global/project)
│   ├── llm/
│   │   └── provider.py           # NVIDIA NIM free API + local models
│   ├── skills/
│   │   ├── manager.py            # Skill discovery & loading
│   │   └── loader.py             # Progressive disclosure
│   ├── tools/
│   │   ├── registry.py           # MCP-like tool system
│   │   ├── local_storage.py      # SQLite + filesystem
│   │   ├── cloud_storage.py      # S3-compatible (Storj/B2/Wasabi)
│   │   └── browser.py            # Web scraping/search
│   ├── artifacts/
│   │   └── manager.py            # Planning/fast mode + review
│   ├── hooks/
│   │   └── runner.py             # JSON hook system
│   ├── voice/
│   │   └── transcriber.py        # Termux API voice input
│   └── utils.py                  # Utilities & banner
├── skills/                       # 4 built-in skills
│   ├── code-review/SKILL.md
│   ├── python-dev/SKILL.md
│   ├── web-dev/SKILL.md
│   └── terminal/SKILL.md
├── scripts/
│   ├── install.sh                # Full Termux installer
│   ├── setup_mcp.sh              # MCP server wizard
│   └── setup_cloud.sh            # Cloud storage wizard
├── docs/GUIDE.md                 # Complete user guide
├── README.md                     # Quick start reference
├── config.example.json           # Configuration template
├── requirements.txt
└── setup.py
```

---

# # 🔑 What Replaced Google

Google Product	Replacement	Cost	
Gemini API	NVIDIA NIM free tier	Free — 5000 RPM, no CC	
Google Drive	Local SQLite + Storj/Backblaze B2	10-25GB free	
Google Cloud Storage	S3-compatible free tiers	Free tier	
Chrome DevTools	Lightweight requests/BS4 scraper	Free	
Google Speech	Termux API speech-to-text	Free	
Agent Manager	Built-in project system	Free	
Telemetry	Opt-in, disabled by default	—	

---

# 🚀 Quick Install in Termux

```bash
# 1. Clone and enter directory
cd aichat

# 2. Run the installer
bash scripts/install.sh

# 3. Get FREE API key at https://build.nvidia.com

# 4. Set your key
export NVIDIA_API_KEY=nvapi-your-key

# 5. Launch!
aichat
```

---

# 🎮 Key Commands

Command	Action	
`/help`	Show all 25+ commands	
`/plan`	Planning mode with artifact review	
`/fast`	Fast mode (auto-execute)	
`/model`	Switch between 20+ free models	
`/skills`	List and activate skills	
`/browser <query>`	Web search without Chrome	
`/goal <task>`	Run autonomously until done	
`/grill-me <task>`	Ask clarifying questions first	
`/voice`	Toggle voice input	
`/storage cloud on`	Enable cloud sync	

---

# 🧠 Free API Endpoints Used

Endpoint	Purpose	Limits	
`integrate.api.nvidia.com/v1`	LLM inference (20+ models)	5000 RPM free	
`html.duckduckgo.com`	Web search	Unlimited	
`gateway.storjshare.io`	Cloud storage	25GB free	
Local port 8080	llama.cpp local models	Unlimited	

All 13 Python modules compile cleanly, all JSON configs validate, and the full documentation has zero references to Google products — replaced entirely with NVIDIA NIM, open-source models, S3-compatible free tier cloud storage, and local-first architecture.