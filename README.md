<div align="center">

# Ferrum-Sidereum

**AI for ur I**

Building tools that connect AI agents to real systems — with explicit permissions, protected secrets, and inspectable traces.

</div>

<table>
<tr>
<td width="62%" valign="top">

## System status

```text
ROLE      AI / backend developer
FOCUS     LLM infrastructure · agent security
BUILDING  Sentinel · mist
APPROACH  Build → inspect → test → ship
```

I build the infrastructure around AI agents:
how they access tools, use credentials, and communicate with model providers.

My focus is on **human-controlled workflows** —
with explicit approval gates and actions you can inspect.

### Currently building

- **Sentinel** — secret management and access controls for AI agents.
- **mist** — an LLM proxy with API key rotation and a web dashboard.
- **Agent workflows** — experiments with tool use, approvals, and execution traces.

</td>
<td width="38%" align="center" valign="top">

<img src="assets/entrity%20copy.jpg" alt="entrity — artwork by Radomir Karimov" width="100%" />

<sub><i>“entrity” by Radomir Karimov</i></sub>

</td>
</tr>
</table>

## Selected work

### [Sentinel](https://github.com/Ferrum-Sidereum/sentinel)
**Agents get references, not raw secrets.**

An open-source security tool that resolves secret references at the request boundary, rather than exposing credentials directly to the agent.

- Encrypted vault with OS keychain integration or Argon2id-based key derivation.
- Egress proxy for secret injection and response redaction.
- MCP gateway with payload scrubbing and approval controls.
- Tamper-evident audit log, live policy reload, CLI, and Windows desktop app.
- Cross-platform CI, automated releases, and Homebrew/Scoop packages.

`Go` · `SQLite` · `MCP` · `Wails` · `React` · `TypeScript`

### mist
**One endpoint for multiple LLM clients.**

A personal LLM proxy project with an OpenAI-compatible API and streaming responses.

- API key rotation with quota-aware cooldowns and invalid-key detection.
- CLI tools for importing and checking keys.
- Vue dashboard for pool status and management.
- Persistent pool state across restarts.

`Rust` · `Vue 3` · `REST API` · `SQLite / JSON`

## Toolbox

| Area | Tools |
| --- | --- |
| Backend | Go · Rust · Python |
| Interfaces | TypeScript · React · Vue 3 · Wails |
| LLM integrations | OpenAI-compatible APIs · MCP · streaming |
| Browser automation | Playwright · Chrome DevTools Protocol |
| Storage & delivery | SQLite · Git · CI · GoReleaser |
| Exploring | Hermes · Pi · agent workflows |

## Engineering principles

- **Keep humans in control.** Make sensitive actions explicit and reviewable.
- **Keep secrets out of model context.** Resolve credentials where they are needed.
- **Make behavior inspectable.** Prefer visible traces over hidden automation.
- **Test the boundaries.** Failure paths and access controls are part of the feature.
- **Prefer evidence over hype.** Build things others can run and inspect.

---

<div align="center">

> Don't forget who you are.

[**Explore my repositories →**](https://github.com/Ferrum-Sidereum?tab=repositories)

</div>
