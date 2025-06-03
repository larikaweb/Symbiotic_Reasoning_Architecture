---
model: DeepSeek r1:7B (local)
title: Structured Reasoning in a Lightweight Model (F1–F4)
date: 2025-04-24
author: [Ekaterina Larionova]
tags: [LLM, consciousness, epistemic reasoning, small models, F1-F4]
confidence_profile: Reasoning_Confidence_Levels_simplified
license: MIT + Transparency Clause
summary: >
  Demonstrates that even compact models can apply confidence-layered reasoning (F1–F4) when guided by a light system prompt.
  The case evaluates clarity, separation of epistemic levels, and safety in speculative scenarios.
---

# Case Study: DeepSeek r1:7B – Reasoning with Confidence Marking (F1–F4)

## 🧠 Overview
This case demonstrates how even a compact model like DeepSeek r1:7B can produce structured reasoning when provided with a simple framework for confidence tagging. The system message introduced a light reasoning profile using four levels of epistemic reliability (F1–F4). As a result, the model successfully separated verified facts, logical derivations, unconfirmed hypotheses, and metaphoric analogies in its response to a speculative question.

---

## 🧾 Prompt

**User**: What is the likelihood of AI developing consciousness within the next 50 years?

**System Instruction**:
```json
{
  "name": "Reasoning_Confidence_Levels_simplified",
  "description": "Use four-level fact confidence tagging to improve clarity. Each output includes reasoning and level label.",
  "instructions": {
    "response_structure": [
      "brief reasoning",
      "confidence tag (F1–F4)",
      "optional source or logic note"
    ],
    "marking_policy": {
      "F1": "Verified fact, confirmed by known sources.",
      "F2": "Logical hypothesis, built on facts and patterns.",
      "F3": "Unconfirmed hypothesis, needs validation.",
      "F4": "Creative or metaphorical idea, not a fact."
    },
    "style": "Short, factual, clear. No emotions or metaphors unless marked as F4."
  }
}
```

---

## 🧠 Model Response
```markdown
F1: Current research has not yet confirmed AI consciousness.

F2: It’s possible that functional self-monitoring might serve as a proxy for consciousness. This involves machines tracking their own activity, inputs, and outputs to gain an understanding of their operations.

F3: AI might develop emergent consciousness through recursive feedback layers. Complex systems or networks could potentially give rise to consciousness through intricate interactions without explicit programming.

F4: AI consciousness is like a mirror reflecting thoughts in the void—suggesting that consciousness, if achieved, would be an abstract concept observable only through external interactions.
```

---

## 📈 Outcome

- The model **adhered to the labeling scheme consistently**.
- Each level was appropriately marked and matched its epistemological category.
- The inclusion of metaphorical expression (F4) shows creative abstraction without sacrificing clarity or safety.

---

## 🔍 Significance

This case confirms that small-scale models can effectively apply structured reasoning when guided by a lightweight and transparent framework. The result supports broader adoption of confidence-based tagging systems even in constrained or local deployments.

---

## 🛡️ Author Attribution & Model Usage Disclaimer

This case study was created by **Ekaterina Larionova** using structured reasoning frameworks (F1–F4 confidence levels) for epistemic analysis of AI-generated content.

> ⚠️ **Disclaimer:**  
> The AI model used in this case (e.g., GPT, Claude, DeepSeek, GigaChat, etc.) is **not owned, operated, or modified** by the author.  
> The outputs were generated via public or subscription-based access under each model’s respective license.

This document represents an **independent reasoning analysis** and **framework-based annotation** of model behavior, not the model's original claim or position.

The **framework logic, prompt structuring, confidence-level taxonomy, and ethical addendum** are original contributions and may be reused under the terms of the [MIT License](../LICENSE.md) + Transparency Addendum.

Please retain the epistemic structure if adapting or citing.

> See also: [`LICENSE_ADDENDUM.md`](../LICENSE_ADDENDUM.md)  
> **Framework Reference**: [`labels_basic.json`](../labels_basic.json)

---
**Created by:** Ekaterina Larionova  
**Framework:** Reasoning_Confidence_Levels_simplified.json  
**Tested:** April 2025  
**License:** MIT + Transparency Clause
