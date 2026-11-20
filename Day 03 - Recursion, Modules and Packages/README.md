# 🎓 GLA University • Python Programming Training
## **Day 3: Recursion, Modules and Packages — Afternoon Session (3 Hours)**
### **Curriculum: Inbuilt Functions, Module Architecture, math (12), time (8), os (12), random, datetime & NumPy Foundations**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shivam990q/Python-Programming-Training/blob/main/Day%2003%20-%20Recursion%2C%20Modules%20and%20Packages/Day3_Recursion_Modules_and_Packages.ipynb)
[![Training Partner: Edulateral Foundation](https://img.shields.io/badge/Partner-Edulateral%20Foundation-blue.svg?style=for-the-badge)](https://edulateral.com)
[![Institution: GLA University](https://img.shields.io/badge/Institution-GLA%20University-orange.svg?style=for-the-badge)](https://www.gla.ac.in)

---

## 📂 Day 3 Afternoon Package Files
```text
Day 03 - Recursion, Modules and Packages/
│
├── Day3_Recursion_Modules_and_Packages.ipynb # Master Google Colab Notebook (22 cells, 10 challenges)
├── presentation_visuals.html                                   # 5 Interactive Visual Simulation Labs (100% Light Mode)
├── interactive_mcq_quiz.html                                   # 40 Placement MCQs Exam Engine with Timer & Feedback
├── Python_Day3_Afternoon_Training.pptx                         # 24-Slide 16:9 Light-Themed Executive PowerPoint Deck
├── assets/
│   ├── edulateral_logo.jpg                                     # Official Edulateral branding asset
│   └── logo_b64.txt                                            # Embedded Base64 image
└── README.md                                                   # Trainer & Student Lesson Guide (this document)
```

---

## ⏱️ 3-Hour Session Timeline & Lesson Plan

| Minute Range | Topic Module | Pedagogical Objectives & Live Demonstrations | Key Placement Traps Addressed |
| :---: | :--- | :--- | :--- |
| **00 – 30 min** | **Inbuilt Functions & Banker's Rounding** | `eval()` security risks; `range()` memory efficiency; IEEE 754 Banker's Rounding in `round()`. | Expecting `round(2.5)` to be 3 (it is 2!). Code injection via `eval()`. |
| **30 – 65 min** | **Modules, Namespaces & Packages** | Import styles (`import`, `from-import`, `as`); `sys.modules` cache; `__name__ == '__main__'`; package `__init__.py`. | Wildcard imports `from m import *` silently shadowing local variables. |
| **65 – 100 min** | **math (12 funcs) & random Modules** | The 12 core math functions (`sqrt`, `ceil`, `floor`, `gcd`, `log`, etc.); `random.seed()` deterministic testing; `randint()` boundary rules. | `randint(1, 10)` including BOTH 1 and 10 vs `range(1, 10)` excluding 10. |
| **100 – 140 min** | **time (8 funcs), os (12 funcs) & datetime** | High-resolution profiling with `perf_counter()`; cross-platform path management with `os.path.join()`; `timedelta` date arithmetic. | Path crashes on Windows (`\`) vs Linux (`/`); `time.time()` vs `perf_counter()`. |
| **140 – 180 min** | **NumPy & Vectorized Computing** | Contiguous C-memory `ndarray`; vectorization without loops; 2D reshaping (`reshape(-1)`); axis aggregations. | Reshaping arrays with mismatched dimensions; understanding `axis=0` vs `axis=1`. |

---

## 🏆 Top 10 Placement & Exam Traps Quick Reference

1. **Banker's Rounding:** `round(2.5) == 2` and `round(3.5) == 4` (Rounds half to the nearest even number).
2. **`random.randint(a, b)`:** Both endpoints `a` and `b` are INCLUSIVE, unlike `range(a, b)`.
3. **`os.path.join`:** Always join filesystem paths using `os.path.join()` to prevent cross-OS separator bugs.
4. **`perf_counter()` for Benchmarking:** Never use `time.time()` for micro-benchmarks; use `time.perf_counter()`.
5. **`float('nan') == float('nan')` is `False`:** By IEEE 754, NaN is not equal to itself. Always use `math.isnan()`.
6. **`math.sqrt()` with Negatives:** Raises `ValueError: math domain error`. Use `cmath.sqrt()` for complex roots.
7. **Wildcard Imports:** `from module import *` pollutes the namespace and can cause subtle variable shadowing.
8. **NumPy Reshape Dimension `-1`:** Passing `-1` tells NumPy to automatically calculate the remaining dimension.
9. **`random.shuffle()` Mutates In-Place:** Returns `None`, not a new list.
10. **`date` vs `datetime`:** `date` stores year-month-day only; `datetime` stores down to microsecond precision.

---
&copy; 2026 **Edulateral Foundation** • Designed exclusively for GLA University Python Training Programs.
