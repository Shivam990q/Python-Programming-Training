# 🎓 GLA University • Python Programming Training
## **Day 5: Regex and Projects — Afternoon Session (3 Hours)**
### **Curriculum: 6 Capstone Placement Projects Hands-on Implementation**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shivam990q/Python-Programming-Training/blob/main/Day%2005%20-%20Regex%20and%20Projects/Day5_Afternoon_Capstone_Placement_Projects.ipynb)
[![Training Partner: Edulateral Foundation](https://img.shields.io/badge/Partner-Edulateral%20Foundation-blue.svg?style=for-the-badge)](https://edulateral.com)
[![Institution: GLA University](https://img.shields.io/badge/Institution-GLA%20University-orange.svg?style=for-the-badge)](https://www.gla.ac.in)

---

## 📂 Day 5 Afternoon Package Files
```text
Day 05 - Regex and Projects/
│
├── Day5_Afternoon_Capstone_Placement_Projects.ipynb # Master Google Colab Notebook (25 cells, 6 complete projects)
├── presentation_visuals.html                        # 6 Interactive Capstone Project Simulators (100% Light Mode)
├── interactive_mcq_quiz.html                        # 40 Placement Architecture MCQs with Timer & Feedback
├── Python_Day5_Afternoon_Training.pptx              # 24-Slide 16:9 Light-Themed Executive PowerPoint Deck
├── assets/
│   ├── edulateral_logo.jpg                          # Official Edulateral branding asset
│   └── logo_b64.txt                                 # Embedded Base64 image
└── README.md                                        # Trainer & Student Lesson Guide (this document)
```

---

## ⏱️ 3-Hour Session Timeline & Lesson Plan

| Minute Range | Topic Module | Pedagogical Objectives & Live Demonstrations | Key Placement Traps Addressed |
| :---: | :--- | :--- | :--- |
| **00 – 30 min** | **Project 1: Contact Book Application** | JSON CRUD file operations, case-insensitive substring search, 10-digit phone number assertion. | `KeyError` on deletion; atomic JSON saves using context managers. |
| **30 – 65 min** | **Project 2: Student Grade Analyzer** | Functional data pipelines: `map()` for record transformation, `filter()` for honors filtering, `reduce()` for class averages and topper finding. | In-place mutations vs immutable functional data transformations. |
| **65 – 105 min** | **Project 3: Interactive Quiz Engine** | `random.sample()` for non-repeating question pools, scoring algorithms, timestamped persistent leaderboard logging. | Question repetition with `random.choices()`; trailing newlines in log files. |
| **105 – 140 min** | **Project 4: Multi-Category Expense Tracker** | CSV persistence with `csv.DictReader` and `writerows()`, category dictionary aggregation, budget warning logic. | Omitting `newline=''` creating double line breaks on Windows. |
| **140 – 160 min** | **Project 5: Regex Forensic Log & Email Validator** | Compiling regex with `re.compile()`, email RFC pattern matching, phone validation, parsing Apache/Nginx web server logs. | Recompiling regex patterns inside loops; `match()` vs `search()` semantics. |
| **160 – 180 min** | **Project 6: ATM & Banking Simulation System** | User-defined custom exception hierarchies (`InsufficientFundsError`, `InvalidPinError`), 3-attempt PIN lockout, stateful transactions. | Catching `BaseException` vs `Exception`; passing forensic parameters to error classes. |

---

## 🏆 Top 10 Placement & System Design Traps Quick Reference

1. **Custom Exceptions Must Inherit from `Exception`:** Never inherit from `BaseException` (which catches system interrupts like Ctrl+C).
2. **`json.dump()` vs `json.dumps()`:** `dump(obj, f)` writes to a file; `dumps(obj)` returns a string.
3. **Precompile Regular Expressions:** Always use `re.compile()` for regex patterns executed in high-throughput loops.
4. **`re.match()` vs `re.search()`:** `match()` only looks at index 0; `search()` scans the entire string.
5. **Safe Dictionary Removal:** Use `dict.pop(key, None)` instead of `del dict[key]` to avoid unhandled `KeyError`.
6. **Unique Sampling:** `random.sample()` guarantees sampling without replacement.
7. **Clean Subtotal Accumulation:** Use `dict.get(key, 0.0) + amount` to avoid initializing missing keys manually.
8. **Always Pass `newline=''` to CSV on Windows:** Prevents blank lines between rows.
9. **Private Attribute Encapsulation:** Use `_attribute` to signal private state and expose mutation via validation methods.
10. **The `finally` Block:** Always executes to clean up resources regardless of whether an exception was raised.

---
&copy; 2026 **Edulateral Foundation** • Designed exclusively for GLA University Python Training Programs.
