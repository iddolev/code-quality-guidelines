---
description: "Check that lines don't exceed ~100 characters"
argument-hint: <python-filepath>
---

Run Ruff's line-length check (E501) configured for 100 chars.

## Steps

1. Run:
   ```
   ruff check --select E501 --line-length 100 --output-format text $ARGUMENTS
   ```
2. If ruff is not installed, install it: `pip install ruff --break-system-packages`
3. Report each over-length line with its line number and current length.
