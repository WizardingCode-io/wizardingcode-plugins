# wizardingcode-plugins

The plugin marketplace of [WizardingCode](https://wizardingcode.io)'s tools for coding agents. One repository, read by Claude Code and by Codex.

**Claude Code**

```sh
claude plugin marketplace add WizardingCode-io/wizardingcode-plugins
claude plugin install wizardingcode-mem@wizardingcode-plugins
```

**Codex**

```sh
codex plugin marketplace add WizardingCode-io/wizardingcode-plugins
codex plugin add wizardingcode-mem@wizardingcode-plugins
```

| Plugin | What it does |
|---|---|
| [wizardingcode-mem](https://github.com/WizardingCode-io/wizardingcode-mem) | Persistent memory across sessions, shared by every agent you use: what one session learns, the next one is told. One local binary, no daemon, no LLM in the loop. |
| [wizardingcode-developer-crew](https://github.com/WizardingCode-io/wizardingcode-developer-crew) | Guided delivery for Claude Code where done is proven, not claimed: a deterministic engine detects the project, records test-first, runs the real build, tests and checks, and holds the turn until the evidence says the work is done. Claude Code only, for now. |

Each plugin lives in its own repository; this marketplace points at a released version of it. For Gemini CLI, OpenCode and Cursor, see the plugin's own README. The developer crew is in the Claude Code marketplace only; Codex sees the memory plugin.

Until October 2026 this marketplace was `shibaox-plugins` and the memory plugin `shibaox-mem`. If you have it, install `wizardingcode-mem` as above: on its first run it takes over the old one's memories, and `wizardingcode-mem install` removes the old plugin.
