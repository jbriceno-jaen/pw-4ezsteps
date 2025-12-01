# Playwright Self-Training Program  
_A 4-Step Guided Learning Path With Independent Task Validation_

This document provides a structured, hands-on training flow to help you fully understand a complete Playwright + TypeScript + POM automation framework.

---

# ✅ Step 1 — Environment & Tooling (Checklist)

Before you begin, ensure your environment is ready.

## Required Tools
- Node.js (LTS)
- Git
- VS Code

## Required VS Code Extensions
- Playwright Test for VS Code
- ESLint
- Prettier

## Playwright MCP Setup
- Ensure your ChatGPT/VS Code integration supports MCP tools.
- Confirm **Playwright MCP** is available and allowed to read/write files.
- Test MCP by asking:
  > “Create a Playwright test in this repository that logs in to saucedemo.com.”

---

# ✅ Step 2 — Framework Generation (Prompt)

Run the following prompt with your MCP-enabled assistant to generate the full framework:

```
You are helping me bootstrap a complete Playwright automation framework in this repository.

Requirements:
- Playwright Test
- TypeScript
- Page Object Model (POM)
- Target: https://www.saucedemo.com/
- Structure:
  tests/, pages/, fixtures/, config/

Playwright config:
- Multi-browser: Chromium, Firefox, WebKit
- Parallel workers
- Set baseURL
- Proper retries & timeouts

Pages & tests:
- LoginPage.ts
- login.spec.ts (successful login + assertion)

Tooling:
- ESLint
- Prettier
- .gitignore

CI:
- GitHub Actions workflow running tests with all browsers

Docs:
- README explaining usage & structure

Generate all files with paths and valid TypeScript code.
```

---

# ✅ Step 3 — Self-Training Tasks (Hands-On Learning)

This step contains **independent small tasks**, each with its own **review prompt** so you can validate progress without doing a full project review.

---

## 🧩 **Task 1 — Build Inventory Page + Add-to-Cart Test**

### **Goal**
Create:
- `pages/InventoryPage.ts`
- `tests/add-to-cart.spec.ts`

### **Checklist**
- Add method to add an item to cart  
- Add method to open cart  
- Assert the item appears in the cart  

### **Review Prompt (paste after you finish Task 1)**
```
I just completed Task 1.

Scope:
- pages/InventoryPage.ts
- tests/add-to-cart.spec.ts

Review ONLY these files:
- POM design quality
- Locator quality and robustness
- Test clarity and assertions
- Any test logic leaking into POM?
- Maintainability

Output:
- Summary
- Strengths
- Improvements with examples
- Score from 1–100 for Task 1 only
```

---

## 🧩 **Task 2 — Negative Login Test**

### **Goal**
Create:  
- `tests/login-negative.spec.ts`

### **Checklist**
- Use invalid credentials  
- Assert error message  
- Assert user is NOT redirected  

### **Review Prompt**
```
I completed Task 2: negative login test.

Please review ONLY tests/login-negative.spec.ts.

Focus:
- Test readability
- Proper arranging (arrange-act-assert)
- Correct assertions for negative flow
- Selector quality

Output:
- Assessment
- Recommendations
- Score from 1–100 for Task 2 only
```

---

## 🧩 **Task 3 — Flow Extension + Refactor**

### **Goal**
- Extend login → add to cart → proceed to checkout  
- Refactor duplicated logic into fixtures or helpers  

### **Review Prompt**
```
I completed Task 4: flow extension and refactor.

Scope:
- Updated POM files
- Updated test files
- New helper/fixture files

Focus:
- Was duplication actually reduced?
- Is the flow clear and maintainable?
- Are helpers/fixtures used correctly?

Output:
- Summary
- Praise (what was done well)
- Improvement opportunities
- Score from 1–100 for Task 4 only
```

---

# ✅ Step 4 — (Optional) Final Review

After tasks 1–4 and their individual reviews, you can request a **final holistic review**.

### **Final Review Prompt**
```
Please perform a full, holistic code review of this entire Playwright + TypeScript + POM framework.

Scope:
- playwright.config.ts
- All pages/
- All tests/
- Any fixtures/helpers
- GitHub Actions workflow
- ESLint + Prettier
- README and TRAINING.md

Output:
- High-level summary
- Strengths
- Weaknesses with examples
- Top 5 recommendations
- Final score from 1–100 for the full project
```

---

# 🎉 Congratulations!

This `README.md` file is your fully guided, self-paced Playwright training program with:

- Independent hands-on tasks  
- Per-task review prompts  
- Optional final review  
- Production-ready workflow  
