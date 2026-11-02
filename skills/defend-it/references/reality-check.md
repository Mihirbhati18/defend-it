# Reality check — full procedure

Goal: find what a mature examiner or interviewer will attack *before* they do, and give the student a fix or an honest answer for each.

Remember the golden rules: short, simple, top issue first, max 3 issues before asking to continue.

## 1. Research the real world

Use a web search tool if you have one. Do 3–6 searches, not more. Good queries:

- `<what the app does> app` / `<what the app does> alternative`
- `<problem> software for <user group>`
- `<project name or idea> github`
- `<problem> reddit` — to see if real people complain about it
- `<problem> statistics <country>` — only if the student will need a number

From the results, pull out:

| Find | Why it matters |
|---|---|
| 2–3 similar apps / products | Examiner asks "this already exists, why build it?" |
| 1–2 similar GitHub projects | Shows the student what others did better or differently |
| Proof the problem is real | Gives them a strong opening line |
| What the existing tools *don't* do | This becomes the student's unique point |

Always show links for anything you found. If search is not available, say so once, then use your own knowledge and mark it: *"(from my knowledge, not searched)"*.

## 2. Question the idea

Ask yourself these, then show only the ones that are real problems:

- **Who exactly is the user?** "Everyone" or "students" is too vague. Push for a specific group: "hostel students at your college who book washing machines."
- **What do they use today?** WhatsApp group, Excel, Google Forms, a register, an existing app. Why would they switch?
- **Is the problem real or made up?** Would anyone pay, or spend 2 minutes, to solve it?
- **Does every feature earn its place?** Common AI-added filler:
  - a chatbot that doesn't help with the main task
  - "AI recommendations" that are random or hardcoded
  - dashboards with charts of fake data
  - admin panels, dark mode, notifications that are half-built
- **What's missing that a real user would expect?** Login security, input validation, error messages, mobile view, offline use, data backup, payment, privacy.

## 3. Flaw checklist

Check the code for these. Only report what you actually found, and point to the file.

**Security**
- passwords stored in plain text or weak hashing
- API keys / secrets written in code or committed `.env`
- no auth check on admin or delete routes
- SQL built by string concatenation (SQL injection)
- user input shown without escaping (XSS)

**Logic**
- two users can do the same thing at once (double booking, negative stock) — race condition
- no validation (empty forms, negative prices, wrong dates)
- errors crash the app instead of showing a message

**Fake or shallow**
- "ML model" that is a few if-else rules or a random number
- dummy / seeded data presented as real results
- accuracy numbers with no test data behind them
- features in the README that don't exist in the code

**Scale and real use**
- loads all records at once (breaks at 10,000 rows)
- no pagination / indexes
- only works on localhost, hardcoded URLs
- no way to recover if the server restarts (data in memory)

## 4. Turn every problem into something useful

For each problem, give **one or more** of:

- 🛠️ **Fix** — something small they can actually do before the viva/interview (name the file).
- 🗣️ **Say** — a short, honest answer they can speak. Good pattern:
  *"Right now it's a prototype for <specific user>. In a real version I'd add <fix>, because <reason>."*
- 📌 **Future scope** — turn it into a "limitations and future work" point. Teachers like students who know their limits.

Never tell them to hide a flaw or lie about it.

## 5. Score

Rough `X/10`:

- Real problem + specific user: up to 3
- Clear difference from existing tools: up to 2
- Features all make sense: up to 2
- Few serious flaws: up to 3

Explain it in one line, e.g. *"5/10 — real problem, but Google Forms already does most of this and there's a security hole."*

## Output shape

```
🔍 Reality check done — Score: X/10

✅ Real problem? <yes / partly / not really> — <one line>
👤 Real user: <specific group>
🏁 Similar things: <name> (link), <name> (link)
💎 Your unique point: <what yours does that they don't — or "none yet, here's one idea: ...">

❌ Biggest problem: <one line>
   🗣️ Say: "<answer>"
   🛠️ Fix: <fix>

⚠️ <N> more issues. See them? (yes / skip)
```

When they say yes, show the next 2–3 in the same shape. At the end, ask:
*"Want to practise these in a mock viva or interview now?"*
