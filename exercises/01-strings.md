# Exercise 3 — Concatenation Predictions

Predict every result **before** running anything. Be exact — include spaces.

Assume: `int a = 5;  int b = 3;  String s = "Score";  char c = 'A';`

| # | Expression | Predicted | Actual | Right? |
|---|---|---|---|---|
| 1 | `s + a` | | | |
| 2 | `s + a + b` | | | |
| 3 | `s + (a + b)` | | | |
| 4 | `a + b + s` | | | |
| 5 | `a + (b + s)` | | | |
| 6 | `"" + a + b` | | | |
| 7 | `c + 1` | | | |
| 8 | `"" + c + 1` | | | |
| 9 | `(char)(c + 1)` | | | |
| 10 | `s + c` | | | |

---

## Follow-up

**1. Compare #2 and #4. Same three values, opposite order, and the results are structurally different. Explain the rule.**

[your answer]

**2. Why does #7 give `66` instead of `A1`?**

[your answer]

**3. Why does #8 give `A1` when #7 gives `66`? What did the empty string change?**

[your answer]

**4. Write a single line that prints exactly `The total of 5 and 3 is 8` using the variables `a` and `b`.**

```java
// your line here
```

---

## Immutability check

Run this:
```java
String word = "hello";
word.toUpperCase();
System.out.println(word);

word = word.toUpperCase();
System.out.println(word);
```

**1. What did each line print?**

[your answer]

**2. In your own words: what does it mean that Strings are immutable?**

[your answer]

**3. Why is it easy to write `word.toUpperCase();` and think you've changed something? What kind of error is this — syntax, runtime, or logic?**

[your answer]
