# SSXL Engine Releases

Welcome to the official public distribution repository for **SSXL**, the high-performance, GPU-accelerated engine synthesized via **SSXL-GEN**. 

This repository hosts pre-compiled binaries, toolchains, runtime templates, and official demo releases across desktop platforms. The core engine synthesis toolchain remains proprietary, but you can explore, test, and build games using the distributed binaries here.

---

## ⚡ What is SSXL?

SSXL is a data-oriented, GPU-first game simulation platform designed around automated architectural generation. Rather than manually wiring boilerplate, SSXL uses a generative compiler (`ssxl-gen`) to emit full-stack editor frameworks and low-latency runtimes.

### Key Capabilities Included in Editor Releases:
- **Integrated Editor UI:** Complete SceneTree hierarchy, interactive Viewport canvas, and dynamic real-time Component Inspector.
- **Substrate Execution Model:** GPU-driven procedural computation and low-latency simulation cycles.
- **Turnkey Reference Project:** Bundled with the official **SSXL Pacman Showcase** featuring 10 custom play modes demonstrating engine systems, input pipelines, and dynamic render passes.

---

## 🏷️ Release Tiers & Roadmap

SSXL is distributed across four distinct tiers tailored for evaluation, open creation, professional studios, and early architecture backers:

| Tier | Status | Focus & Description |
| :--- | :---: | :--- |
| **SSXL-BETA** | **Available Now** | Public preview builds. Includes full access to the editor, viewport, inspector, and the 10-mode showcase project for stress-testing and architecture feedback. |
| **SSXL-COMMUNITY** | *Coming Soon* | Free non-commercial and indie creation tier with standardized tooling, community plugins, and runtime export capability. |
| **SSXL-PRO** | *Coming Soon* | Production-grade engine distributions with extended profiling toolchains, priority target export modules, and advanced compute pipelines. |
| **SSXL-FOUNDER** | *Invite / Direct* | Early-adopter tier featuring direct engine architectural previews, custom template modules, and bespoke synthesis hooks. |

---

## 🚀 Getting Started (SSXL-BETA)

### 1. Download & Verify
Grab the latest pre-compiled archive for your operating system from the [Releases Tab](../../releases):
* `ssxl-beta-v<version>-windows-x86_64.zip`
* `ssxl-beta-v<version>-linux-x86_64.tar.gz`
* `ssxl-beta-v<version>-macos-universal.zip`

### 2. System Requirements
* **GPU:** Vulkan 1.3 / DirectX 12 / Metal-compatible dedicated GPU (Compute Shader support required).
* **OS:** Windows 10/11 (64-bit), Linux (glibc 2.31+, modern desktop environment), or macOS 12+ (Apple Silicon or modern Intel).
* **RAM:** 8 GB minimum (16 GB recommended for high-density compute scenes).

### 3. Launching the Editor
Extract the archive and execute the main binary:

```bash
# Linux / macOS
./ssxl-editor

# Windows
ssxl-editor.exe
```

By default, the editor will boot directly into the workspace selector or open the bundled Pacman showcase project.

---

## 🎮 Included Showcase: Pacman (10 Modes)

Every Beta release includes a fully operational reference project showcasing the limits of the SSXL architecture:
1. **Classic Arcade:** Authentic frame timing, tilemaps, and state machines.
2. **GPU Swarm:** Hundreds of dynamic entities pathfinding concurrently via compute kernels.
3. **Hyper-Speed:** High-frequency physics and sub-frame tick updates.
4. **Procedural Maze:** Dynamic runtime layout synthesis via cellular automata.
5. **Inverse Hunter:** Dynamic AI inversion and multi-target chase algorithms.
6. *...plus 5 additional experimental game variations demonstrating live inspector mutations.*

Select different modes directly from the **SceneTree** or swap play configs inside the **Inspector** at runtime.

---

## 🐛 Feedback & Issue Reporting

Because SSXL-BETA is an active testbed release, your feedback is crucial:
* **Bug Reports:** Open an issue in this repository using the `[Beta Bug]` prefix.
* **Performance Logs:** Attach system specs and the auto-generated `ssxl_session.log` from your root folder.

---

## ⚖️ License

The binaries and demo assets distributed in this repository are licensed under the **SSXL Binary Evaluation & Distribution License**. See [`LICENSE.md`](LICENSE.md) for full terms and conditions.
