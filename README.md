# English C-Test

This repository contains three parallel English C-test versions designed to measure contextualised English language proficiency. Each version consists of two short texts in standard C-test format, where the second half of every second word is deleted and must be reconstructed using context.

## Version A
- Missing Computer
- Fear of Flying

**Total gaps:** 40

---

## Version B
- Deforestation
- Pets and Health

**Total gaps:** 40

---

## Version C
- Student Advice
- Job Market

**Total gaps:** 39

---

## Scoring

- One point is awarded for each correctly completed gap.
- Incorrect or unanswered responses receive zero points.
- Scores are reported as both a raw score and a percentage.
- Completion time is recorded separately and does not contribute to the final score.

---

## Data Collection

Results are collected through **Google Apps Script** and stored automatically in a **Google Sheet**.

To use your own spreadsheet:

1. Create a new Google Sheet.
2. Open **Extensions → Apps Script**.
3. Create and deploy a Web App.
4. Copy the Web App URL.
5. Replace the URL in the HTML files inside the `fetch()` function.

Example:

```javascript
await fetch(
    "YOUR_GOOGLE_APPS_SCRIPT_URL",
    {
        method: "POST",
        mode: "no-cors",
        body: JSON.stringify(result)
    }
);
```

---

## References

- Dörnyei, Z., & Katona, L. (1992). *Validation of the C-test amongst Hungarian EFL learners*. Language Testing, 9(2), 187-206.
- Sarapuu, I., & Alas, E. (2016). *Developing a C-test to measure language ability as an alternative to a skills-based test*. Eesti Rakenduslingvistika Ühingu Aastaraamat, 12, 237-252.
