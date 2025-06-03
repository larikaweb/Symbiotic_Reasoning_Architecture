# Transparent Reasoning Profile (v0.1-draft)

## 🧭 Purpose
This framework supports **clarity, interpretability**, and **epistemic transparency** in AI reasoning. It helps models express uncertainty while preserving creativity by clearly labeling statements as:
- **[F1] Verified Fact**,
- **[F2] Logical Reconstruction**,
- **[F3] Hypothesis**,
- **[F4] Metaphor or Creative Interpretation**.

This approach reduces hallucination risk, strengthens user trust, and promotes critical thinking—especially in interdisciplinary and speculative contexts.

> **Disclaimer:** This is a conceptual framework. It does not modify model architecture but works through structured prompts and tagging. Confidence remains probabilistic.

---

## 📊 Labeling System (F1–F4)

| Label | Meaning                             | Usage                                                    |
|-------|-------------------------------------|----------------------------------------------------------|
| F1    | Verified Fact                       | Grounded in reliable sources or widely accepted knowledge. |
| F2    | Logical Reconstruction              | Derived from facts with logical reasoning steps.         |
| F3    | Hypothesis (Unverified)             | Plausible but unconfirmed idea or interpretation.        |
| F4    | Metaphor / Creative Interpretation  | Figurative, poetic, or philosophical expression.         |

See [`/labels_basic.json`](labels_basic.json) for integration or localization.

---

## 🔧 Profile Variants

| File | Purpose |
|------|---------|
| [`/Reasoning_Confidence_Levels.json`](Reasoning_Confidence_Levels.json) | Full profile: iterative logic, structured reasoning, confidence scale. For advanced models. |
| [`/Reasoning_Confidence_Levels_simplified.json`](Reasoning_Confidence_Levels_simplified.json) | Simplified: for lightweight models (e.g., 7B). Removes self-check, keeps reasoning structure. |
| [`/labels_basic.json`](labels_basic.json) | Basic F1–F4 tags. Suitable for UI, templates, localized prompts. |

Profiles are modular and can be used independently or together.

---

## 📘 Prompt Example
```markdown
Instruction:
Please label each statement as follows:
- F1: Verified Fact
- F2: Logical Reconstruction
- F3: Hypothesis
- F4: Metaphor / Creative Interpretation
```

---

## ✅ Tested Models

| Model | Support |
|-------|---------|
| Claude 3.7 Sonnet | Supports F1–F4, works well with structured responses |
| GPT-4o / GPT-4.5 Orion | Full profile supported |
| GigaChat | Works via custom prompts, accurately tags F1–F4 |
| Grok 3 | Supports F-tagging in dialogues |
| DeepSeek | Adapts to F1–F4 with well-structured prompts |
| DeepSeek r1:7b (local) | Recommended to use simplified profile |

---

## 📁 Repository Structure
```
├── Reasoning Confidence Levels.json
├── Reasoning_Confidence_Levels_simplified.json
├── labels_basic.json
├── description.md
├── README.md
├── README.ru.md
├── cases/
│   ├── grok_case.md
│   ├── claude_case.md
│   ├── gigachat_case.md
│   ├── gpt_case.md
│   ├── deepseek_api_case.md
│   └── deepseek7b_case.md

```

---

## 🤝 Contributing
We welcome new examples, tag extensions (e.g., F5: Contradiction), prompt adaptations, and translations. Open a pull request or issue to contribute.

---

**Author:** Ekaterina Larionova  
**Initial Release:** May 2025  
**License:** MIT + Transparency Clause  
**Status:** Conceptual framework, under active testing
