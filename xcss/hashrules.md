# `./hashrules.jsonc`

This approach to using media queries is unconventional but highly flexible, extending beyond media queries to manage very specific, locally scoped selector states. Although it may take some time to understand, its scalability benefits make it worthwhile for large projects.

### Properties

- **Hashrules** define reusable **wrapper-attribute snippets** as key-value pairs.
- Keys are restricted to characters: `A–Z`, `a–z`, `0–9`, and `-`.
- Supports **recursive loading**, allowing inheritance across definitions.
- Use a `hashrule` in a script by embedding `#{___}` within the **wrapper-attribute** of a tag.
- The `hashrule` applies only if the tag already includes a declared style.
- Recursion loops caused by conflicting shorthand definitions are detected, and affected entries are ignored with compilation errors.
- For clarity and to avoid conflicts, any `hashrule` used as a variable should begin with a **`-` prefix**.
- Prefixed **hashrules** are not available during class composition within target folders.

> Be sure to check the practical example in [../tutorial/3.hashrules.md](../tutorial/3.hashrules.md).

---

- Checkout file: [./#at-rules.css](./#at-rules.css)
- Next Chapter: [./#constants.md](./#constants.md)