# Preparation sheet — understand GEO in your own words

For the presenters, not for the slides. Read it once and you should be able to explain every slide without notes.

---

## 1. Key notions in plain words

| Notion (EN) | In French | Plain explanation | Example with Decathlon |
|---|---|---|---|
| **GEO** — Generative Engine Optimization | Optimisation pour les moteurs génératifs | Making a brand appear **inside** the answer an AI writes, not just in a list of links | ChatGPT recommends Kalenji shoes when someone asks for beginner running shoes |
| **Generative engine** | Moteur génératif / moteur de réponse | A tool that writes an answer instead of listing links: ChatGPT, Perplexity, Gemini, Copilot, Google AI Overviews / AI Mode | — |
| **RAG** — Retrieval-Augmented Generation | Génération augmentée par la recherche | The AI first **searches** the web, **then** writes using what it found. That is why it can cite sources | Perplexity fetches a running-shoe test from a magazine and quotes it |
| **Query fan-out** | Démultiplication de la requête | The AI splits one question into several smaller searches | "beginner running shoes under €100" → "best cushioning for beginners", "cheap running shoes 2026"… |
| **Citation** | Citation / source citée | A link to your site shown in the answer | A link to decathlon.fr under the answer |
| **Mention** | Mention | Your brand is named, with or without a link | "Decathlon's Kalenji range is a good budget option" |
| **AI share of voice** | Part de voix dans les IA | Your mentions ÷ all tracked brands' mentions, on a set of prompts | Decathlon named 30 times out of 100 brand mentions = 30% |
| **AI Overviews** | Aperçus IA | The AI summary at the top of Google results | — |
| **AI Mode** | Mode IA | Google's conversational search tab, like a chatbot inside Google | — |
| **Crawler / bot** | Robot d'exploration | Program that reads websites for a search engine or AI | OAI-SearchBot (ChatGPT search), PerplexityBot, Googlebot |
| **robots.txt** | Fichier robots.txt | File telling bots what they may read | Blocking OAI-SearchBot = invisible in ChatGPT search |
| **Structured data / Schema.org** | Données structurées | Hidden labels in the page code ("this is a product, this is its price, this is its rating") | Product + Review markup on a Kalenji product page |
| **llms.txt** | — | A proposed file listing your key pages for AI. **Not used by major AIs** according to Google | Low priority |
| **hreflang** | Balise hreflang | Code telling Google "this page is the French version, this one the UK version" | decathlon.fr ↔ decathlon.co.uk |
| **E-E-A-T** | Expérience, expertise, autorité, fiabilité | Google's quality idea: is this content made by people who know and can be trusted? | A coach's advice signed with their name |

### The 30-second pitch (memorise it)
> "SEO gets you ranked; GEO gets you recommended. AI engines search the web, pick a few trusted, clear passages, and write an answer. To be in that answer you must be **retrievable** (bots allowed, pages indexed), **quotable** (clear answers, facts, sources) and **talked about** (press, reviews, forums) — in every language you sell in. Then you measure it: share of voice, citations, sentiment, AI traffic."

### Proven vs supposed (the honesty grid used in the slides)
- **PROVEN**: AI search bots must be allowed (OpenAI and Perplexity say so); Google AI Overviews require indexing; content with sources, quotations and statistics is more visible (Princeton study — in a lab).
- **PARTLY PROVEN**: structured data (helps understanding; no proof of more citations).
- **SUPPOSED**: brand mentions drive AI visibility (strong correlation in Ahrefs data, not proof of cause).
- **DEBATED**: llms.txt.

### The key numbers (all sourced in sources.md)
| Number | What it means | Source |
|---|---|---|
| 22 July 2026 | AI Overviews + AI Mode launch in France | Clubic, Blog du Modérateur |
| 8% vs 15% | Share of Google visits with a click on a result, with vs without AI summary (US, March 2025) | Pew Research Center |
| −58% | CTR of the #1 result when an AI Overview is shown (Dec 2025 data) | Ahrefs |
| +35% | Organic CTR of brands cited in AI Overviews vs not cited (correlation) | Seer Interactive |
| up to +40% | Visibility gain from GEO rewriting methods (lab) | Aggarwal et al., KDD 2024 |
| 0.664 vs 0.218 | Correlation of brand mentions vs backlinks with AI Overview visibility | Ahrefs (75k brands) |
| 200+ countries, 40+ languages | AI Overviews coverage since May 2025 | Google |
| ≈382M | Doubao monthly active users in China (May 2026) | QuestMobile via Diploria |
| 82 / 1,902 | Decathlon countries & regions / stores (2025) | Decathlon press release |
| $199 / $699 per month | Ahrefs Brand Radar: one AI index / all platforms | Ahrefs pricing reviews, Oct 2026 |

