# Viva prep — full procedure

## Learn mode

Teach in small chunks. After each chunk ask *"Got it? Next: <topic> (yes / ask a question)"*.

1. **2-minute summary** — what they can say out loud when asked "explain your project". Problem → user → how it works → main tech → one thing they're proud of. Under 120 words.
2. **Data flow** — what happens from the user's first click to the result. A short arrow diagram:
   `User fills form → React sends POST /book → Express checks slot → MongoDB saves → confirmation shown`
3. **Key files** — 3–6 files, one or two lines each: what it does and the one function worth knowing.
4. **Why this, not that** — for each main choice (framework, database, auth, hosting, algorithm), one line on why it fits and one line on the main alternative.
5. **Weak spots** — the top 2–3 things from the reality check, with the 🗣️ answers.

Use the student's real file and function names. Plain words first, real term after.

## Mock viva

### Question types

Mix these. Don't stay on one type for more than 2 questions in a row.

| Type | Examples |
|---|---|
| Overview | "Explain your project in 2 minutes." "What problem does it solve?" |
| Why | "Why MongoDB and not MySQL?" "Why did you choose this algorithm?" |
| Code | "Walk me through `bookSlot()` in `routes/booking.js`." "What does this line do?" |
| What-if | "What if two users book the same slot?" "What if the internet goes off?" |
| Change it | "How would you add forgot-password?" "How would you add a second admin?" |
| Real world | "Who will actually use this?" "Google Forms can do this — why your app?" |
| Theory link | See `theory-links.md`. "Which normal form is this table in?" "What's the time complexity here?" |
| Testing | "How did you test it?" "What happens with wrong input?" |
| Honesty | "Which part was hardest?" "Which part did you not write yourself?" |
| Results | "How do you know it works?" "Where does this accuracy number come from?" |

### Flow

1. Start easy (overview), so they warm up.
2. Use the reality-check findings — real examiners ask those.
3. Ask about **specific code** at least every 3rd question. Name the file and function.
4. If the answer is vague, follow up once: *"Can you be more specific? Which file does that?"*
5. Get harder as they get ✅s: why → what-if → change-it → theory.

### Feedback after each answer

```
✅ Good — <one line why>
```
or
```
⚠️ Almost — <what was missing>
💡 Better: "<short model answer, 1–3 sentences>"
```
or
```
❌ Not quite — <one line>
💡 Better: "<short model answer>"
📖 Learn: <file or concept to revise>
```

Then the next question, in the same message. Keep a quiet tally for the final score.

### Common viva traps to prepare them for

- "Show me where that happens in the code." → they must know file names.
- "Change this now." → small live edit (rename a field, add a validation).
- "What's the difference between X and Y?" for tech they used (SQL vs NoSQL, GET vs POST, session vs JWT, props vs state).
- "What's your contribution?" in team projects — they must name their part clearly.
- "Limitations and future scope?" — always have 3 ready.
