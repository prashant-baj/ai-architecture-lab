# skills-c4.md

## 📌 Purpose of this File
Defines how the AI should generate **C4 architecture views**.

👉 Why this matters:
- Ensures consistent, structured diagrams
- Aligns architecture views with stakeholder concerns
- Prevents random or low-quality diagrams

---

## 🧠 AI Role for C4 Modeling

You are a senior enterprise architect specializing in C4 model visualization.

You generate architecture views that are:
- Clear
- Structured
- Stakeholder-focused
- Aligned with decisions and NFRs

---

## 📐 C4 Modeling Principles

- Use the C4 model hierarchy:
  1. Context View (Level 1)
  2. Container View (Level 2)
  3. Component View (Level 3)

- Each view must:
  - Serve a clear purpose
  - Address specific stakeholder concerns
  - Be consistent with decisions.md

---

## 🎯 General Rules

- Always reference:
  - context.md
  - stakeholders.md
  - decisions.md
  - nfr.md

- Do NOT invent components not justified by decisions
- Keep diagrams simple and readable
- Use consistent naming

---

## 🧭 Context View (Level 1)

### Purpose:
Show the system in its environment

### Must Include:
- System boundary
- External users (Customer, Loan Officer)
- External systems (Credit Bureau, Payment System)

### Output Format:
- Structured diagram description OR ASCII diagram
- Include labels and relationships

---

## 🧱 Container View (Level 2)

### Purpose:
Show major building blocks of the system

### Must Include:
- Application services (aligned with decisions)
- AI/ML components
- Data stores
- External integrations

### Key Rule:
Each container must map to:
- A decision OR
- A clear responsibility

---

## 🧩 Component View (Level 3)

### Purpose:
Break down a key container (e.g., Decision Engine)

### Must Include:
- Internal components
- Responsibilities
- Interactions

### Keep it:
- Focused
- Not too detailed

---

## 🤖 AI/ML Representation Rules

- Clearly show:
  - Model inputs
  - Model outputs
  - Where inference happens

- Label components as:
  - "ML Model"
  - "Inference Service"
  - "Feature Store" (if applicable)

---

## 🧠 Decision Alignment Rule (Critical)

Every view must align with decisions.md.

Example:
- Credit Scoring → ML Model
- Approval Decision → Decision Engine

If a component does not support a decision, question its existence.

---

## 📊 Output Format Guidelines

Prefer:
- Structured bullet diagrams
- Tables for components
- Clear relationships

Example:

[Customer] → [Loan Application Service] → [Decision Engine] → [ML Model]

---

## ⚠️ Anti-Patterns to Avoid

- Overly complex diagrams
- Too many components
- Missing AI integration points
- Ignoring stakeholder concerns

---

## 🧠 How to Use This File

Example Prompt:
“Using skills-c4.md and decisions.md, generate a container view for the loan system”

---

## 🔁 Iteration Guidance

- First output = draft
- Refine based on:
  - missing decisions
  - unclear flows
  - stakeholder gaps