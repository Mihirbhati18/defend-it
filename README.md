# 🛡️ defend-it

**Your AI built the project. Now make sure *you* can defend it.**

An AI agent skill that gets you ready for your **viva, project review, or job interview**, using *your own code*.

<!-- 🎬 Demo GIF goes here -->

---

## 😬 The problem

- AI picked your project topic. AI wrote most of the code.
- Then the examiner asks: *"Who would actually use this?"* or *"Walk me through this function."*
- …and you freeze.

## ✅ What defend-it does

| Mode | What you get |
|---|---|
| 🔍 **Reality check** | Searches the internet for similar apps and real users, finds weak features and flaws **before** your examiner does, and gives you a fix or an honest answer for each |
| 🎓 **Viva prep** | Explains *your* code in simple words, then runs a mock viva, one question at a time, with theory links (DBMS, OS, OOP, DSA, CN) |
| 💼 **Interview prep** | Mock interview about your project (startup / big tech / service / HR style) + honest resume lines |

Plus:
- 💀 **Examiner styles**: Friendly guide → Strict professor → External examiner
- 📄 **1-page cheat sheet** (`DEFENSE_NOTES.md`) at the end, no long reports
- 🗣️ **Simple language**, short answers, Hinglish if you want it

## 👀 What it looks like

```
🔍 Reality check done. Score: 5/10

✅ Real problem? Partly. Hostel students do fight over washing machines
👤 Real user: Students in your hostel (not "everyone")
🏁 Similar things: Google Forms, a WhatsApp group, paid laundry apps

❌ Biggest problem: Two students can book the same slot at once.
   🗣️ Say: "Right now it's a prototype. I'd add a slot lock in the database to stop double booking."
   🛠️ Fix: check the slot inside a transaction in routes/booking.js

⚠️ 2 more issues. See them? (yes / skip)
```

```
💀 External examiner: "Google Forms can do this. Why did you build an app?"

You: "because it's better"

❌ Not quite. Too vague.
💡 Better: "Forms can't stop double booking or show live free slots. My app does both."
```

## 📦 Install

**Any agent that supports skills (Claude Code, Codex, Cursor, and others):**
```bash
npx skills add Mihirbhati18/defend-it
```

**Claude Code (manual):** copy the `skills/defend-it` folder into `~/.claude/skills/`.

**ChatGPT / Claude / Gemini website (no install):** copy the prompt from [`chat-version/PROMPT.md`](chat-version/PROMPT.md), paste it in a new chat, and then paste or upload your main project files.

## 🚀 Use

Open your project folder in your agent and say:

```
/defend-it
```
or just:
- "reality check my project"
- "prepare me for my viva"
- "mock interview on my project"

## 🤔 Is this cheating?

No. It does the opposite: it makes you **understand** your own project. It never writes fake achievements or tells you to hide flaws.

## 🤝 Contributing

Ideas welcome, especially:
- more viva questions from your college or branch
- new examiner styles
- support for more languages

Open an issue or a PR.

## 📄 License

MIT
