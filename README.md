
# 🎥 Tinyflix QA Assessment

## 🛠 Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/testpress/tinyflix-qa.git
   ```
2. **Navigate to the project directory:**
   ```bash
   cd tinyflix-qa
   ```
3. **Install dependencies:**
   ```bash
   npm install
   ```
4. **Start the development server:**
   ```bash
   npm run dev
   ```
5. **Run automated tests:**
   ```bash
   npx cypress open
   ```

---

## 📑 Submission Overview

| Section | Description |
|---------|-------------|
| **1. Bug Report** | Prioritized list of 10+ verified bugs with severity, steps, screenshots, and suggested fixes |
| **2. Test Plan** | Functional, edge case, and UI test cases with expected and actual results |
| **3. Test Implementation** | Cypress-based automated tests for critical UI and flows |
| **4. Accessibility Report** | WCAG-based findings with 94/100 Lighthouse score, touch target & heading hierarchy fixes |
| **5. Performance Report** | Analysis using Lighthouse with 78/100 score, optimizations recommended |
| **6. README.md** | Setup guide, project summary, and reviewer instructions |

---

## 📈 Summary of Findings

- ✅ **Total Bugs Identified:** 11
- ❌ **Critical Issues:** Video playback failure, unresponsive authentication buttons
- ⚠️ **UX/UI Issues:** Bookmark formatting, mobile layout misalignment, thumbnail inconsistencies
- 🔐 **Security Risk:** Comment input accepts unsanitized special characters (XSS potential)
- ♿ **Accessibility Score:** 94/100 — small touch targets, heading order issues
- 🚀 **Performance Score:** 78/100 — unminified JS, no preload on LCP image, no caching

---

## ✅ Automation Testing Summary

- **Tool:** Cypress
- **Total Automated Tests:** 7
- **Test Coverage:** Home page, sorting, commenting, mobile layout, input validation
- **How to Run:**  
  - `npx cypress open` (GUI)  
  - `npx cypress run` (headless)

---

## 🧩 Assumptions & Limitations

- Auth system is not implemented, so login/signup buttons do not function
- Video files are not present in `/public/videos`, causing playback to fail
- Data is hardcoded or mocked — no live API integration
- Performance and accessibility metrics are based on localhost (Vite Dev Server), not production

---

## 🙏 Acknowledgement

This report was prepared with professional-level QA standards to demonstrate real-world testing skills, bug identification, automation, and reporting. Thank you for reviewing this assessment.

---

## 📂 Folder Structure (Recommended Submission)

```
Tinyflix-QA-Assessment/
│
├── Bug Analysis Report.docx
├── TestPlan.docx
├── accessibility-report.md
├── performance-report.md
├── README.md
├── TestImplementation/
│   ├── tinyflix.cy.js
│   ├── test-results.md
│   └── run-instructions.txt
```
