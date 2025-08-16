# Echo Journal - Installation Guide

This guide covers two installation methods:  
1. **Quick Start** – Use the provided scripts to install everything automatically.  
2. **Manual Setup** – Step-by-step process in case the scripts fail.

---

## ⚡ Quick Start (Recommended)

**You need:**  
- Python 3.11+  
- Node.js 20+  
- [Ollama](https://ollama.ai) installed  

---

### 1. Clone the Repository  
```bash
git clone https://github.com/29sayantanc/echo.git
cd echo
```

### 2. Install Dependencies  
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

### 3. Run Echo  
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

### 4. Install AI Models *(first run only)*  
```bash
ollama pull qwen3:8b
ollama pull mistral:7b
```

✅ Once the launch script runs, Echo will automatically open in your default browser ([http://localhost:3000/](http://localhost:3000/)).

---

## 🛠 Manual Installation (If Scripts Fail)

Follow these steps only if the Quick Start scripts fail.

---

### 📋 Prerequisites

Before installing Echo, you need these components:

| Component  | Minimum Version | Recommended | Purpose |
|------------|-----------------|-------------|---------|
| **Python** | 3.9+            | 3.11+       | Backend API server |
| **Node.js**| 18+             | 20+         | Frontend development server |
| **npm**    | 9+              | 10+         | Package manager (comes with Node.js) |
| **Git**    | 2.0+            | Latest      | Version control and cloning repository |
| **Ollama** | Latest          | Latest      | Local AI language models |

**Hardware Requirements**  
- **RAM**: 8 GB minimum, 16 GB recommended (for AI models)  
- **Storage**: 10 GB free space minimum (more if installing additional AI models)  
- **CPU**: Any modern processor (AI processing benefits from faster CPUs)
- **GPU**: 8 GB minimum, 16 GB recommended (for AI models) 

---

### 1. Clone the Repository  
```bash
git clone https://github.com/29sayantanc/echo.git
cd echo
```

### 2. Backend Setup  
```bash
cd backend
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Start Backend  
```bash
python run.py
```
Leave this terminal running.

### 4. Frontend Setup *(in a new terminal)*  
```bash
cd frontend
npm install
```

### 5. Start Frontend  
```bash
npm run dev
```

### 6. Install AI Models  
```bash
ollama pull qwen3:8b
ollama pull mistral:7b
```

### 7. Access Echo  
Open your browser and go to:  
[http://localhost:3000/](http://localhost:3000/)

---

✅ You now have Echo running locally! If you encounter issues, check your dependencies and version numbers before retrying.
