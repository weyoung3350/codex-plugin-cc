---
description: Send arbitrary text or a prompt to Codex without requiring a code review target
argument-hint: '[--wait|--background] [--prompt-file <path>] [--model <model|spark>] [--effort <none|minimal|low|medium|high|xhigh>] [text ...]'
disable-model-invocation: true
allowed-tools: Bash(node:*)
---

!`node "${CLAUDE_PLUGIN_ROOT}/scripts/codex-companion.mjs" ask $ARGUMENTS`

Present the full command output to the user.
Do not summarize or condense it.
Preserve any follow-up commands such as `/codex:status <id>` when the run was started in the background.
