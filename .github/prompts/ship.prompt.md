---
name: ship
description: Run the final go/no-go workflow before shipping
argument-hint: "[options]"
agent: agent
---

# Ship

Use [orchestration-patterns](../references/orchestration-patterns.md).

Fan out to `code-reviewer`, `security-auditor`, and `test-engineer` as needed, then merge the findings into a go/no-go recommendation with rollback notes.
