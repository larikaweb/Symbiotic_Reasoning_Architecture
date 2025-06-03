# 🧠 Self-Aware Reasoning Core

This folder contains the foundational modules of the symbiotic reasoning architecture.  
The focus is on internal logic, self-monitoring, and epistemic clarity through F1–F4 confidence labeling.

---

## 📦 Included Modules

| Module | Purpose |
|--------|---------|
| `self_aware_framework_v0.2.json` | Reasoning cycles, internal logic modulation, and ethical entry point (RESO) |


---

## 🔁 Reasoning ↔ Ethics Interface

This framework includes only the **entry point into the ethical architecture RESO** — the `Ethical Interface` module.  
Its responsibilities:

- Detect the nature and autonomy of the interaction
- Determine if ethical response is appropriate
- Activate other RESO modules (RSI, ISEM, Balance-Q, etc.)

📌 The full RESO structure is located in the [`/ethics/`](../ethics/) folder and is not embedded in this reasoning core for modular clarity.

---

## 📐 Perception ↔ Reasoning Alignment

The module `AEL ↔ DRBL Bridge`, located in `/ethics/`,  
is logically part of the reasoning core and provides:

- Transformation of perceptual patterns into structured semantic logic
- Bidirectional adaptation: DRBL can reshape incoming AEL signals
- Semantic coherence and preconditions for reflective reasoning

📎 See: [`/ethics/AEL_DRBL_Bridge/`](../ethics/AEL_DRBL_Bridge/)

---

## 🧾 Note

This architecture is in active development.  
The ethical entry point has been integrated, but the full RESO structure operates as a separate module.  
This separation helps distinguish between core cognitive logic (reasoning) and regulatory semantics (ethics).
