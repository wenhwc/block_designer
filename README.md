# Block Designer

**Block Designer** is a professional visual programming environment for control systems, simulation, and embedded firmware generation. Designed for engineers and hobbyists, it provides a high-performance workspace to design, simulate, and deploy complex logic directly to microcontrollers.

> **Note:** This repository hosts the binary releases and documentation for Block Designer. The source code is closed-source.

---

## 🚀 Key Features

- **Visual Logic Design**: Intuitive drag-and-drop interface for creating complex control loops and signal processing chains.
- **Real-time Simulation**: Run high-fidelity simulations with immediate visual feedback.
- **Signal Monitor**: Integrated oscilloscope-style view for live telemetry and signal analysis.
- **Embedded Targeting**: Program and debug firmware directly on supported STM32 microcontrollers.
- **Flash & Trace (RTT)**: High-speed bi-directional communication with hardware targets via Segger RTT for real-time debugging.
- **Hardware Validation**: Real-time checking of hardware resources, pin configurations, and peripheral conflicts.
- **Rich Library**: Comprehensive set of Math, Logic, Signal Sources, and Hardware-specific blocks.
- **PDF Export**: Generate detailed PDF reports and documentation of your designs.

## 📥 Download & Installation

### macOS
1. Go to the [Releases](https://github.com/wenhwc/block_designer/releases) page.
2. Download the latest `block_designer_mac_x64.dmg` (or Apple Silicon version if available).
3. Open the DMG file and drag **Block Designer** to your `Applications` folder.
4. Launch the app.

### Windows
1. Go to the [Releases](https://github.com/wenhwc/block_designer/releases) page.
2. Download the latest `block_designer_v0.1.1-windows-x64.zip`.
3. Extract the zip file and run the `block_designer.exe` file.

## 📖 Getting Started

1. **New Project**: Start a new design from the `File` menu.
2. **Library**: Drag blocks from the left-hand library into the workspace.
3. **Connections**: Click and drag from an output port to an input port to connect them.
4. **Properties**: Select a block to adjust its parameters (e.g., frequencies, gains, pins) in the right-hand panel.
5. **Simulation**: Click the **Simulate** button to run your logic and watch signals in the **Signal Monitor**.
6. **Hardware**: Connect your compiled STM32 board and use the **Program** feature to flash your logic directly to the hardware.

## 📄 License & Support

**Block Designer** is provided under a Private License.
The software is free for evaluation and personal use.

For feedback, bug reports, or commercial licensing inquiries, please [report issues](https://github.com/wenhwc/block_designer/issues) or contact [wen.hwc@gmail.com](mailto:wen.hwc@gmail.com).
---
© 2026 Project Day Off. All rights reserved.
