# 🐧 Madagascar

> *Plugin universe for Claude Code.*

Marketplace of plugins that scaffold, document and keep your project scalable.

## Available plugins

### 🐧 [skipper](https://github.com/c-donnachie/skipper) — The captain

Complete Claude Code framework:

- **Detects your stack** (8 supported stacks: React Vite, Next.js, Expo, Node API, Python FastAPI, all with/without Supabase)
- **Applies an opinionated profile** (CLAUDE.md + docs/architecture/stack.md with structure, naming, libs, SOLID rules)
- **Keeps living docs** (ADRs, PRDs, plans, architecture, business)
- **Specialist subagents** that can refactor:
  - 🐧 Skipper (captain/router)
  - 🐧 Kowalski (docs analyst)
  - 🛠 architect, solid-coach (cross-cutting)
  - 🛠 react-vite, react-native, nextjs, node-backend, supabase (stack-agents)

## Installation

```
/plugin marketplace add c-donnachie/madagascar
/plugin install skipper@madagascar
/reload-plugins
```

Then in any project:

```
/skipper:init-structure          # detect stack and scaffold docs/
/skipper:scan                    # see what stack you have
/skipper:stack-apply <id>        # apply opinionated profile
/skipper:ask "..."               # captain routes to specialist
/skipper:react-vite "..."        # invoke specialist directly
/skipper:update                  # kowalski updates docs from diff
```

## Why "Madagascar"?

Skipper is the captain. Kowalski analyzes ("Kowalski, analysis"). In the future: Rico for aggressive refactor, Private for tutorials/lookups. Madagascar is the place where they all live.

Each plugin in the marketplace can be a standalone add-on. The core is **skipper** (install that and you have the full framework). The rest will be optional.

## Roadmap

- **v1.x** — More stacks (Astro, SvelteKit, Tauri, Remix) based on real demand
- **future** — Optional add-ons (`private`, `rico`)
- **goal** — Submission to Anthropic's official marketplace

## License

MIT
