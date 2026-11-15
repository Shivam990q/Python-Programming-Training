# 🎓 GLA University • Python Programming Training
## **Day 2: Tuples, Sets, Dictionaries & Functions — Afternoon Session (3 Hours)**
### **Curriculum: Functions Anatomy, Arguments, LEGB Scope Hierarchy, Closures & Functional Programming (Lambda, Map, Filter, Reduce)**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shivam990q/Python-Programming-Training/blob/main/Day%2002%20-%20Tuples%2C%20Sets%2C%20Dictionaries%20and%20Functions/Day2_Afternoon_Functions_Scope_and_Functional_Programming.ipynb)
[![Training Partner: Edulateral Foundation](https://img.shields.io/badge/Partner-Edulateral%20Foundation-blue.svg?style=for-the-badge)](https://edulateral.com)
[![Institution: GLA University](https://img.shields.io/badge/Institution-GLA%20University-orange.svg?style=for-the-badge)](https://www.gla.ac.in)

---

## 📂 Day 2 Afternoon Package Files
```text
Day 02 - Tuples, Sets, Dictionaries and Functions/
│
├── Day2_Afternoon_Functions_Scope_and_Functional_Programming.ipynb # Master Google Colab Notebook (22 cells, 10 challenges)
├── presentation_visuals.html                                       # 5 Interactive Visual Simulation Labs (100% Light Mode)
├── interactive_mcq_quiz.html                                       # 40 Placement MCQs Exam Engine with Timer & Feedback
├── Python_Day2_Afternoon_Training.pptx                             # 24-Slide 16:9 Light-Themed Executive PowerPoint Deck
├── assets/
│   ├── edulateral_logo.jpg                                         # Official Edulateral branding asset
│   └── logo_b64.txt                                                # Embedded Base64 image
└── README.md                                                       # Trainer & Student Lesson Guide (this document)
```

---

## ⏱️ 3-Hour Session Timeline & Lesson Plan

| Minute Range | Topic Module | Pedagogical Objectives & Live Demonstrations | Key Placement Traps Addressed |
| :---: | :--- | :--- | :--- |
| **00 – 30 min** | **Functions Anatomy & Returns** | `def` keyword, first-class functions, returning multiple values as tuples, PEP 257 docstrings (`__doc__`, `help()`). | Forgetting return returning `None`; treating return tuples as multiple scalar variables. |
| **30 – 70 min** | **Arguments & Packing/Unpacking** | Positional, keyword, default parameters, `*args` tuple packing, `**kwargs` dict packing, positional-only `/` and keyword-only `*`. | **The Mutable Default Trap:** `def f(x=[])` sharing list across calls! |
| **70 – 110 min** | **LEGB Scope & Closures** | Local -> Enclosing -> Global -> Built-in. `global` vs `nonlocal` keywords; lexical scope retention; factory functions and closures. | `UnboundLocalError` on modifying globals; closure late-binding loop trap `[lambda: i for i in range(3)]`. |
| **110 – 140 min** | **Lambda & Higher-Order Sorts** | Syntax: `lambda args: expr`. Conditional lambdas, multi-key sorting with `sorted(..., key=lambda x: (-gpa, backlogs))`. | SyntaxError on using statements like `return` or `for` inside lambda bodies. |
| **140 – 180 min** | **map(), filter(), reduce() & Pipelines** | Lazy generators in Python 3; `filter(None, ...)` truthiness stripping; `functools.reduce()` accumulators; pipeline chaining vs comprehensions. | Performance trade-offs: C-loop `LIST_APPEND` in comprehensions vs function stack overhead. |

---

## 🏆 Top 10 Placement & Exam Traps Quick Reference

1. **The Mutable Default Trap:** Default arguments are evaluated once at definition time. Always use `def f(x=None): if x is None: x = []`.
2. **UnboundLocalError:** Assigning to a variable anywhere in a function body makes it local to the entire function. Use `global` or `nonlocal` before mutating.
3. **Closure Late-Binding Trap:** Lambdas inside loops capture variables by reference, not by value. Use default arguments `lambda i=i: i` to freeze values.
4. **Multiple Returns are Tuples:** `return a, b, c` creates an immutable 3-tuple `(a, b, c)`.
5. **Shortest Iterable in `map()`:** When multiple iterables are provided to `map()`, processing stops at the shortest iterable length.
6. **`filter(None, seq)`:** Strips all falsy values (`0`, `""`, `None`, `False`, `[]`) efficiently.
7. **`reduce()` on Empty Sequences:** Raises `TypeError` unless an initializer value is provided.
8. **Positional-Only vs Keyword-Only:** Parameters before `/` must be positional; parameters after `*` must be keyword-only.
9. **Lambdas Cannot Contain Statements:** `lambda x: return x` is a fatal `SyntaxError`.
10. **Comprehensions vs map/filter:** List comprehensions run in optimized C bytecode without the Python function call frame overhead per item.

---
&copy; 2026 **Edulateral Foundation** • Designed exclusively for GLA University Python Training Programs.
