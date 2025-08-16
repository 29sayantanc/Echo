# 🎙️ Echo – Your Private AI Journal
([Frontend Walkthrough](https://github.com/29sayantanc/Echo/blob/main/Documentation/Walkthrough/echo_frontend_walkthrough_updated.md)),            ([Backend Flow Diagram](https://29sayantanc.github.io/Echo/))


## The Problem: 

Ever tried to dig up that brilliant idea from last Tuesday’s meeting… and found it buried under half-written notes, or a pile of voice memos you never listen to?  
Most journaling apps are just fancy text boxes. Note-taking apps spread your thoughts across too many places. Voice memos sit in a folder like a junk drawer you’re afraid to open.

**Echo changes that.**  

Type your thoughts directly, record them on the spot, or even paste in text from elsewhere. Got old voice notes? Drop them in — Echo transcribes and processes them so your ideas become searchable, connected, and actually useful.

It’s not just storage – it’s your personal AI that remembers and connects your thoughts. And it doesn’t even need the internet to work. Imagine that.

## What is Echo?

Echo turns scattered thoughts into an intelligent, searchable memory system:

- **🔒 100% Local** – Your data stays on your device. No cloud. No subscriptions. No spying.
- **🧠 Smart Memory** – AI extracts facts, preferences, and patterns from your entries.
- **🎯 Powerful Search** – Find entries by meaning, keywords, or context.
- **💬 Natural Chat** – Ask Echo about your thoughts like talking to a friend.
- **🎤 Voice-First** – Speak naturally, Echo transcribes and processes everything.

## Real Use Cases (Not Just “Dear Diary”)

**Work Profile:**
- Track daily meetings, decisions, and deal progress.
- Remember client preferences and conversation details.  
- Search: *“What did I discuss with Sarah about the Q3 strategy?”*
- Analyze patterns: *“Show me all blockers from last month.”*

**Personal Profile:**
- Journal relationships, goals, and life decisions.
- Remember recommendations and important conversations.
- Spot patterns in mood and energy levels.
- Vent freely, knowing it’s completely private.

**Project Profile:**
- Keep a record of research, ideas, and progress.
- Track what worked and what didn’t.
- Connect related concepts across time.
- Build a personal knowledge base you can search anytime.

## Quick Start

**You need:** Python 3.11+, Node.js 20+, and [Ollama](https://ollama.ai) installed on your system.

1. **Clone the repo**  

    ```bash
    git clone https://github.com/29sayantanc/echo.git
    cd echo
    ```

2. **Install**  

   Go to the `scripts/install` folder and run the installer for your OS:  

   - **Windows**: double-click `install.bat` or run:  

     ```bash
     scripts/install/install.bat
     ```
   - **Mac/Linux**:  

     ```bash
     bash scripts/install/install.sh
     ```
   - **Python-only option** (cross-platform):  

     ```bash
     python scripts/install/install.py
     ```

3. **Run Echo**  

   After installation completes, use the launch script for your OS:  

   - **Windows**:  

     ```bash
     scripts/run/launch.bat
     ```
   - **Mac/Linux**:  

     ```bash
     bash scripts/run/launch.sh
     ```
   - **Python-only option**:  

     ```bash
     python scripts/run/launch.py
     ```

4. **Install AI models** *(first run only)*  

    ```bash
    ollama pull qwen3:8b
    ollama pull mistral:7b
    ```

Once the launch script runs, Echo will automatically open in your default browser ([http://localhost:3000/](http://localhost:3000/)).

## Walkthrough

Want to see Echo in action? ([Walkthrough](https://github.com/29sayantanc/Echo/blob/main/Documentation/Walkthrough/echo_frontend_walkthrough_updated.md))

## My Story

*I Googled “what is an LLM” 2 months ago because I wanted to understand how AI actually works. I came into this without any substantial coding experience – just curiosity, a lot of reading, and the help of AI tools. Echo started as weekend tinkering, turned into something I use daily. Always open to suggestions and feedback!*

## Built With

- **Backend**: Python + FastAPI + SQLite + Sentence Transformers
- **Frontend**: React + TypeScript + Tailwind CSS  
- **AI**: Ollama + Whisper + BGE embeddings + Piper TTS
- **Architecture**: Async processing, memory systems, tool-calling agents

## Development Credits

**AI Coding Assistants:**
- [Claude Code](https://claude.ai/code) – Primary development and architecture implementation.
- [Cursor](https://cursor.sh/) – Code editing and debugging assistance.  
- [Gemini CLI](https://github.com/google/generative-ai-cli) – Additional coding support.

**Documentation:**
- [Claude Desktop](https://claude.ai/) – Technical documentation and user guides.
- [GPT + Monday](https://openai.com/) – Additional documentation support.

**Open Source Projects used:**
- [Ollama](https://ollama.ai/) – Local LLM inference engine.
- [OpenAI Whisper](https://github.com/openai/whisper) – Speech-to-text transcription.
- [Piper TTS](https://github.com/OHF-Voice/piper1-gpl) – Neural text-to-speech synthesis.
- [BGE Embeddings](https://huggingface.co/BAAI/bge-small-en-v1.5) – Semantic embeddings model.
- [FastAPI](https://fastapi.tiangolo.com/) – Modern Python web framework.
- [SQLite](https://sqlite.org/) – Embedded database engine.

**Development Approach:**

This project demonstrates AI-assisted development – I provided the vision, architecture decisions, and user experience design, while AI coding assistants handled the implementation. Every line of code was written by AI according to my specifications and requirements.

## Contributing

Echo is for people who believe your thoughts are too valuable for cloud storage and too important for basic text boxes. Whether you’re:

- Adding new features
- Fixing bugs  
- Improving documentation
- Just trying it out and sharing feedback

**You’re welcome here.** 

Star ⭐ if this resonates with you.

---

*100% local, 100% private, 100% yours*
