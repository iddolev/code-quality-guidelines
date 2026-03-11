---
description: "Check for deeply nested blocks (>3 levels)"
argument-hint: <python-filepath>
---

Run Pylint's too-many-nested-blocks check.

## Steps

1. Run:
   ```
   pylint --disable=all --enable=R1702 --max-nested-blocks=3 $ARGUMENTS
   ```
2. If pylint is not installed, install it: `pip install pylint --break-system-packages`
3. For each violation, report the function name, line number, and nesting depth.
4. Do NOT refactor. Only report. Suggest which inner block could be
   extracted to a helper function.
