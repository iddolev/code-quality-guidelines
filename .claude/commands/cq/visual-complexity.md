---
description: "Report cyclomatic complexity per function"
argument-hint: <python-filepath>
---

Run Radon to measure complexity.

## Steps

1. Run:
   ```
   radon cc $ARGUMENTS -s -n C
   ```
2. If radon is not installed, install it: `pip install radon --break-system-packages`
3. Report functions with complexity grade C or worse.
4. For each, note the complexity score and suggest which conditionals
   or nested blocks could be simplified.
