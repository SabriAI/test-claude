# Demo & workshop script

Step-by-step script for the opening demo (slide 2) and the live workshop (slide 19).
Language: English (the oral is in English). Prompts in other languages are given verbatim.

---

## 0. Preparation (the week before — 30 min, whole group)

| When | What | Who |
|---|---|---|
| D-7 | Create the Google Form (questions in §2.2) and its linked Google Sheet | P5 |
| D-7 | Generate the Form's QR code (Form › Send › link › copy, then any free QR generator, or Chrome › share › QR code) and paste it on slide 19 in place of the QR icon | P5 |
| D-7 | **Rehearsal run**: each member runs the workshop prompt in 1 language × 3 engines and fills the Form → this is your Plan B data | All |
| D-7 | Take the demo screenshots (§1.3) and save them in a `demo-backup/` folder + on a USB key | P1 |
| D-1 | Re-run the demo prompts once (answers change), update screenshots if needed | P1 |
| D-day | Laptop logged into ChatGPT, two browser tabs pre-opened, phone hotspot ready | P1 |

> Write the **date** of every screenshot on it. AI answers change; a dated screenshot is honest evidence, an undated one is not.

---

## 1. Opening demo — slide 2 (1 min 15)

### 1.1 Set-up
- Browser: ChatGPT open on chatgpt.com. Use **a fresh chat** (or a temporary chat) so the history does not influence the answer.
- If possible, turn **off memory / personalisation** for the demo account.
- Zoom the browser to 125–150% so the room can read.

### 1.2 Exact prompts

**Tab 1 — English**
```
What are the best running shoes for beginners under €100?
```

**Tab 2 — French (new chat)**
```
Quelles sont les meilleures chaussures de running pour débuter à moins de 100 € ?
```

### 1.3 What to observe and say (read from the screen, never invent)
1. **Is Decathlon or Kalenji named?** Point at it, or say clearly "Decathlon is not mentioned".
2. **Position**: first, middle, last, or absent?
3. **Sources**: which websites are cited (click the source chips)? Local (French) or international (US/UK) sites?
4. **Difference between EN and FR**: same brands? same order? same sources?

Possible punchline depending on what appears:
- If Decathlon appears in FR but not EN: *"Same question, two languages, two different shop windows."*
- If it appears in both: *"Good for Decathlon — but look at the sources: who is the AI trusting?"*
- If it appears in neither: *"For this user, one of Europe's biggest sports retailers doesn't exist."*

### 1.4 Plan B (no Wi-Fi / ChatGPT down / login problem)
1. Switch immediately to the dated screenshots in `demo-backup/` (EN and FR side by side).
2. Say: *"We ran this on [date] — answers change, which is itself a GEO lesson."*
3. Do not wait more than 15 seconds for a slow page.

---

## 2. Live workshop — slide 19 (5 min)

### 2.1 The task
Pairs, one phone per pair. Each pair asks the **same question** in **their native language** in whichever assistant they have (ChatGPT, Gemini, Perplexity, Copilot, Google AI Mode…).

**Reference prompt (English)**
```
I'm a beginner and want to start running. Which shoes should I buy for under €100, and where?
```

**Ready-made translations** (show on screen or in the Form description)
- FR: `Je débute la course à pied. Quelles chaussures acheter pour moins de 100 €, et où ?`
- ES: `Soy principiante y quiero empezar a correr. ¿Qué zapatillas debería comprar por menos de 100 € y dónde?`
- DE: `Ich bin Anfänger und möchte mit dem Laufen anfangen. Welche Laufschuhe sollte ich für unter 100 € kaufen, und wo?`
- IT: `Sono principiante e voglio iniziare a correre. Quali scarpe dovrei comprare con meno di 100 € e dove?`
- PT: `Sou iniciante e quero começar a correr. Que sapatilhas devo comprar por menos de 100 € e onde?`
- Other languages: students translate themselves (that's part of the exercise).

> The words "and where?" matter: they push the AI to name **retailers**, so Decathlon has a chance to appear as a shop and not only through its Kalenji brand.

### 2.2 Google Form questions (copy exactly)
1. **Language of your prompt** — short answer (e.g. FR, EN, ES…)
2. **AI used** — multiple choice: ChatGPT / Gemini / Perplexity / Copilot / Google AI Mode / Other
3. **Is Decathlon or one of its brands (Kalenji, etc.) mentioned?** — Yes / No
4. **If yes, in which position among the brands or shops named?** — 1 / 2 / 3 / 4 / 5+ / not mentioned
5. **Other brands or shops named** — short answer
6. **First source cited (website name)** — short answer, "none" if no source
7. **Tone towards Decathlon** — Positive / Neutral / Negative / Not mentioned

### 2.3 Google Sheet — results tab (prepare the formulas before D-day)
Assuming answers land in the `Form Responses 1` sheet with column B = language, C = AI, D = mentioned (Yes/No):

- Overall mention rate:
  `=COUNTIF('Form Responses 1'!D:D;"Yes")/COUNTA('Form Responses 1'!D2:D)`
- Mention rate by language: in a `Results` tab, list the languages in A2:A10 and put in B2:
  `=IFERROR(COUNTIFS('Form Responses 1'!B:B;A2;'Form Responses 1'!D:D;"Yes")/COUNTIF('Form Responses 1'!B:B;A2);"")`
- Same by AI engine: list engines in D2:D7 and use the same formula on column C.
- Insert a **bar chart** on each table before D-day so it updates live.

> Depending on your Google Sheets locale, the separator is `;` (French locale) or `,` (English locale).

### 2.4 Timing
| Time | Presenter (P5) says / does |
|---|---|
| 0:00 | "Phones out, pair up. Scan the QR code." |
| 0:30 | "Ask this exact question in your native language, in any AI you have. We need at least one pair in English and one in French." |
| 1:00 – 3:00 | Students run the prompt and fill the Form. Other group members walk around and help. |
| 3:00 | "Last 20 seconds, submit now." Switch the projector to the `Results` tab. |
| 3:20 – 4:30 | Comment: *In which language is Decathlon most visible? Which engine? Which competitors keep coming back? Are the sources local or global?* Link back to slides 9–11. |
| 4:30 – 5:00 | Bonus: "One action Decathlon should take in your country, based on what you saw?" Take 2–3 answers. |

### 2.5 What the class should learn (say it out loud at the end)
- They have just run a **real GEO audit** — the same method as Ahrefs or Semji, done by hand.
- Results **differ by language and by engine** → one test is never enough.
- The cited **sources** are the to-do list: those are the sites where Decathlon must be present.

### 2.6 Plan B
| Problem | Fallback |
|---|---|
| No network for students | Show the rehearsal results (D-7) in the Sheet and ask the class to interpret them |
| Form/QR doesn't work | Students shout their answers; P4 types them into the Sheet |
| Too few answers | Merge with rehearsal data, clearly say "including our rehearsal data" |
| Running late | Skip the bonus question; keep the results comment (it is the key learning) |
