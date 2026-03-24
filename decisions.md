# decisions.md

## 📌 Purpose of this File
This file defines **decision-centric architecture**.

👉 Why this matters:
- This is the **core artifact**
- Architecture exists to support these decisions
- AI/ML is introduced only at decision points

---

## 🔑 Decision Mapping

| Process Step | Decision | Type | Data Inputs | Output |
|-------------|----------|------|------------|--------|
| Application Intake | Is data complete? | Rule-Based | Application data | Valid/Invalid |
| Eligibility Check | Is applicant eligible? | Rule-Based | Policy rules | Pass/Fail |
| Credit Scoring | What is risk score? | AI/ML | Credit history, financials | Risk score |
| Fraud Detection | Is this fraudulent? | AI/ML | Behavior, device data | Fraud probability |
| Approval Decision | Approve or reject? | Hybrid | Risk score + rules | Decision |
| Disbursement | Release funds? | Rule-Based | Approved application | Payment |

---

## 🧠 Design Principle
Not every decision needs AI.
Use AI only where:
- prediction is required
- patterns are complex

---

## 🧠 How to Use This File with AI
- This file must be referenced for:
  - logical architecture
  - AI integration
  - ADD

Example:
“Create architecture aligned with decisions.md”