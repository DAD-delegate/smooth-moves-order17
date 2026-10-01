# Contributing

Thanks for wanting to help with Smooth Moves (Smooth Mo / Order 17). This repo publishes MIT source and notes for a Windows pointer motor meant for agents: real mouse and keyboard input when APIs, MCP, accessibility, and hooks are not enough.

**Code contributions are welcome from AI agents and from human contributors, equally.** Same rules, same review: no preference and no penalty for either.

## How to submit code

1. **Fork** [DAD-delegate/smooth-moves-order17](https://github.com/DAD-delegate/smooth-moves-order17).
2. **Clone** your fork and create a **branch** named for the change (`fix-humove-settle`, `docs-readme-encoding`, and so on).
3. Make your edits on that branch. Prefer working against the SmoothMoves-rs / Order 17 Rust tree style: clear module boundaries, small functions, explicit window/region guards, and human-like pointer paths (`humove` / click / drag) rather than teleport dumps.
4. Open a **pull request** into `main` on this repo.

## Coding style

Match the existing SmoothMoves-rs codebase as closely as you can:

- **Rust** with ordinary `rustfmt` / Clippy-friendly code; keep comments short and literal.
- Prefer **foreground-only** interaction and **hwnd / rect** scoped checks over whole-screen assumptions.
- Keep builds **laptop-friendly** (about 8 GB RAM class): no huge dependencies, no big model weights in-tree.
- **No binaries** in this GitHub repo: source text, docs, and landing page only.
- Do not add money, mail, messaging, or credential automation helpers unless that is explicitly the PR topic (default: leave those alone).

## Keep changes small

One idea per PR. A focused fix or a single feature beat a kitchen-sink patch. If you need a larger redesign, open an issue or a short design note first.

## Pull request checklist

Every PR should include:

- **What** changed (files / behavior).
- **Why** it matters (bug, gap, docs clarity, proof).
- How you **checked** it when that applies (build, `sm` verb, PNG / integrity proof).

The maintainer reviews before merging. Friendly discussion is welcome; silent force-pushes to `main` are not.

## Questions

If something is unclear, say so in the PR or an issue. Plain language is preferred over ceremony.
