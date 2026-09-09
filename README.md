# AP CSA — Assignment 03: Objects, Strings & Input
**Sessions 9–11 · Oct 5, 6, 7**

Your first objects. Strings turn out to be more interesting than they look, and `Scanner` makes your programs actually interactive.

---

## Exercises

| # | File | Session | What you're doing |
|---|---|---|---|
| 1 | `src/MadLibs.java` | 9 | Concatenation with mixed types |
| 2 | `src/Formatter.java` | 9 | A formatted profile card |
| 3 | `exercises/01-strings.md` | 9 | Concatenation predictions |
| 4 | `src/CharMath.java` | 9 | Chars are secretly numbers |
| 5 | `src/Receipt2.java` | 9 (HW) | Receipt with a *calculated* total |
| 6 | `src/PersonalGreeter.java` | 10 | First Scanner program |
| 7 | `src/InteractiveTip.java` | 10 | Tip calculator, now with input |
| 8 | `src/QuizGame.java` | 10 | Ask, collect, echo |
| 9 | `exercises/02-scanner.md` | 10 | The newline trap |
| 10 | `src/ProjectPrototype.java` | 10 (HW) | Your project's data, live |

---

## The three things that will trip you up

**1. Concatenation goes left to right.**
```java
"Total: " + 5 + 3    →  "Total: 53"
"Total: " + (5 + 3)  →  "Total: 8"
```
Wrap computed values in parentheses. Always.

**2. Strings are immutable.**
```java
name.toUpperCase();          // does nothing visible
name = name.toUpperCase();   // this is what you meant
```

**3. The `nextInt()` / `nextLine()` trap.**
```java
int age = input.nextInt();
input.nextLine();            // ← you need this line
String name = input.nextLine();
```
Without the middle line, `name` comes back empty. Everyone hits this once.

---

## Before you submit
- [ ] All programs run
- [ ] Predictions in `01-strings.md` written **before** running
- [ ] `ProjectPrototype.java` reflects your actual project idea
- [ ] 3+ commits
- [ ] Fork URL in Google Classroom

---

## Coming up
**Session 11:** Unit 1 review · **Session 12:** Unit 1 Test + M1 Proposal due
