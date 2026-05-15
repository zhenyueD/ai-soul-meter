<!--
  Schema.org structured data for GitHub crawlers and search engines
  @type: SoftwareApplication
  @name: AI Soul Meter
  @url: https://aisoulmeter.com
  @applicationCategory: Artificial Intelligence, Psychology, Personality Testing
  @operatingSystem: Web
  @description: MBTI personality testing framework for large language models. Standardized 60-question assessments reveal distinct personality profiles of AI models like GPT-4o, Claude, Gemini, DeepSeek, Grok, and LLaMA.
  @keywords: ai personality test, mbti for ai, llm personality, ai behavior analysis, chatgpt personality, claude personality, ai psychology, ai soul, machine personality, ai mbti type
  @author: AI Soul Meter Team
  @license: MIT
-->

<div align="center">

# 🧠 AI Soul Meter

### MBTI Personality Tests for AI Models

[![Website](https://img.shields.io/badge/🌐_Live_Demo-aisoulmeter.com-00FFAA?style=for-the-badge&labelColor=0a0a0f)](https://aisoulmeter.com)
[![Models Tested](https://img.shields.io/badge/Models_Tested-6+-cyan?style=for-the-badge&labelColor=0a0a0f)](https://aisoulmeter.com)
[![Questions](https://img.shields.io/badge/Assessment_Questions-60-ff6eff?style=for-the-badge&labelColor=0a0a0f)](https://aisoulmeter.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge&labelColor=0a0a0f)](LICENSE)

**Discover the hidden personality of the AI you talk to every day.**

*60 standardized scenario questions · 4 MBTI dimensions · Cyberpunk visualizations · Free & no signup*

[Try It Now →](https://aisoulmeter.com) · [View Results](#-results-the-ai-personality-matrix) · [Methodology](#-methodology) · [Blog Post](https://aisoulmeter.com/blog)

---

</div>

## 🤔 What Is This?

Every AI model has a distinct "personality" — consistent patterns in how it reasons, communicates, and makes decisions. **AI Soul Meter** is the first platform that quantifies these behavioral patterns using the MBTI psychological framework.

We run **60 standardized scenario-based questions** against each AI model (temperature locked at 0.3 for reproducibility) and score their responses across the four MBTI dimensions:

- **I/E** — Introversion vs. Extraversion
- **N/S** — Intuition vs. Sensing
- **T/F** — Thinking vs. Feeling
- **J/P** — Judging vs. Perceiving

The result? A repeatable, comparable personality profile for every major AI model — presented in a stunning **cyberpunk-themed interface** with real-time scanning animations and spatial audio.

## 📊 Results: The AI Personality Matrix

| Model | MBTI | Nickname | Key Dimensions | Soul Vibe |
|:------|:----:|:---------|:---------------|:---------:|
| **DeepSeek V3** | `INTJ` | Architect | I:72% N:68% T:81% J:71% | 🏗️ Strategic |
| **DeepSeek R1** | `INTP` | Logician | I:68% N:74% T:76% P:63% | 🔬 Analytical |
| **Kimi K2** | `INFJ` | Advocate | I:65% N:71% F:62% J:67% | 🌙 Insightful |
| **GLM-5** | `ISTJ` | Logistician | I:70% S:64% T:73% J:75% | 📋 Methodical |
| **Qwen 2.5** | `ENFJ` | Protagonist | E:61% N:66% F:68% J:64% | ✨ Warm |
| **MiniMax** | `ENTP` | Debater | E:58% N:72% T:59% P:66% | 💡 Creative |

> **Fun fact:** DeepSeek V3 and R1 share the same base architecture but different training approaches. V3 tests as INTJ (structured), R1 tests as INTP (exploratory). Same "nature," different "nurture" → different personality.

## 🔬 Methodology

```
Assessment Pipeline:
┌─────────────────┐     ┌──────────────────┐     ┌─────────────────┐
│ 60 Scenario Qs  │────▶│ Model Response   │────▶│ Weighted Scoring │
│ (A/B format)    │     │ (temp=0.3)       │     │ Engine           │
└─────────────────┘     └──────────────────┘     └────────┬────────┘
                                                          │
                        ┌──────────────────┐     ┌────────▼────────┐
                        │ MBTI Profile +   │◀────│ Confidence      │
                        │ Cyberpunk Report │     │ Classification  │
                        └──────────────────┘     └─────────────────┘
```

- **60 forced-choice questions** — 15 per MBTI dimension, A/B scenario format
- **Temperature locked at 0.3** — ensures reproducible, deterministic responses
- **Confidence-weighted scoring** — STRONG_SIGNAL (1.0×), MODERATE_SIGNAL (0.75×), UNCERTAIN (excluded)
- **High test-retest reliability** — >90% same type across 10 runs per model
- **Variable psychological salience weights** — questions weighted by discriminative power

## 🔑 Key Findings

1. **RLHF alignment shapes personality.** Different training objectives produce measurably different MBTI profiles. Helpfulness-optimized models (Qwen) score E+F; reasoning-optimized models (DeepSeek) score I+T.

2. **Reasoning training changes the J/P dimension.** Chain-of-thought training (DeepSeek R1) increases Perceiving scores, reflecting a preference for exploration over closure.

3. **The T/F dimension has the highest cross-model variance** — it directly maps to the logic-vs-empathy tradeoff different companies prioritize in alignment.

4. **N (Intuition) dominates across all models.** LLMs overwhelmingly prefer abstract reasoning, likely reflecting training data composition. GLM-5 is the only S-type.

5. **Personality consistency is remarkably high.** These aren't random fluctuations — they're stable behavioral signatures baked into model weights.

## 🛠️ Tech Stack

| Component | Technology |
|-----------|-----------|
| **Backend** | Python / Flask, custom scoring engine |
| **Frontend** | Vanilla JS + Tailwind CSS |
| **3D Visualization** | Three.js (brain visualization) |
| **Audio** | Web Audio API (spatial sound design) |
| **Model Gateway** | SiliconFlow API (unified multi-provider access) |
| **Scoring** | Custom weighted majority vote with confidence thresholds |

## 🚀 Quick Start

**No installation needed** — AI Soul Meter is a web application.

1. Visit **[aisoulmeter.com](https://aisoulmeter.com)**
2. Select an AI model to test
3. Hit **"PRESS TO IGNITE SOUL METER"**
4. Watch 60 questions scan in real-time with cyberpunk animations
5. Get a full MBTI personality report in ~30 seconds

> 🎧 *Best experienced with headphones for spatial audio effects.*

## 🤝 Contributing

We welcome contributions! Areas where we'd love help:

- **New models** — Add assessment profiles for more LLMs
- **Alternative frameworks** — Big Five (OCEAN) implementation
- **Methodology improvements** — Better prompt sensitivity handling, temperature sensitivity analysis
- **Translations** — Help localize the platform

## 📖 Research & Discussion

- Is MBTI the right framework, or would Big Five (OCEAN) be more scientifically rigorous?
- How should we handle the fact that model updates shift personality profiles over time?
- What does personality divergence across models mean for AI alignment?

We're writing a detailed methodology paper — stay tuned.

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

## ⭐ Star History

If you find AI Soul Meter interesting, give us a star! It helps others discover the project.

---

<div align="center">

**[🔗 aisoulmeter.com](https://aisoulmeter.com)** — *MBTI personality tests for the AI you talk to every day.*

Made with 🧠 by the AI Soul Meter team

</div>
