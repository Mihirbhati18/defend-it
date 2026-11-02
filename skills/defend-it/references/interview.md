# Interview prep — full procedure

Interviewers ask about projects differently from examiners. They care less about theory and more about: *did you really build this, can you make decisions, and do you think about users?*

## Pick the interview type

Ask once (default: general tech):

| Type | Focus |
|---|---|
| 🚀 Startup | ownership, shipping fast, users, trade-offs, "what would you build next" |
| 🏢 Big tech | depth, scaling, design decisions, edge cases, clean code |
| 🧑‍💼 Service company | fundamentals, clear explanation, teamwork, tech basics behind the stack |
| 🤝 HR round | motivation, teamwork, challenges, learning — little code |

## Question types

| Type | Examples |
|---|---|
| Pitch | "Tell me about this project in 60 seconds." |
| Your role | "What exactly did *you* build?" "What was the hardest part?" |
| Decisions | "Why this database? What else did you consider?" |
| Deep dive | "How does auth work end to end?" "Walk me through what happens when I click Book." |
| Scale | "What if this had 1 million users? What breaks first?" |
| Debugging story | "Tell me about a bug you got stuck on. How did you fix it?" |
| Reflection | "What would you do differently now?" |
| Product sense | "How would you know if users like it?" "Which feature would you remove?" |
| Real world | "Who uses it? Does something like this already exist?" |
| Proof | Follow-ups that check they really built it: exact file, exact error, exact library version |

Use the student's real code and the reality-check findings in questions.

## Feedback

Same ✅ / ⚠️ / ❌ format as viva mode, plus interview-specific tips when relevant:

- **Be specific:** "I used JWT stored in an httpOnly cookie" beats "I did login".
- **Say "I", not "we"** for your own work — but be honest in team projects.
- **Use STAR for stories:** Situation → Task → Action → Result, under 1 minute.
- **Admit gaps well:** "I didn't handle that yet. I'd fix it by ___." is a good answer.
- **Pitch structure:** problem → who → what I built → tech → one result or learning.

## Resume lines

Offer at the end: *"Want 2–3 resume lines for this project?"*

Rules:
- Pattern: **action verb + what you built + how + result**
- Only claim what the code shows. If the student says they did more, ask them, don't assume.
- **No made-up numbers.** If there's a real metric (users, test count, speed measured), use it. Otherwise, describe the scope instead.
- Max 2 lines each.

Example:
- Built a hostel laundry booking web app (React, Express, MongoDB) with JWT login and slot-conflict checks to prevent double bookings.
- Designed REST APIs for booking, cancellation and admin approval; added input validation and error handling across all routes.