---

## 2. The 10 most likely questions — with answer elements

**1. "Isn't GEO just SEO with a new name?"**
Partly, and we say so. Google itself says there is no extra requirement for AI Overviews beyond SEO best practices. What is new: the unit is the passage, not the page; the KPI is mention/citation, not ranking; authority comes more from brand mentions than from links; and you must measure across several engines and languages. → GEO builds on SEO, it doesn't replace it.

**2. "How reliable is the Princeton 40% figure?"**
It is an academic, peer-reviewed study (KDD 2024), but on a **simulated** engine with a fixed set of documents. The direction (sources, quotes, statistics help; keyword stuffing doesn't) is credible; the exact 40% should not be promised to a client. Later research found some effects less robust. That's why we labelled it "proven in a lab".

**3. "Why Decathlon? Did you talk to them?"**
No. We chose Decathlon because it is international (≈82 countries and regions), has its own brands (Kalenji, Quechua) and everyone in class knows it. Its real GEO strategy is not public, so the audit protocol, the plan and the team are **our recommendations**, clearly labelled as such.

**4. "AI answers change all the time — how can you measure anything?"**
Exactly why we use many prompts (50), several languages and engines, and repeat each check (×3). We measure trends and averages (share of voice), never one screenshot. Tools like Ahrefs Brand Radar and Semji automate this daily or monthly.

**5. "Should a brand block AI bots to protect its content?"**
Distinguish two kinds of bots. **Training** bots (GPTBot, Google-Extended): blocking them is a legitimate business choice. **Search** bots (OAI-SearchBot, PerplexityBot): blocking them makes you invisible in those answers. A retailer like Decathlon wants to sell, so it should allow search bots; training is a separate decision.

**6. "Ahrefs or Semji — which would you choose?"**
Depends on the need. Ahrefs Brand Radar is **data-first**: big prompt database, competitor gaps, cited domains — great for a central SEO/GEO team, public pricing from $199/month. Semji is **workflow-first**: tracking plus content production in the brand voice and publishing to the CMS — great for content teams; price on quote. A large group could use both; a smaller one would start with free tools + one paid tool.

**7. "How do you know if AI brings traffic or sales?"**
GA4: create an "AI assistants" channel group (regex on chatgpt.com, perplexity.ai, gemini.google.com, copilot.microsoft.com, claude.ai) placed above Referral, then look at sessions and conversions. Search Console: AI Overviews/AI Mode clicks are inside "Web" data, plus a generative AI impressions report. Bing Webmaster Tools: Copilot citations. Limit: part of AI traffic has no referrer, so this undercounts.

**8. "Why did France get AI Overviews so late?"**
The US had it in May 2024, the UK in August 2024, several EU countries in March 2025. France waited until 22 July 2026; reporting links the delay to European regulation and negotiations with French press publishers. (Say "reported", don't claim to know Google's internal reasons.)

**9. "What about China / non-Western markets?"**
ChatGPT and Gemini are not officially available in mainland China; leaders are Doubao (ByteDance, ≈382M monthly users in May 2026), Qwen and DeepSeek, and search is Baidu. In South Korea Naver is a strong local search engine with its own AI features. In Russia, Yandex (Alice) and GigaChat. → GEO starts by mapping which engines people actually use in each market.

**10. "Isn't GEO manipulation? What are the ethical limits?"**
Legitimate GEO = being clearer, more factual, more present where people talk. Illegitimate: fake reviews, undisclosed sponsored posts, hidden text meant to trick AIs (prompt injection). These are deceptive, can break consumer-protection law, and damage the brand when exposed — and AI vendors work to detect them.

**Backup questions**
- *"What is llms.txt?"* → a proposed file for AIs; Google says no AI system uses it; cheap but not a priority.
- *"Do ads appear in AI Overviews?"* → Google said none in the initial French rollout; elsewhere ads exist in AI features and are expanding. Check before stating a market-specific fact.
- *"What KPI would you show a CEO?"* → AI share of voice vs top 3 competitors, by country, plus revenue from the AI channel in GA4.

---

## 3. Traps to avoid during the oral
- Don't say "ChatGPT uses Google" or "ChatGPT uses Bing" as a fact: engines don't fully publish their retrieval sources.
- Don't compare Pew (8% vs 15%, per visit) and Ahrefs (−58%, per impression) as if they were the same metric.
- Don't present tool prices as definitive: "public price in October 2026, to be checked".
- Don't read the demo results from memory — read what is on screen, or the dated screenshot.
