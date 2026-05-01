# CLaude-freely-use-mobile-AI-chatbot-using-termux

# 🚀 Claude Code Setup (Termux / Linux)

This guide will help you install and run Claude Code using OpenRouter API.

---

## 📦 Step 1: Update System

```bash
pkg update && pkg upgrade -y
```

---

## 📦 Step 2: Install Required Packages

```bash
pkg install nodejs git nano -y
```

---

## 🔍 Step 3: Verify Installation

```bash
node -v
npm -v
```

---

## ⚙️ Step 4: Install Claude Code

```bash
npm install -g @anthropic-ai/claude-code@2.1.112
node $PREFIX/lib/node_modules/@anthropic-ai/claude-code/install.cjs
```

---

## 🔑 Step 5: Setup API (OpenRouter)

Set environment variables:

```bash
export ANTHROPIC_BASE_URL="https://openrouter.ai/api"
export ANTHROPIC_AUTH_TOKEN="sk-or-v1-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
export CLAUDE_CODE_USE_AUTH_TOKEN=true
export ANTHROPIC_MODEL="z-ai/glm-4.5-air:free"
```

---

### 💾 (Optional) Save Environment Variables Permanently

```bash
echo 'export ANTHROPIC_BASE_URL="https://openrouter.ai/api"' >> ~/.bashrc
echo 'export ANTHROPIC_AUTH_TOKEN="sk-or-v1-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"' >> ~/.bashrc
echo 'export CLAUDE_CODE_USE_AUTH_TOKEN=true' >> ~/.bashrc
echo 'export ANTHROPIC_MODEL="z-ai/glm-4.5-air:free"' >> ~/.bashrc
source ~/.bashrc
```

---

## ✨ Step 6: Run Claude

```bash
claude
```

---

## ✅ Done!

You can now use Claude Code with OpenRouter 🚀

---

## 🧪 Test Command

```bash
claude "Write a Python script to print Hello World"
```

---

## ⚠️ Important Notes

* Replace `sk-or-v1-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx` with your actual OpenRouter API key.
* Ensure your internet connection is active.
* Restart the terminal if any command is not recognized.

---

## 💡 Troubleshooting

* If `claude` command not found:

```bash
npm list -g --depth=0
```

* Reinstall if needed:

```bash
npm install -g @anthropic-ai/claude-code@2.1.112
```

---

## 🎯 You're Ready!

Happy Coding with Claude Code 🎉
