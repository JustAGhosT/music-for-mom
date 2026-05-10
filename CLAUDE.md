# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

**Music For Mom** — Simple desktop app to download YouTube music to a USB drive. Built with Tauri for a lightweight, native experience.

## Tech Stack

- **Desktop**: Tauri (Rust backend)
- **Frontend**: React/TypeScript (or vanilla web)
- **Audio**: YouTube download integration

## Key Commands

```bash
npm install               # Install JS dependencies
npm run dev               # Start Tauri dev
npm run build             # Production build
cargo tauri build         # Build native installer
```

## AgentKit Forge

This project has not yet been onboarded to [AgentKit Forge](https://github.com/phoenixvc/agentkit-forge). To request onboarding, [create a ticket](https://github.com/phoenixvc/agentkit-forge/issues/new?title=Onboard+musicformom&labels=onboarding).

## Baton Integration

Baton is the shared task graph for cross-repo work. When the `baton` MCP server is available, agents should check for existing work with `task_check` at the start of meaningful tasks, create or claim visible work with `task_notify`/`log_agent_message`, update the task when significant new information becomes available, and log completion or blockers before handing off.
