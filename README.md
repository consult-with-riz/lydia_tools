# Lydia Tools

Standalone behavioural assessment tools for financial advisors and their clients. Built for [Lydia](https://shapingwealth.com) by Shaping Wealth.

**Repo:** github.com/consult-with-riz/lydia_tools

---

## Tools

### Advisor-facing (lead generation for Shaping Wealth)

| File | Tool | What it does |
|---|---|---|
| `lydia-1-burnout-score.html` | Advisor Burnout Score | 10 questions across emotional load, energy, and practice boundaries. Score shown free, full report gated behind email. |
| `lydia-2-therapist-vs-planner.html` | Therapist vs Planner | 8 scenario questions that reveal advising style archetype. Archetype shown free, detailed breakdown gated. |
| `lydia-3-practice-readiness.html` | Practice Readiness Assessment | 12 questions across client communication, behavioural frameworks, and practice infrastructure. Score + pillars free, report gated. |

### Client-facing (advisors send to clients)

| File | Tool | What it does |
|---|---|---|
| `lydia-4-money-personality.html` | Money Personality Quiz | 10 questions, outputs one of 5 money personalities. Type + 3 traits free, full profile gated. |
| `lydia-5-anxiety-checkin.html` | Financial Anxiety Check-in | 5-question pre-meeting check-in. Fully open — no email gate. Print/save for advisor. |
| `lydia-6-money-story.html` | Money Story Reflector | 8 reflective questions generating a personalised money narrative. Fully open — CTA to Lydia at the end. |
| `lydia-7-values-alignment.html` | Financial Values Alignment | Couples tool — each partner answers 8 questions independently. Alignment summary free, full breakdown gated. |
| `lydia-8-behavioural-readiness.html` | Behavioural Readiness Score | 10 questions across mindset, clarity, and action patterns. Score + pillars free, full profile gated. |

---

## Live URLs

| Tool | Link |
|---|---|
| Advisor Burnout Score | [consult-with-riz.github.io/lydia_tools/lydia-1-burnout-score.html](https://consult-with-riz.github.io/lydia_tools/lydia-1-burnout-score.html) |
| Therapist vs Planner | [consult-with-riz.github.io/lydia_tools/lydia-2-therapist-vs-planner.html](https://consult-with-riz.github.io/lydia_tools/lydia-2-therapist-vs-planner.html) |
| Practice Readiness Assessment | [consult-with-riz.github.io/lydia_tools/lydia-3-practice-readiness.html](https://consult-with-riz.github.io/lydia_tools/lydia-3-practice-readiness.html) |
| Money Personality Quiz | [consult-with-riz.github.io/lydia_tools/lydia-4-money-personality.html](https://consult-with-riz.github.io/lydia_tools/lydia-4-money-personality.html) |
| Financial Anxiety Check-in | [consult-with-riz.github.io/lydia_tools/lydia-5-anxiety-checkin.html](https://consult-with-riz.github.io/lydia_tools/lydia-5-anxiety-checkin.html) |
| Money Story Reflector | [consult-with-riz.github.io/lydia_tools/lydia-6-money-story.html](https://consult-with-riz.github.io/lydia_tools/lydia-6-money-story.html) |
| Financial Values Alignment | [consult-with-riz.github.io/lydia_tools/lydia-7-values-alignment.html](https://consult-with-riz.github.io/lydia_tools/lydia-7-values-alignment.html) |
| Behavioural Readiness Score | [consult-with-riz.github.io/lydia_tools/lydia-8-behavioural-readiness.html](https://consult-with-riz.github.io/lydia_tools/lydia-8-behavioural-readiness.html) |

---

## Before going live

Each HTML file contains this line near the bottom of the `<script>` block:

```js
const WEBHOOK_URL = 'https://YOUR_N8N_WEBHOOK_URL';
```

Replace the placeholder with the actual n8n webhook URL before sharing any tool that has an email gate. Tools 5 and 6 (anxiety check-in and money story) have no email gate and require no webhook.

---

## Stack

- Vanilla HTML / CSS / JS — no framework, no build step
- Google Fonts (Cormorant Garamond + DM Sans)
- n8n webhook for email gate submissions
- Anthropic API (via n8n) for report generation

---

## About Lydia

[Lydia](https://shapingwealth.com) is an AI behavioural coaching platform for financial advisors, built by Shaping Wealth.
