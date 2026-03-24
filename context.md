# context.md

## 📌 Purpose of this File
This file defines the **business context, scope, and constraints** of the system.

👉 Why this matters:
- This is the **foundation for all architecture artifacts**
- Every AI prompt should reference this file
- Ensures all outputs are aligned to the same problem

---

## 🏢 Business Context
We are designing a digital loan approval system for a financial institution.

Current challenges:
- High manual effort in loan processing
- Slow approval cycles (days instead of seconds)
- Higher default rates due to rule-based scoring
- Lack of intelligent decisioning

---

## 🎯 Business Goals
- Enable near real-time loan approval
- Improve credit risk assessment accuracy
- Reduce operational cost
- Ensure regulatory compliance and auditability

---

## 📦 System Scope
Include:
- Loan application intake
- Validation
- Credit scoring
- Approval decisioning
- Disbursement

Exclude:
- Core banking ledger systems (assume external)
- Third-party integrations implementation details

---

## ⚠️ Constraints
- Must comply with financial regulations
- Decisions must be explainable
- High availability required
- Sensitive customer data must be protected

---

## 🧠 How to Use This File with AI
- Always load/reference this file before generating:
  - architecture views
  - decisions
  - ADD
- Example:
  “Using context.md, generate a system context diagram...”