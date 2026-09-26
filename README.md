# Hi, I'm XiaoPu (小溥)

I build **AI-native products and the systems behind them**.

My favorite projects start as a messy problem and end up spanning product design, system architecture, backend, frontend, infrastructure, integrations, and AI.

I'm especially interested in what happens when AI stops being a feature and becomes part of the software architecture: agents using tools, operating on real application state, coordinating work, and knowing when control should return to a human.

---

## What I build

- **AI-native systems** — agents, tool use, MCP, multi-model routing, local models, browser automation, and human-in-the-loop execution
- **Product systems** — turning product ideas into coherent workflows, interfaces, data models, and abstractions
- **Backend & infrastructure** — APIs, databases, networking, payments, deployments, reliability, and observability
- **Developer tooling** — infrastructure for making humans and AI faster at building software
- **End-to-end products** — I like owning the path from architecture diagram to something people can actually use

I care a lot about questions like:

**Where should intelligence live? What should be deterministic? What can an agent change? What happens when it fails?**

---

## Things I've built

### [openchatx-mcp](https://github.com/XiaoPuOuO/openchatx-mcp)

A **local agent runtime and MCP gateway for ChatGPT** that gives a normal conversation controlled access to local execution, files, tools, external MCP servers, and provider-backed subagents.

It keeps the main tool surface small through lazy capability discovery: ChatGPT can discover and invoke Blender, Unreal, browser automation, custom TypeScript toolboxes, local models, and other connected capabilities only when a task actually needs them. The result is a practical bridge between a cloud planner and a user-controlled local runtime.

### [chatgpt-image-bridge](https://github.com/XiaoPuOuO/chatgpt-image-bridge)

A **zero-dependency CLI and MCP server** that turns the ChatGPT Desktop App into an image-generation tool any AI agent can call.

No API reverse-engineering, no extra subscription: it relaunches the app with loopback CDP, injects the prompt into the chat composer, waits for generation to finish, and recovers the PNG straight from the DOM. Cross-process file locking lets multiple agents queue against one app instance safely. Same CDP trick as Codex Dream Skin — but pointed at capability instead of cosmetics.

### [Cursor Dream Skin](https://github.com/XiaoPuOuO/cursor-dream-skin)

A **notarized macOS menu bar app** that skins the **Cursor Agents** window through local loopback CDP injection — wallpapers, glass UI, theme switching, and Codex theme import — without modifying the official Cursor app.

Inspired by [Codex Dream Skin](https://github.com/Fei-Away/Codex-Dream-Skin), but scoped to Cursor's agent surface: inject only where humans actually pair with AI, keep the IDE chrome native, and make re-application automatic across reloads.

### [OpenCode Dream Skin](https://github.com/XiaoPuOuO/opencode-dream-skin)

A **macOS menu bar app** that skins **OpenCode Desktop** through local loopback CDP injection — wallpapers, glass themes, one-click restore — without touching the official install.

The third skin in the same family (Codex → Cursor → OpenCode), keeping the shared discipline: non-destructive, reversible, auto re-apply on login, and theme-pack compatible with Codex Dream Skin.

### [UniqueCharEditor](https://github.com/XiaoPuOuO/UniqueCharEditor)

An open-source Windows tool for **game font and glyph workflows**, including unique-character extraction and missing-glyph detection.

Built because manually debugging large character sets is a terrible use of human time.

---

## Currently exploring

**AI agents · AI-native product architecture · developer infrastructure · human × AI workflows · systems that can act, not just answer**

---

If you're building something ambitious around AI or software infrastructure, I'd be happy to talk.

*Still learning. Still building.*
