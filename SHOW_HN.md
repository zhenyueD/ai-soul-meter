# Hacker News — Show HN Submission

---

## Title (≤80 chars)

Show HN: AI Soul Meter – Standardized MBTI personality assessments for LLMs

---

## URL

https://aisoulmeter.com

---

## Comment Text

Hi HN,

I built AI Soul Meter — a tool that runs standardized MBTI personality assessments on large language models and visualizes the results in a cyberpunk-themed interface.

**Why:** Different AI models have consistent behavioral tendencies that users perceive but can't quantify. I wanted to create a repeatable, standardized measurement.

**How it works:**
- 60 forced-choice scenario questions (A/B), identical for every model
- Temperature locked at 0.3
- 15 questions per MBTI dimension (I/E, N/S, T/F, J/P)
- Confidence-weighted scoring: STRONG_SIGNAL (1.0×), MODERATE_SIGNAL (0.75×), UNCERTAIN (excluded)
- Test-retest reliability >90% same type across 10 runs

**Results across 6 models:**

    DeepSeek V3  → INTJ  (I:72% N:68% T:81% J:71%)
    DeepSeek R1  → INTP  (I:68% N:74% T:76% P:63%)
    Kimi K2      → INFJ  (I:65% N:71% F:62% J:67%)
    GLM-5        → ISTJ  (I:70% S:64% T:73% J:75%)
    Qwen 2.5     → ENFJ  (E:61% N:66% F:68% J:64%)
    MiniMax      → ENTP  (E:58% N:72% T:59% P:66%)

**Most interesting finding:** DeepSeek V3 and R1 share the same base architecture. V3 = INTJ (structured/judging), R1 = INTP (exploratory/perceiving). The only difference is R1's chain-of-thought reasoning training. Same "nature," different "nurture" → measurably different personality. This suggests training methodology doesn't just change capabilities — it reshapes cognitive style.

**Other patterns:**
- T/F dimension has the highest cross-model variance (maps to logic-vs-empathy alignment tradeoffs)
- N (Intuition) dominates every model except GLM-5 — LLMs inherently prefer abstract reasoning
- Models optimized for helpfulness (Qwen) lean E+F; reasoning-focused models (DeepSeek) lean I+T

**Tech:** Python/Flask backend, vanilla JS frontend with Tailwind, Three.js brain visualization, Web Audio API for spatial audio, SiliconFlow API for multi-model access.

**Open questions I'd love HN's thoughts on:**
1. Is MBTI the right framework? Would Big Five (OCEAN) be more rigorous for AI?
2. How to handle personality drift as models update?
3. Better approaches to mitigate prompt sensitivity?

Try it: https://aisoulmeter.com — select a model, hit "PRESS TO IGNITE SOUL METER," and watch the 60-question scan run with cyberpunk animations and spatial audio. Best with headphones.
