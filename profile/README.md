# Lenga Engine

<p align="center">
  <img src="https://lengaengine.com/assets/lenga-logo-default-CdVQJ-2-.png" width="140" alt="Lenga Engine Logo" />
</p>

**Lenga Engine** is a modern game engine built around a high-performance **C++ runtime** with **PHP 8.5+** as its primary scripting language.

It is designed for developers who value:
- Clear architecture
- Explicit systems
- Component-based workflows
- Fast iteration without sacrificing control

---

## What Makes Lenga Different

- **PHP as a First-Class Scripting Language**  
  Gameplay logic is written in modern PHP, embedded directly into the engine runtime.

- **Component-Driven Architecture**  
  GameObjects, Components, and Behaviour lifecycles (`awake`, `start`, `update`, etc.) are core concepts.

- **Clear Runtime / Script Separation**  
  - C++ handles rendering, input, physics, audio, and memory  
  - PHP handles gameplay logic and orchestration

- **Runtime-Agnostic Design**  
  The current rendering backend is raylib, but the engine architecture does not depend on a single graphics framework.

---

## Project Status

**Stage:** Pre-alpha  

Lenga Engine is under active development. Core systems are still stabilizing and public APIs may change.

Current focus areas include:
- Runtime correctness
- Deterministic behaviour execution
- Scene loading and lifecycle management

---

## Repository Overview

This organization hosts multiple repositories, including:

- **`lenga-runtime`**  
  The C++ engine runtime (rendering, input, physics, audio)

- **`lenga-php`**  
  The PHP scripting API exposed to game developers

- **`lenga-editor`**  
  A future editor application for authoring scenes and assets

- **`.github`**  
  Organization-wide documentation, roadmap, and contribution policies

---

## Roadmap

Development follows a milestone-driven approach:

1. Core runtime & scripting
2. Scene system
3. Physics (2D)
4. Camera & rendering layers
5. Prefabs & object lifecycle
6. Input abstraction
7. Asset pipeline
8. Editor prototype
9. Build & distribution
10. Advanced systems

Detailed milestones are maintained in the roadmap documentation.

---

## Contributing

Contributions are currently **restricted** while the engine’s core architecture is finalized.

Bug reports, build issues, and architectural feedback are welcome.  
General pull requests will open in later milestones.

---

## Learn More

- Website: https://lengaengine.com
- Documentation and roadmap are maintained within this organization

---

**Lenga Engine**  
*A deliberate engine for serious creators.*
