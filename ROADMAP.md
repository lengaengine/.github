# Lenga Engine — Development Roadmap (2025–2026)

This roadmap outlines the planned evolution of Lenga Engine from core runtime to a full editor-driven production pipeline.

The progression intentionally mirrors how mature engines historically evolved:
**Runtime → Scene → Physics → Rendering → Prefabs → Input → Assets → Editor → Builds**

---

## Milestone 1 — Core Engine Runtime
**Status:** In progress  
**Goal:** A stable movement demo driven by PHP scripts.

### Deliverables
- Embedded PHP runtime (php-embed)
- Behaviour lifecycle:
  - `awake`
  - `onEnable`
  - `start`
  - `update`
  - `lateUpdate`
  - `fixedUpdate`
  - `onDisable`
  - `onDestroy`
- Transform bindings
- Vector math utilities
- Input axis handling
- C++ ↔ PHP debug logging

### Acceptance Criteria
- A sprite renders on screen
- PHP script moves the sprite using input
- Engine shuts down cleanly

---

## Milestone 2 — Scene System & Asset Loading

### Deliverables
- JSON-defined scenes
- GameObject naming
- Transform hierarchies
- Component definitions
- Behaviour class mapping (JSON → C++ → PHP)
- Basic asset lookup system

### Acceptance Criteria
- JSON scenes behave identically to hardcoded scenes
- Removing a behaviour removes runtime execution
- Transform changes reflect immediately

---

## Milestone 3 — Basic Physics Engine (2D)

### Deliverables
- `Rigidbody2D`
- `Collider2D` (AABB)
- Collision events:
  - enter
  - stay
  - exit
- PHP bindings:
  - `onTriggerEnter2D`
  - `onTriggerStay2D`
  - `onTriggerExit2D`
- Fixed timestep loop
- Optional debug rendering

### Acceptance Criteria
- Objects collide correctly
- PHP receives collision callbacks
- Players cannot pass through walls
- Trigger pickups work

---

## Milestone 4 — Camera System & Rendering Layers

### Deliverables
- Camera component
- World-space projection
- Sorting layers
- Order-in-layer
- Optional parallax layers

---

## Milestone 5 — Prefabs & GameObject Lifecycle

### Deliverables
- Prefab asset format
- Runtime instantiation API
- Internal GUID system
- “Don’t Destroy On Load”

---

## Milestone 6 — Input System v2

### Deliverables
- Axis-based input
- Button mappings
- Configurable input file
- Device abstraction

---

## Milestone 7 — Asset Pipeline

### Deliverables
- Texture cache
- Audio system
- Asset metadata
- Hot reload (editor only)

---

## Milestone 8 — Lenga Editor (Prototype)

### Deliverables
- Scene hierarchy
- Inspector
- Scene view
- Play / Stop workflow
- Live reload

---

## Milestone 9 — Build & Distribution Pipeline

### Deliverables
- `lenga build` CLI
- Bundled runtime + scripts + assets
- Platform-specific outputs
- Runtime / script version compatibility checks

---

## Milestone 10 — Advanced Systems (Future)

### Possible Targets
- Animation system
- UI system
- Navigation & AI
- Networking
- Particle systems
- Full 3D pipeline

---

## Summary

Lenga Engine prioritizes **correctness, clarity, and long-term maintainability** over early feature breadth.

This roadmap will evolve as milestones are completed.
