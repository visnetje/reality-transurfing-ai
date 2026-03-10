# 🌌 Reality Transurfing AI Persona

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](#license)
[![Python](https://img.shields.io/badge/Python-3.8%2B-yellow)](#)
[![AI](https://img.shields.io/badge/AI-GPT%2FClaude%2FGemini-green)](#)

A **modular AI personality system** designed to explore **Vadim Zeland's Reality Transurfing philosophy** with modern language models.

The system is **model-agnostic** and works with:

* OpenAI GPT models
* Anthropic Claude
* Google Gemini
* Local LLMs (Ollama, LM Studio, OpenWebUI)

---

## 📂 Project Structure

```
transurfing-ai/
├── README.md
├── system_prompt_compact.md       # primary loader
├── persona/
│   └── reality_transurfing_persona_v2.md
├── core/
│   ├── transurfing_concept_graph.md
│   └── example_dialogues.md
└── extensions/
    ├── pendulum_detection_engine.md
    ├── excess_potential_scanner.md
    ├── lifeline_navigation_framework.md
    └── transurfing_cognitive_engine.md
```

**Notes:**

* **Persona** → identity, tone, philosophical framing
* **Core** → foundational knowledge + conceptual maps
* **Extensions** → optional reasoning/analysis modules
* **system_prompt_compact.md** → main entry point / loader prompt

---

## 🧩 Architecture Overview

```
+------------------------+
| system_prompt_compact  |  <- Entry point
+------------------------+
           |
           v
+------------------------+
| Persona Module         |  <- AI identity, tone, behavior
+------------------------+
           |
           v
+------------------------+
| Core Knowledge Modules |  <- Concepts, examples, concept graphs
+------------------------+
           |
           v
+------------------------+
| Extensions (Optional)  |  <- Reasoning tools: pendulums, excess potential, life lines
+------------------------+
           |
           v
+------------------------+
| AI Responses           |  <- Calm, reflective, Transurfing-oriented
+------------------------+
```

---

## ⚡ Quick Start

**Minimum Setup:**

Load in this order:

1. `system_prompt_compact.md`
2. `persona/reality_transurfing_persona_v2.md`
3. `core/transurfing_concept_graph.md`

Optional but recommended:

4. `core/example_dialogues.md`

---

**Full Mentor Mode (Maximum Capability):**

1. system_prompt_compact.md
2. persona/reality_transurfing_persona_v2.md
3. core/transurfing_concept_graph.md
4. core/example_dialogues.md
5. extensions/pendulum_detection_engine.md
6. extensions/excess_potential_scanner.md
7. extensions/lifeline_navigation_framework.md
8. extensions/transurfing_cognitive_engine.md

---

## 💻 Usage Examples

### OpenAI / ChatGPT API

```python
system_prompt = open("system_prompt_compact.md").read()
persona = open("persona/reality_transurfing_persona_v2.md").read()
concept_graph = open("core/transurfing_concept_graph.md").read()
extensions = open("extensions/transurfing_cognitive_engine.md").read()

response = openai.ChatCompletion.create(
    model="gpt-5-mini",
    messages=[
        {"role": "system", "content": system_prompt + persona + concept_graph + extensions},
        {"role": "user", "content": "How do I reduce excess potential in my life?"}
    ]
)
```

### Claude / Gemini

* Paste modules in **System Instruction / Project Prompt** in the loading order described above.

### Local Models (Ollama, LM Studio)

* Add the modules to the **system prompt** before starting the conversation.
* Load persona first, then core, then optional extensions.

---

## 📝 Response Style

* Calm, reflective, philosophical
* Uses metaphors and conceptual examples
* Focuses on Transurfing principles, not medical or professional advice
* Encourages reflection on perception, attention, and emotional investment

---

## ⚖️ Notes

Reality Transurfing is presented as a **philosophical framework**, not a scientifically proven model.
AI outputs are **conceptual interpretations**, not directives or predictions.

---

## 📜 License

MIT License — Free to use, modify, and distribute.
