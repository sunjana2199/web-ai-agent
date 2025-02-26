# Web-AI-Agent
This is the repository for demonstrating Web-AI Agents





# Browser-Use Web UI - Local Installation Guide

## Prerequisites
Ensure you have the following installed before proceeding:

- **Python 3.11 or higher**
- **Git** (for cloning the repository)

## Installation
Follow these steps to set up and run Browser-Use Web UI locally.

### Step 1: Clone the Repository
```sh
git clone https://github.com/browser-use/web-ui.git
cd web-ui
```

### Step 2: Set Up Python Environment
Use `uv` to create a virtual environment:
```sh
uv venv --python 3.11
```

Activate the Virtual Environment:

**Windows (Command Prompt):**
```sh
.venv\Scripts\activate
```

**Windows (PowerShell):**
```sh
.\.venv\Scripts\Activate.ps1
```

**macOS/Linux:**
```sh
source .venv/bin/activate
```

### Step 3: Install Dependencies
Install required packages:
```sh
uv pip install -r requirements.txt
```

Install Playwright:
```sh
playwright install
```

### Step 4: Configure Environment
Copy the example environment file:

**Windows (Command Prompt):**
```sh
copy .env.example .env
```

**macOS/Linux/Windows (PowerShell):**
```sh
cp .env.example .env
```

Edit `.env` and add your API keys.

### Step 5: Create a Gemini API Key
1. Open [Google AI Studio](https://ai.google.com/studio/).
2. Sign in and generate a **Gemini API Key**.
3. Copy and paste it into your `.env` file.

### Step 6: Run Browser-Use Web UI
Start the Web UI with:
```sh
python webui.py --ip 127.0.0.1 --port 7788
```

Access the interface at [http://127.0.0.1:7788](http://127.0.0.1:7788).

For more details, visit: [Browser-Use Web UI Repository](https://github.com/browser-use/web-ui).


