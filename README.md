# Block Designer

**Block Designer** is a self-hosted visual environment for embedded control — a lightweight, self-contained take on model-based design. Design your control loop visually, simulate it with real solver fidelity, then flash it straight to an STM32. Built for engineers and hobbyists alike.

> **Note:** This repository is for **bug reports and discussion**. Downloads and documentation live on the [website](https://projectdayoff.com).

🌐 **Website & tutorial:** [projectdayoff.com](https://projectdayoff.com) — a 7-lesson walkthrough of the basics.

---

## 🚀 Key Features

### 🎨 Visual Logic Design
- Click-to-place canvas with an infinite, zoomable grid.
- Searchable palette of 100+ pre-built blocks across 14 categories (Source, Math, Logic, Dynamic, Control, Hardware, Sink, and more).
- Automatic orthogonal wire routing (A* pathfinding) that re-routes as you move blocks.
- Live parameter editing with inline validation.
- Subsystems for collapsing parts of a large design into reusable modules.

### ⚡ Real-time Simulation
- High-fidelity DAE solver for continuous-time control.
- Configurable step sizes and integrator methods.
- Multi-rate support — fast loops and slow supervisors run at the right relative speeds.

### 📊 Signal Analysis
- Integrated oscilloscope-style **Signal Monitor**: pan, zoom, cursors, and multi-signal overlay.
- **Automatic eigenvalue (pole) analysis** — the system is linearized after every run and its poles plotted on the complex plane; a time slider re-linearizes at any instant.
- **Root locus** from a **Gain Probe** block — sweep a gain across a range and watch the poles trace their path. Multiple probes can coexist on one canvas.
- CSV export for spreadsheets, Python, and other analysis tools.

### 🔌 Embedded Targeting
- STM32 targeting across the **F4 / L4 / H7** families.
- **Safe, pure-Rust firmware generation** — no C, no hand-written code. An optional **auditable** codegen style emits Rust that reads like hand-written code, so you can review exactly what runs on the chip.
- One-click flashing directly over **OpenOCD / ST-Link** — zero-config.
- Real-time **hardware validation**: pin configurations and peripheral conflicts are checked as you design.
- Rich hardware block library: PWM, ADC, GPIO, and more.

### 🛰️ Flash & Trace (RTT)
- High-speed bi-directional communication with hardware targets via Segger RTT for real-time debugging and live tuning.

### 🛠️ Professional Workflow
- Built-in **Undo/Redo**, workspace management, and high-quality **PDF Export** for design documentation.
- **Safety first**: active monitoring of unsaved changes and confirmation dialogs to protect your work.

## 📥 Download & Installation

### macOS
1. Download the latest **Apple Silicon (M-series)** [`.dmg`](https://downloads.projectdayoff.com/latest/block_designer_macos_arm64.dmg). *(Intel Macs are not supported.)*
2. Open the DMG file and drag **Block Designer** to your `Applications` folder.
3. Launch the app.

### Windows
1. Download the latest [Windows x64 zip](https://downloads.projectdayoff.com/latest/block_designer_windows_x64.zip).
2. Extract the zip file and run `block_designer.exe`.

## 📖 Getting Started

New to Block Designer? The [tutorial](https://projectdayoff.com/tutorial/) walks through the basics in 7 short lessons. In brief:

1. **New Project**: Start a new design from the `File` menu.
2. **Library**: Click a block in the left-hand library — it follows your cursor; click again on the canvas to place it.
3. **Connections**: Click an output port, then click an input port to connect them.
4. **Properties**: Select a block to adjust its parameters in the right-hand panel.
5. **Simulation**: Click the **Simulate** button to run your logic and watch signals in the **Signal Monitor** — and read the system's eigenvalues / root locus in the **Analysis Console**.
6. **Hardware**: Connect your STM32 board and use **Program STM32** to flash your logic directly to the hardware.

## 📄 License & Support

**Block Designer** is free for evaluation and personal use.

- **Bug reports:** [open an issue](https://github.com/wenhwc/block_designer/issues).
- **Feedback, questions, or commercial licensing inquiries:** start a [discussion](https://github.com/wenhwc/block_designer/discussions).

---
© 2026 Project Day Off. All rights reserved.
