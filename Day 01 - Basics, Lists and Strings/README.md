# 🎓 GLA University &bull; Python Programming Training
## **Day 1: Python Basics, Lists and Strings &mdash; Afternoon Session (3 Hours)**
### **Curriculum: List Comprehensions, Companion Built-ins, Strings Deep Dive, 23 Methods & Modern Formatting**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shivam990q/Python-Programming-Training/blob/main/Day%2001%20-%20Basics%2C%20Lists%20and%20Strings/Day1_Basics_Lists_and_Strings.ipynb)
[![Live Web Portal](https://img.shields.io/badge/Live%20Web%20Portal-Interactive%20Slides%20%26%20MCQs-brightgreen.svg?style=for-the-badge)](https://shivam990q.github.io/Python-Programming-Training/)
[![Training Partner: Edulateral Foundation](https://img.shields.io/badge/Partner-Edulateral%20Foundation-blue.svg?style=for-the-badge)](https://edulateral.com)
[![Institution: GLA University](https://img.shields.io/badge/Institution-GLA%20University-orange.svg?style=for-the-badge)](https://www.gla.ac.in)
[![Python Version: 3.8+](https://img.shields.io/badge/Python-3.8%2B-green.svg?style=for-the-badge)](https://python.org)

---

## 📂 Package Directory Structure
```text
Python Programming Training/
│
├── index.html                      # Interactive Course Portal & Launchpad (GitHub Pages)
├── presentation_visuals.html       # Visual Presentation Deck (24 slides) + 5 Interactive Visual Labs
├── interactive_mcq_quiz.html       # 35 Placement-Grade MCQs with instant feedback & analytics
├── Day1_Basics_Lists_and_Strings.ipynb  # Complete Google Colab Jupyter Notebook
├── assets/
│   ├── edulateral_logo.jpg         # Official Edulateral Foundation branding asset
│   └── logo_b64.txt                # High-density Base64 URI for self-contained portability
├── loop_state.json                 # Ralph loop persistence & verification state
└── README.md                       # Complete Trainer & Student Guide (this document)
```

---

## ⏱️ 3-Hour Session Timeline & Pedagogical Lesson Plan

| Minute Range | Topic Module | Pedagogical Objectives & Live Demonstrations | Key Placement Traps Addressed |
| :---: | :--- | :--- | :--- |
| **00 &ndash; 15 min** | **Orientation & Course Architecture** | Set high energy; contrast imperative C/Java style loops with declarative Pythonic list comprehensions; explain CPython bytecode optimization (`LIST_APPEND`). | Understanding why Python code can be cleaner AND faster. |
| **15 &ndash; 35 min** | **List Comprehensions Mastery** | Syntax formula: `[expr for item in iterable if cond]`. Filtering vs Value Substitution. | **Trap:** Writing `[x for x in nums if x > 2 else 0]` (Fatal SyntaxError!). |
| **35 &ndash; 60 min** | **Nested Comprehensions & 2D Grids** | Flattening 2D matrices row-by-row; matrix transposition; multiplication tables; companion built-ins: `sorted(key=len)`, `enumerate(start=1)`, `zip(*matrix)` unzip idiom. | **Trap:** `list.sort()` returns `None` vs `sorted()` returning a new list. |
| **60 &ndash; 70 min** | **Interactive Visual Lab 1 & 2** | Switch to `presentation_visuals.html` -> Launch **List Comp Pipeline Simulator**; step through live data streams. | Visualizing filtering vs accumulator stages. |
| **70 &ndash; 90 min** | **Strings: Literals, Escape Sequences & Memory** | Single, double, triple quotes, and raw strings `r"..."`. Escape sequences (`\n`, `\t`, `\r`, `\b`, `\\`). CPython memory model: why strings are immutable in memory; `id()` pointer reassignment. | **Trap:** Carriage return `\r` overwriting characters; `TypeError` on in-place mutation. |
| **90 &ndash; 115 min** | **Indexing & Boundary-Safe Slicing** | Dual-directional indexing (0 to $N-1$ and $-1$ to $-N$); slicing formula `s[start:stop:step]`; negative step `s[::-1]`. | **Trap:** `s[100]` raises `IndexError`, but `s[2:100]` is boundary-safe. Directional mismatch returning `""`. |
| **115 &ndash; 125 min** | **Interactive Visual Lab 3 & 4** | Launch **Interactive Slicing Ruler** & **Memory Immutability Lab**; students manipulate live sliders to predict slices. | Eliminating index boundary anxiety. |
| **125 &ndash; 155 min** | **The 23 Essential String Methods & Formatting** | 18 core methods + 5 advanced methods (`center`, `zfill`, `partition`, `isalnum`, `isspace`). String formatting: `%` vs `str.format()` vs modern `f-strings` with alignment (`<`, `>`, `^`), precision (`.2f`), thousands separators (`,`), and debug syntax (`{x=}`). | **Trap:** `title()` with apostrophes (`It'S`); `find()` (-1) vs `index()` (`ValueError`); `strip()` stripping sets of chars. |
| **155 &ndash; 180 min** | **Hands-On Colab Challenges & MCQ Exam** | Students open Colab notebook to solve 10 progressive challenges; conclude with 35-question timed assessment in `interactive_mcq_quiz.html`. | Validating end-to-end placement readiness. |

---

## 🎯 Syllabus & Method Coverage Checklist

### 1. List Comprehensions & Companions
- [x] Basic syntax `[expression for item in iterable]`
- [x] Condition filtering `[x for x in nums if condition]`
- [x] Ternary value substitution `[val1 if cond else val2 for item in iterable]`
- [x] Nested list comprehensions (matrix flattening, 2D generation)
- [x] `sorted(iterable, key=lambda, reverse=True)` vs `list.sort()`
- [x] `enumerate(iterable, start=1)` clean index tracking
- [x] `zip(*iterables)` parallel iteration, truncation rules, and unzipping idiom

### 2. Strings Deep Dive
- [x] String literals: single (`'`), double (`"`), triple (`'''` / `"""`), and raw strings (`r"..."`)
- [x] Escape sequences: `\n`, `\t`, `\r` (carriage return overwrite), `\b`, `\\`, `\xhh`, `\uhhhh`
- [x] Immutability: CPython memory model, `id()`, pointer rebinding, TypeError on item assignment
- [x] Indexing: 0-based forward, -1 negative indexing, `IndexError` conditions
- [x] Slicing: `s[start:stop:step]`, defaults, negative step `s[::-1]`, boundary clipping, directional mismatch
- [x] String operations: Concatenation (`+`), Repetition (`*`), Membership test (`in`, `not in`)

### 3. The 18 Core String Methods
- [x] `upper()` &mdash; All characters to uppercase
- [x] `lower()` &mdash; All characters to lowercase
- [x] `title()` &mdash; Title case (with apostrophe non-word boundary caveat)
- [x] `capitalize()` &mdash; Capitalizes first char, forces ALL others lowercase
- [x] `swapcase()` &mdash; Inverts uppercase and lowercase
- [x] `strip()` &mdash; Trims whitespace or custom character set from both ends
- [x] `lstrip()` &mdash; Trims leading whitespace or custom characters
- [x] `rstrip()` &mdash; Trims trailing whitespace or custom characters
- [x] `split()` &mdash; Splits by delimiter (`sep=None` whitespace collapsing vs explicit sep, `maxsplit`)
- [x] `join()` &mdash; Joins iterable with delimiter (`TypeError` if elements are not strings)
- [x] `replace()` &mdash; Replaces occurrences of old with new (optional count)
- [x] `find()` &mdash; Returns lowest index of substring, returns **-1** if not found
- [x] `index()` &mdash; Like `find()`, but raises **`ValueError: substring not found`**
- [x] `count()` &mdash; Counts **non-overlapping** occurrences of substring
- [x] `startswith()` &mdash; Validates prefix (accepts a tuple of candidate prefixes)
- [x] `endswith()` &mdash; Validates suffix (accepts a tuple of candidate suffixes)
- [x] `isdigit()` &mdash; Checks digits only (returns `False` for negatives and decimals)
- [x] `isalpha()` &mdash; Checks alphabet characters only

### 4. Other String Methods & Formatting
- [x] `center(width, fillchar)` &mdash; Centers string padded with custom fill character
- [x] `zfill(width)` &mdash; Sign-aware zero padding from left
- [x] `isalnum()` &mdash; Alphanumeric validation
- [x] `isspace()` &mdash; Checks exclusively whitespace characters (returns `False` on empty string)
- [x] `partition(sep)` &mdash; Splits into guaranteed 3-tuple `(before, sep, after)`
- [x] `%` operator formatting &mdash; Legacy C-style `%s`, `%.2f`
- [x] `str.format()` &mdash; Positional `{0}` and keyword `{name}` placeholders
- [x] `f-strings` &mdash; Modern Python 3.6+ inline expressions, formatting specs (`:.2f`, `:,`, `:>12`, `:^12`, `:08b`), and Python 3.8+ debug specifier `f"{x=}"`

---

## 🚀 How to Run the Deliverables

### 1. Presentation Deck & Interactive Visual Labs (`presentation_visuals.html`)
- Double-click `presentation_visuals.html` or open in any web browser (Chrome, Edge, Firefox, Safari).
- **Keyboard Shortcuts:**
  - `Right Arrow` / `Space`: Next slide
  - `Left Arrow`: Previous slide
  - `F`: Toggle full-screen presentation mode
  - `N`: Toggle Trainer/Speaker Notes drawer
  - `O`: Open 24-slide visual grid overview
- Switch between **Presentation Deck** and **Interactive Visual Labs** at the top bar to use the live Slicing Ruler, List Comprehension Pipeline Simulator, Memory Immutability Inspector, 23 Methods Explorer, and F-String Studio!

### 2. Interactive MCQ Assessment Engine (`interactive_mcq_quiz.html`)
- Open in any modern web browser.
- **Features:**
  - **Practice Mode:** Select answers and click *Check Answer* for instant pedagogical explanations breaking down why the correct option is right and why distractors are traps.
  - **Timed Exam Mode:** 35-minute countdown timer with auto-submit and complete performance scorecard.
  - **Topic Filters:** Filter dynamically by *List Comprehensions*, *Built-in Utilities*, *Strings & Slicing*, *String Methods*, or *Formatting & Traps*.
  - **Bookmark:** Flag questions for later review.

### 3. Google Colab Notebook (`Day1_Basics_Lists_and_Strings.ipynb`)
- **Option A (Google Colab):**
  1. Go to [Google Colab](https://colab.research.google.com).
  2. Click **Upload** -> Select `Day1_Basics_Lists_and_Strings.ipynb`.
  3. Run the cells step-by-step from top to bottom.
- **Option B (Local Jupyter Lab / VS Code):**
  ```bash
  pip install jupyter
  jupyter lab Day1_Basics_Lists_and_Strings.ipynb
  ```
- Contains complete runnable demonstrations for every topic and **10 automated unit-tested coding challenges**!

---

## 🏆 Top 10 Placement & Exam Traps Quick Reference

1. **The Trailing Else Trap:** `[x for x in nums if x > 2 else 0]` is a `SyntaxError`. In-place value selection requires the ternary syntax before the for loop: `[x if x > 2 else 0 for x in nums]`.
2. **Slicing Boundary Safety:** `s[100]` raises `IndexError: string index out of range`, but `s[100:]` safely returns an empty string `""`.
3. **Empty String Substring Rule:** `"" in s` evaluates to `True` for EVERY string `s`, including `"" in ""`.
4. **Join on Non-Strings:** `"-".join([1, 2, 3])` raises `TypeError`. You must pass strings: `"-".join([str(x) for x in [1, 2, 3]])`.
5. **Find vs Index:** `s.find("abc")` returns `-1` when absent; `s.index("abc")` raises `ValueError: substring not found`.
6. **Title Case Apostrophes:** `"it's".title()` returns `"It'S"` because the apostrophe is treated as a word boundary.
7. **Character Validation on Empty Strings:** All `is...()` methods (`isdigit()`, `isalpha()`, `isspace()`) return `False` on an empty string `""`.
8. **Strip Set Semantics:** `s.strip("an")` strips any combination of `'a'` and `'n'` from both ends, NOT the substring `"an"`.
9. **Directional Mismatch Slicing:** When `step < 0`, `start` must be greater than `stop`. `s[1:5:-1]` yields `""`.
10. **Sort vs Sorted:** `list.sort()` mutates in-place and returns `None`. `sorted()` returns a new list and leaves the original untouched.

---
&copy; 2026 **Edulateral Foundation** &bull; Ideate &bull; Innovate &bull; Integrate  
*Designed exclusively for GLA University Python Training Programs.*
