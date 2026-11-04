# Question template

Every question asked MUST be rendered from this template. In chat, replace `<id>`, `<short-title>`, `<question>`, and the recommendation list.

```markdown
### Q<id>: <short-title>

**Question:** <question>

**Recommendations:**

1. <strongest recommendation>
2. <second-strongest recommendation>
3. <recommendation>
   ...
```

Rules:

- `<id>` is the sequential question number (`Q1`, `Q2`, `Q3`, ...). Ids are never reused; each new round continues the sequence.
- `<short-title>` is a concise title for the question.
- `<question>` is the full question, self-contained and unambiguous.
- Recommendations are ordered by strength: the lower the number, the stronger the recommendation (`1` is the strongest).
