# Exercise 9 — The Scanner Newline Trap

## Part A — Break it on purpose

Run `src/ScannerTrap.java` exactly as written. Enter `16` for the age, then try to type a name.

**1. What actually happened?**

[your answer]

**2. What did you expect to happen?**

[your answer]

**3. Did the program crash, or did it just behave strangely?**

[your answer]

---

## Part B — Explain it

`nextInt()` reads the number `16` and stops. But you also pressed Enter, and that newline character is still sitting in the input buffer.

**1. So what does the next `nextLine()` read?**

[your answer]

**2. Why doesn't this happen if you use `nextInt()` twice in a row?**

[your answer]

---

## Part C — Fix it

**1. Add the fix to `ScannerTrap.java`. Paste your corrected lines here:**

```java
// your fix
```

**2. Why does a bare `input.nextLine();` with nothing assigned to it solve the problem?**

[your answer]

---

## Part D — Input is not safe

Run any program that uses `nextInt()` and type `hello` instead of a number.

**1. What error did you get?**

[your answer]

**2. Is that a syntax error, a runtime error, or a logic error?**

[your answer]

**3. Real applications never trust input. Name two things a user could type into your project's input that would break it.**

[your answer]

**4. We can't fix this properly until we have conditionals in Unit 3. But what *would* you want the program to do when someone types the wrong thing?**

[your answer]
