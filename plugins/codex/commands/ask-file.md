---
description: Send a file's contents to Codex with an optional question
argument-hint: '[--wait|--background] [--model <model|spark>] [--effort <none|minimal|low|medium|high|xhigh>] <path> [question ...]'
disable-model-invocation: true
allowed-tools: Bash(node:*)
---

!`node "${CLAUDE_PLUGIN_ROOT}/scripts/codex-companion.mjs" ask-file $ARGUMENTS`

Present the full command output to the user.
Do not summarize or condense it.
Preserve any follow-up commands such as `/codex:status <id>` when the run was started in the background.
