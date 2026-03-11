---
description: "Check that TODOs have context: TODO(name): reason"
argument-hint: <python-filepath>
---

Run Ruff's FIX rules to flag bare TODO/FIXME/HACK/XXX comments.

## Steps

1. Run:
   ```
   ruff check --select FIX --output-format text $ARGUMENTS
   ```
2. If ruff is not installed, install it: `pip install ruff --break-system-packages`
3. For each flagged TODO, check if it follows the pattern `TODO(name): reason`.
4. Report any TODOs that lack an author or explanation.
