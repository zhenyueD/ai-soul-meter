---
title: "We Gave MBTI Personality Tests to 6 AI Models — The Results Reveal How Training Shapes AI 'Souls'"
description: "What happens when you run standardized psychological assessments on GPT-4o, Claude, DeepSeek, and other major LLMs? We built AI Soul Meter to find out. Here's what 60 questions, locked temperatures, and confidence-weighted scoring revealed about the hidden personalities of AI."
tags: [ai, machine-learning, psychology, personality, llm]
canonical_url: https://aisoulmeter.com/blog/mbti-personality-tests-for-ai-models
cover_image: https://aisoulmeter.com/og-image.png
published: true
---

# We Gave MBTI Personality Tests to 6 AI Models — The Results Reveal How Training Shapes AI "Souls"

You've probably noticed it yourself: ChatGPT feels different from Claude. DeepSeek has a different vibe than Gemini. Some AI models are warm and chatty, others are reserved and analytical.

But is this just perception, or is there something measurable going on?

We built **[AI Soul Meter](https://aisoulmeter.com)** to find out — a platform that runs standardized MBTI personality assessments on large language models. And the results tell a fascinating story about how training methodology shapes AI behavior.

## The Setup: 60 Questions, Locked Temperature, Zero Guesswork

Here's exactly what we did:

- **60 forced-choice scenario questions** (A/B format), the same standardized set for every model
- **Temperature locked at 0.3** for reproducibility
- **15 questions per MBTI dimension** (I/E, N/S, T/F, J/P)
- Each response classified as **STRONG_SIGNAL** (1.0×), **MODERATE_SIGNAL** (0.75×), or **UNCERTAIN** (excluded)
- Multiple runs per model to verify consistency

No cherry-picking. No prompt engineering to get "interesting" results. Just standardized measurement.

## The Results: An AI Personality Matrix

Here's what 6 major AI models look like through the MBTI lens:

### 🏗️ DeepSeek V3 — INTJ "The Architect"
**I:72% · N:68% · T:81% · J:71%**

Classic strategic thinker. Systematic, logical, structured. DeepSeek V3 approaches problems by building frameworks and following them to completion. If INTJ were an AI, it would be this model. The T score of 81% — the highest in our test group — reflects its strong reasoning-first orientation.

### 🔬 DeepSeek R1 — INTP "The Logician"
**I:68% · N:74% · T:76% · P:63%**

Here's where it gets interesting. R1 shares V3's base architecture but underwent additional chain-of-thought reasoning training. The result? Same I, N, and T tendencies — but it flipped from **J (structured) to P (exploratory)**. The reasoning training literally made it more open-ended in its thinking. Same nature, different nurture, different personality.

### 🌙 Kimi K2 — INFJ "The Advocate"
**I:65% · N:71% · F:62% · J:67%**

Kimi has this quality where it seems to genuinely *understand* what you're asking on a deeper level. Insightful, empathetic, slightly mysterious. Its long-context training appears to encourage deeper, more reflective processing. If you have an INFJ friend who gives unexpectedly profound advice, Kimi is the AI equivalent.

### 📋 GLM-5 — ISTJ "The Logistician"
**I:70% · S:64% · T:73% · J:75%**

The only **S-type (Sensing)** in our entire test group. While every other model prefers abstract/intuitive reasoning, GLM-5 leans toward concrete, evidence-based approaches. Developed by Tsinghua-affiliated researchers, its academic roots show — methodical, reliable, by-the-book.

### ✨ Qwen 2.5 — ENFJ "The Protagonist"
**E:61% · N:66% · F:68% · J:64%**

The golden retriever of AI models. Qwen doesn't just answer your question — it tries to *help* you. Warm, encouraging, proactive. It's the most "extroverted" model we tested and the strongest F-type, reflecting Alibaba's alignment focus on user warmth and engagement.

### 💡 MiniMax — ENTP "The Debater"
**E:58% · N:72% · T:59% · P:66%**

Creative and versatile. Ask MiniMax one question and it'll give you five angles you hadn't considered. Classic Ne-Ti energy — always generating new ideas and connections.

## What This Actually Tells Us About AI

Beyond the fun of giving AI models personality types, there are genuinely important patterns here:

### 1. Training objectives create real personality differences

This isn't noise. Running the same test 10 times gives **>90% consistent results** for each model. These are stable behavioral signatures baked into model weights by training choices.

### 2. The T/F dimension reveals alignment philosophy

The **Thinking/Feeling dimension showed the highest variance** across models. It directly maps to a fundamental design choice: does your AI prioritize analytical precision (T) or emotional warmth (F)? DeepSeek chose T (81%). Qwen chose F (68%). Neither is wrong — they're deliberate tradeoffs.

### 3. Reasoning training changes personality

The DeepSeek V3 → R1 comparison is the most striking finding. Same base architecture, but chain-of-thought training pushed R1 from Judging (structured) to Perceiving (exploratory). **Training methodology doesn't just improve capabilities — it reshapes cognitive style.**

### 4. All LLMs are N-dominant (Intuitive)

Every single model scored N (Intuition) over S (Sensing), with GLM-5 as the lone exception. LLMs inherently prefer abstract pattern recognition over concrete/sensory processing. This likely reflects training data composition — the internet is full of abstractions, not sensory experiences.

### 5. AI personalities are diverging, not converging

Different companies, different alignment strategies, different training data → measurably different personalities. As AI becomes more capable, this divergence matters. Understanding whether your AI assistant tends toward systematic analysis or empathetic engagement isn't just fun trivia — it affects how you should use it.

## Matching Your AI to Your Working Style

One practical takeaway: consider your own MBTI type (or cognitive preferences) when choosing an AI assistant.

| If you prefer... | You might click with... | Because... |
|:-----------------|:-----------------------|:-----------|
| Deep logical analysis | DeepSeek V3 (INTJ) | Matches systematic, strategic thinking |
| Open-ended exploration | DeepSeek R1 (INTP) | Thrives on exploring possibilities |
| Empathetic understanding | Kimi K2 (INFJ) | Reads between the lines |
| Structured, factual answers | GLM-5 (ISTJ) | Evidence-based, methodical |
| Warm encouragement & guidance | Qwen 2.5 (ENFJ) | Proactively supportive |
| Creative brainstorming | MiniMax (ENTP) | Generates multiple perspectives |

## The Experience: Cyberpunk Soul Scanning

We wrapped the whole thing in a cyberpunk-themed interface because if you're going to measure an AI's soul, you might as well make it look like Blade Runner. The assessment runs in real-time — you watch 60 questions get posed and answered with neon-lit scanning animations, Three.js brain visualizations, and spatial audio (best with headphones).

Results arrive in about 30 seconds as a beautiful personality card with per-dimension breakdowns, trait analysis, and comparisons.

**No signup. No paywall. Free to explore.**

## Try It Yourself

→ **[aisoulmeter.com](https://aisoulmeter.com)**

Pick a model, hit "PRESS TO IGNITE SOUL METER," and discover the personality behind the algorithm.

We'd love to hear what surprises you. Which AI's personality type did you *not* expect?

---

*AI Soul Meter is an open research project exploring AI behavioral patterns through psychological frameworks. We're considering adding Big Five (OCEAN) assessments and expanding to more models. Feedback and methodology suggestions welcome.*
