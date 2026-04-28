# 🐧 Madagascar

> *Universo de plugins para Claude Code.*

Marketplace de plugins que arman tu proyecto, lo documentan y lo mantienen escalable.

## Plugins disponibles

### 🐧 [skipper](https://github.com/c-donnachie/skipper) — El capitán

Framework completo de Claude Code:

- **Detecta tu stack** (8 stacks soportados: React Vite, Next.js, Expo, Node API, Python FastAPI, todos con/sin Supabase)
- **Aplica perfil opinado** (CLAUDE.md + docs/architecture/stack.md con estructura, naming, libs, reglas SOLID)
- **Mantiene docs vivos** (ADRs, PRDs, planes, architecture, business)
- **Sub-agentes especialistas** que pueden refactorizar:
  - 🐧 Skipper (capitán/router)
  - 🐧 Kowalski (analista de docs)
  - 🛠 architect, solid-coach (transversales)
  - 🛠 react-vite, react-native, nextjs, node-backend, supabase (stack-agents)

## Instalación

```
/plugin marketplace add c-donnachie/madagascar
/plugin install skipper@madagascar
/reload-plugins
```

Después en cualquier proyecto:

```
/skipper:init-structure          # detecta stack y arma docs/
/skipper:scan                    # ver qué stack tienes
/skipper:stack-apply <id>        # aplica perfil opinado
/skipper:ask "..."               # capitán enruta a especialista
/skipper:react-vite "..."        # invoca especialista directo
/skipper:update                  # kowalski actualiza docs según diff
```

## ¿Por qué Madagascar?

Skipper es el capitán. Kowalski analiza ("Kowalski, análisis"). En el futuro: Rico para refactor agresivo, Private para tutoriales/lookups. Madagascar es el lugar donde viven todos.

Cada plugin del marketplace puede ser un add-on independiente. El núcleo es **skipper** (instalas eso y tienes el framework completo). Los demás serán opcionales.

## Roadmap

- **v0.5** — Hook `PostToolUse` paths-based + skill `lib-lookup` con WebSearch
- **v0.6** — Layers componibles (`stack:add`, `stack:doctor`)
- **v1.0** — Submit al marketplace oficial de Anthropic

## Licencia

MIT
