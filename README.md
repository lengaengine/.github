# Lenga Engine

<p align="center">
  <img src="https://lengaengine.com/assets/lenga-logo-default-CdVQJ-2-.png" width="160" alt="Lenga Engine Logo" />
</p>

<p align="center">
  <img alt="Status" src="https://img.shields.io/badge/status-pre--alpha-yellow" />
  <img alt="Language" src="https://img.shields.io/badge/runtime-C%2B%2B-blue" />
  <img alt="Scripting" src="https://img.shields.io/badge/scripting-PHP%208.5%2B-8892BF" />
  <img alt="Platforms" src="https://img.shields.io/badge/platforms-Windows%20|%20Linux%20|%20macOS-lightgrey" />
  <img alt="License" src="https://img.shields.io/badge/license-TBD-lightgrey" />
</p>

**Lenga Engine** is a Unity-inspired game engine that combines a high-performance **C++ runtime** with **PHP 8.5+** as the primary scripting language.

The engine is designed for developers who value:
- Explicit architecture
- Fast iteration
- Familiar Unity-style workflows
- Clear separation between runtime systems and gameplay logic

> **Status:** Pre-alpha  
> **Rendering Backend:** raylib (current)  
> **Architecture:** Runtime-agnostic, component-driven

---

## Vision

Lenga Engine explores a different trade-off in engine design:

- C++ for deterministic performance and memory control
- PHP for expressive, hot-reloadable gameplay scripting
- A Unity-like mental model without Unity’s constraints

The long-term goal is a **fully authorable editor + runtime pipeline** capable of producing complete 2D and 3D games.

---

## Core Design Principles

- **Unity-Like Architecture**
  - GameObjects
  - Components
  - Behaviour lifecycle (`awake`, `start`, `update`, etc.)
- **Clear Runtime / Script Boundary**
  - C++ owns rendering, input, physics, audio
  - PHP owns gameplay logic and orchestration
- **Runtime Independence**
  - raylib is a backend, not a hard dependency
- **Predictable Systems**
  - Explicit scene loading
  - Deterministic lifecycle execution
  - Minimal hidden magic

---

## High-Level Architecture
+-----------------------+
| Lenga Editor | (Future)
+-----------------------+
|
v
+-----------------------+
| Lenga Runtime | C++
|-----------------------|
| Scene | Input | Draw |
| Phys | Audio | Time |
+-----------------------+
|
v
+-----------------------+
| PHP Runtime | PHP 8.5+ (Embed SAPI)
|-----------------------|
| Behaviours |
| Game Logic |
| Events & State |
+-----------------------+

---

## Repository Purpose

This repository contains **organization-wide documentation** for Lenga Engine:

- Public overview
- Contribution rules
- Development roadmap

Engine source code lives in dedicated repositories, including:

- `lenga-runtime` — C++ runtime
- `lenga-php` — PHP scripting API
- `lenga-editor` — Editor application
- `lenga-cli` — Tooling & build pipeline

---

## Roadmap

See **[ROADMAP.md](ROADMAP.md)** for the full milestone plan (2025–2026).

---

## Contributing

Lenga Engine is currently **closed to general contributions** while core systems are stabilizing.

See **[CONTRIBUTING.md](CONTRIBUTING.md)** for details.

---

## License

License information will be published once the engine reaches public alpha.

---

**Lenga Engine**  
*A deliberate engine for serious creators.*

