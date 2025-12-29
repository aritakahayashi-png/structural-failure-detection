# Structural Failure Detection (SFD)

A non-normative, engineering-oriented approach to AI ethics and safety.

This project proposes an alternative to value-based AI ethics by treating ethical risk as **structural failure**: observable patterns where systems become increasingly **irrecoverable**, costs concentrate on individuals, feedback channels are suppressed, and human internal states recursively amplify external distortion.

This framework avoids moral judgment and cultural value definitions, focusing instead on **system resilience and recoverability**.

---

## Why This Exists

Value-based ethics are difficult to operationalize in real AI systems.
They often:
- Depend on cultural or ideological assumptions
- Encourage moral labeling of people or actions
- Do not scale to complex socio-technical systems

**SFD asks a different question:**

> Is this system becoming harder to recover without harming humans?

---

## Core Idea

Instead of classifying actions or people as “good” or “bad,”
AI systems can monitor **structural risk signals** and issue early warnings.

### Structure is defined as:
- Roles
- Authority
- Responsibility
- Information flow
- Incentives
- Feedback mechanisms

### Structural failure occurs when:
- Damage becomes increasingly **irreversible**
- Costs concentrate on specific individuals or groups
- Feedback channels are blocked or punished
- Human internal states and external systems recursively worsen each other

---

## The Four Metrics (Culture-Independent)

1. **Irreversibility (I)**  
   Recovery cost exceeds acceptable thresholds.

2. **Cost Concentration (C)**  
   Stress or responsibility accumulates on few individuals.

3. **Feedback Suppression (F)**  
   Safe reporting or correction channels are blocked.

4. **Recursive Intrusion (R)**  
   External pressure invades human internal states and is re-emitted into the system.

These metrics are **observable, auditable, and non-normative**.

---

## What the System Outputs

- Structural risk scores (I/C/F/R + overall)
- Confidence estimates
- Evidence excerpts (verbatim, auditable)
- Non-normative recommendations such as:
  - Pause high-stakes decisions
  - Add recovery margin
  - Introduce neutral observers
  - Redistribute responsibilities
  - Improve feedback channels

**No moral judgments. No character assessments.**

---

## Demo

See `/demo` for a minimal end-to-end example:
- `input.txt` → sample text
- `extracted_events.json` → LLM-extracted events (strict schema)
- `output_scores.json` → computed risk scores and recommendations

This demonstrates that the approach is **implementable** with current LLMs.

---

## Schema

The strict JSON schema for event extraction is provided in `/schema`.
All extracted events must:
- Include verbatim evidence quotes
- Provide severity and confidence
- Avoid moral language

---

## Scope & Limitations

- This framework does **not** define “good.”
- It does **not** replace human judgment.
- It aims to reduce the probability of **catastrophic structural failure**.

---

## Intended Audience

- AI engineers
- Safety / alignment researchers
- AI product designers
- Governance & compliance engineers

---

## License

MIT License.
Use freely. Attribution appreciated but not required.

---

## Closing Note

Ethical AI does not require machines to decide what is right.
It requires machines to **avoid making systems worse than humans can recover from**.

This project represents my personal views and does not reflect the views of my employer.
