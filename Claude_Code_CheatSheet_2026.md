# Claude Code FREE Setup Guide (2026)

_By BlackBox Security | The Ultimate AI Coding Cheat Sheet_

A highly simplified, lightning-fast cheat sheet to set up Claude Code completely FREE using Minimax M2.5 & OpenCode. No expensive APIs, no GPU required.

---

# Step 1: Install Dependencies

You need Node.js (v18+) and the Claude Code CLI installed on your system.

## Windows

```bash
# 1. Install Node (using Chocolatey) or download from nodejs.org
choco install nodejs

# 2. Install Claude Code
npm install -g @anthropic-ai/claude-code
```

## Mac

```bash
# 1. Install Node (using Homebrew)
brew install node

# 2. Install Claude Code
npm install -g @anthropic-ai/claude-code
```

## Linux (Ubuntu/Debian)

```bash
# 1. Install Node
sudo apt update && sudo apt install nodejs npm

# 2. Install Claude Code
sudo npm install -g @anthropic-ai/claude-code
```

---

# Step 2: Get Your Free API Key

1. Go to OpenCode.ai and click **"Get started with Zen"**
2. Login with Google/GitHub
3. **Do NOT enable billing**
4. Copy your free **Minimax 2.5 API Key**

---

# Step 3: Configure Settings (The Magic Patch)

We need to redirect Claude Code to use our free OpenCode API instead of Anthropic's paid servers.

Open the configuration file in VS Code:

## Windows

```powershell
code $env:USERPROFILE\.claude\settings.json
```

## Mac/Linux

```bash
code ~/.claude/settings.json
```

Paste this exact JSON into the file and save:

```json
{
  "env": {
    "ANTHROPIC_BASE_URL": "https://opencode.ai/zen",
    "ANTHROPIC_MODEL": "minimax-m2.5-free",
    "ANTHROPIC_API_KEY": "PASTE_YOUR_OPENCODE_API_KEY_HERE",
    "ENABLE_TOOL_SEARCH": "true"
  }
}
```

> ⚠️ SECURITY WARNING:
> Treat your API key like a password.
> Never share this `settings.json` file or commit it to a public GitHub repository.

---

# Step 4: Run & Test

Open your terminal and type:

```bash
claude
```

It will ask if you want to use the custom API key.

Select: **Yes**

---

# Quick Commands Reference

| Command | What it does |
|---|---|
| `claude` | Starts an interactive AI coding session |
| `claude -p "build a python script"` | Runs a single prompt directly |
| `claude --verbose` | Shows detailed background logs |

---

# Recommended Laptops for AI & Coding (2026)

## Gaming & Heavy AI

- Asus TUF F16
- Lenovo Legion 5
- HP Omen Ryzen 7
- MSI Katana i7

## Students & Daily

- Lenovo Ideapad Slim 3
- Asus Vivobook 15
- Acer Aspire Lite
- HP 15

## Creators & Pro

- MacBook Pro M5
- MacBook Air

---

# Connect with BlackBox Security

- YouTube: `@TheBlackBoxSecurity`
- Telegram: `t.me/theblackboxsecurity`
- Instagram: `@blackbox__security`

---

Happy Vibe Coding! 🚀
