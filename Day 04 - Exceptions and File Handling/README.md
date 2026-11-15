# 🎓 GLA University • Python Programming Training
## **Day 4: Exceptions and File Handling — Afternoon Session (3 Hours)**
### **Curriculum: open(), Context Managers, 8 File Modes (r, w, a, r+, rb, wb), 10 Methods (seek, tell, truncate) & CSV/Binary Persistence**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shivam990q/Python-Programming-Training/blob/main/Day%2004%20-%20Exceptions%20and%20File%20Handling/Day4_Afternoon_File_Handling_and_Persistence.ipynb)
[![Training Partner: Edulateral Foundation](https://img.shields.io/badge/Partner-Edulateral%20Foundation-blue.svg?style=for-the-badge)](https://edulateral.com)
[![Institution: GLA University](https://img.shields.io/badge/Institution-GLA%20University-orange.svg?style=for-the-badge)](https://www.gla.ac.in)

---

## 📂 Day 4 Afternoon Package Files
```text
Day 04 - Exceptions and File Handling/
│
├── Day4_Afternoon_File_Handling_and_Persistence.ipynb # Master Google Colab Notebook (22 cells, 10 challenges)
├── presentation_visuals.html                          # 5 Interactive Visual Simulation Labs (100% Light Mode)
├── interactive_mcq_quiz.html                          # 40 Placement MCQs Exam Engine with Timer & Feedback
├── Python_Day4_Afternoon_Training.pptx                # 24-Slide 16:9 Light-Themed Executive PowerPoint Deck
├── assets/
│   ├── edulateral_logo.jpg                            # Official Edulateral branding asset
│   └── logo_b64.txt                                   # Embedded Base64 image
└── README.md                                          # Trainer & Student Lesson Guide (this document)
```

---

## ⏱️ 3-Hour Session Timeline & Lesson Plan

| Minute Range | Topic Module | Pedagogical Objectives & Live Demonstrations | Key Placement Traps Addressed |
| :---: | :--- | :--- | :--- |
| **00 – 30 min** | **File Architecture & Context Managers** | `open()`, OS file descriptors, `__enter__` / `__exit__`, `with` statement, explicit UTF-8 encoding. | Leaked file descriptors on unhandled exceptions; `UnicodeDecodeError` on Windows cp1252. |
| **30 – 65 min** | **The Complete 8-Mode Matrix** | `r`, `w`, `a`, `r+`, `w+`, `a+`, `rb`, `wb`. Overwriting vs appending vs creating. | **The 'w' Mode Trap:** opening in `'w'` wipes the file to 0 bytes instantly before writing! |
| **65 – 110 min** | **10 Core Methods: seek(), tell(), truncate()** | `read()`, `readline()`, `readlines()`, `write()`, `writelines()`, `seek(offset, whence)`, `tell()`, `flush()`, `close()`, `truncate()`. | `writelines()` not appending `\n`; `seek()` in text mode only supporting `whence=0` for non-zero offsets. |
| **110 – 145 min** | **CSV Parsing & Binary Streams** | `csv.reader`, `csv.writer(newline='')`, `csv.DictReader`, bytes serialization, chunked buffering. | Blank rows on Windows without `newline=''`; memory exhaustion reading multi-GB files. |
| **145 – 180 min** | **10 Hands-On Challenges & Placement Quiz** | 10 automated unit-tested coding tasks and 40 placement MCQs with instant feedback. | End-to-end placement readiness validation. |

---

## 🏆 Top 10 Placement & Exam Traps Quick Reference

1. **The 'w' Mode Trap:** Mode `'w'` truncates the file to 0 bytes immediately upon opening.
2. **Always Use `with` Statement:** Guarantees `f.close()` is executed even during unhandled exceptions.
3. **`newline=''` in CSV Writing:** Omitting `newline=''` on Windows creates blank lines between CSV rows.
4. **`writelines()` Does NOT Append `\n`:** You must explicitly append `\n` to strings.
5. **Memory-Efficient File Reading:** Use `for line in f:` rather than `f.readlines()` on large files.
6. **`f.tell()` Returns Byte Offset:** Returns byte integer offset, not character or line count.
7. **`f.read()` at EOF:** Returns empty string `""` without raising errors.
8. **Closed File I/O Trap:** Accessing `f.read()` outside the `with` block raises `ValueError: I/O operation on closed file`.
9. **`seek()` in Text Mode:** Non-zero offsets relative to current (1) or EOF (2) are forbidden in Python 3 text streams.
10. **Binary Mode Types:** `'rb'` and `'wb'` strictly process `bytes` objects, not strings.

---
&copy; 2026 **Edulateral Foundation** • Designed exclusively for GLA University Python Training Programs.
