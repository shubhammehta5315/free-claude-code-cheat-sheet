# free-claude-code-cheat-sheet

# 🚀 Claude Code FREE Setup Guide (2026)
**By BlackBox Security** | [YouTube Channel](https://www.youtube.com/@TheBlackBoxSecurity)

A highly simplified, lightning-fast cheat sheet to set up **Claude Code** completely FREE using Minimax M2.5 & OpenCode. No expensive APIs, no GPU required.

---

## 🛠️ Step 1: Install Dependencies

You need **Node.js (v18+)** and the **Claude Code CLI** installed on your system.

### 🪟 Windows
```powershell
# 1. Install Node (using Chocolatey) or download from nodejs.org
choco install nodejs

# 2. Install Claude Code
npm install -g @anthropic-ai/claude-code

🍎 Mac

# 1. Install Node (using Homebrew)
brew install node

# 2. Install Claude Code
npm install -g @anthropic-ai/claude-code

🐧 Linux (Ubuntu/Debian)

# 1. Install Node
sudo apt update && sudo apt install nodejs npm

# 2. Install Claude Code
sudo npm install -g @anthropic-ai/claude-code

🔑 Step 2: Get Your Free API Key
Go to OpenCode.ai and click "Get started with Zen".

Login with Google/GitHub (⚠️ Do NOT enable billing).

Copy your free Minimax 2.5 API Key.

⚙️ Step 3: Configure Settings (The Magic Patch)
We need to redirect Claude Code to use our free OpenCode API instead of Anthropic's paid servers.

Open the configuration file in VS Code:

Windows: code $env:USERPROFILE\.claude\settings.json

Mac/Linux: code ~/.claude/settings.json

Paste this exact JSON into the file and Save:

{
  "env": {
    "ANTHROPIC_BASE_URL": "[https://opencode.ai/zen](https://opencode.ai/zen)",
    "ANTHROPIC_MODEL": "minimax-m2.5-free",
    "ANTHROPIC_API_KEY": "PASTE_YOUR_OPENCODE_API_KEY_HERE",
    "ENABLE_TOOL_SEARCH": "true"
  }
}

🛡️ SECURITY WARNING: Treat your API key like a password. Never share this settings.json file or commit it to a public GitHub repository.

⚡ Step 4: Run & Test
Open your terminal and type:

claude code


It will ask if you want to use the custom API key. Select Yes.Quick Commands Reference:Command
What it doesclaudeStarts an interactive AI coding sessionclaude -p "build a python script"Runs a single prompt directlyclaude --verboseShows detailed background logs

💻 Recommended Laptops for AI & Coding (2026 Picks)
If you are looking to upgrade your setup, here are my top recommended laptops for developers,
categorized by use case:
🔥 Gaming, Editing & Heavy AI Workloads
Asus TUF F16Lenovo Legion 5HP Omen Ryzen 7MSI Katana i7⚡ Students & Daily ProgrammingLenovo Ideapad Slim 3Asus Vivobook 15Acer Aspire LiteHP 15🍎 Creators & Pro DevelopersMacBook Pro M5MacBook Air🌐 Connect with BlackBox SecurityYouTube: Subscribe for more Tech & CybersecurityTelegram: Join our Cyber-CellInstagram: @blackbox__securityHappy Vibe Coding! 🚀
