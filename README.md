# Robinson George Arysseril

An engineer working at the convergence of Low-Level Systems Architecture, Emulation, and Machine Learning Infrastructure.

- **GitHub:** [github.com/death7654](https://github.com/death7654)
- **LinkedIn:** [linkedin.com/in/robinsonarysseril](https://linkedin.com/in/robinsonarysseril)
- **Portfolio:** [death7654.github.io](https://death7654.github.io) — Documenting my journey into programming.

---

## Technical Focus

### Systems, Kernel & Hardware Emulation
- **Languages:** Rust, C/C++, Zig, Xtensa Assembly
- **Low-Level Concepts:** Bare-metal development, Custom Bootloaders, Memory-Mapped I/O, DMA, Interrupt Handling, FAT32/MBR Parsing
- **Databases & Tooling:** SQL (MySQL), JSON, Git, Make

### Machine Learning & AI Research
- **Frameworks:** PyTorch, TensorFlow, Transformers, Sentence-Transformers, Scikit-Learn
- **Core Libraries & Architecture:** Pandas, NumPy, Matplotlib, SciPy, Time-Series (LSTM)
- **Custom Implementations:** Writing fundamental ML mathematical algorithms completely from scratch.

### Full-Stack Desktop & Web Stacks
- **Frameworks & Languages:** Tauri (Rust backend), Angular, C#, TypeScript, JavaScript, Bootstrap, HTML/CSS

---

## Experience & Research

### Research Intern
**Amrita School of Artificial Intelligence, Amrita Vishwa Vidyapeetham** | *May 2026 - Jun. 2026*
- Investigated and analyzed linguistic features relevant to gender bias in AI systems using modern NLP techniques under Dr. Premjith B.
- Benchmarked classical machine learning models and deep learning architectures for text bias classification tasks.
- Applied prompt engineering techniques to assess and mitigate bias in Large Language Models and generative AI systems.

### Open Source Contributor
**Chrultrabook Project** | *May 2023 - Present*
- Maintained Chrultrabook Tools, a cross-platform system utility with 45,000+ downloads serving users running alternate operating systems on Chromebook hardware.
- Managed core hardware compatibility database entries, expanding accurate chipset and driver support across device models.

---

## Repository Ecosystem

### Systems & Operating Systems

#### null32
- **Stack:** C, Xtensa Assembly
- A custom operating system for the ESP32 built completely from scratch, focusing on low-level resource management and register-level hardware control.

#### Bare Metal ESP32 Kernel
- **Stack:** C, Xtensa Assembly, Python
- Designed a two-stage boot process where a flash-resident bootloader reads a kernel binary from an SD card into DRAM, then copies it to IRAM via a custom Xtensa assembly trampoline before execution.
- Built a register-level SPI driver from ESP32 TRM documentation covering GPIO matrix routing, IO MUX configuration, and full SD card SPI mode initialization.
- Implemented an interactive kernel shell and a script interpreter to execute timed GPIO sequences at runtime without reflashing.

#### FAT32-Reader-Windows
- **Stack:** Low-Level C
- An implementation of a raw disk parser written in low-level C to inspect and traverse FAT32 file systems directly.

### Hardware Emulators (Correctness & Cycle-Accuracy)

- **NES-Emulator-Rust:** A Nintendo Entertainment System (NES) emulator engineered in Rust.
- **Game Boy (DMG) Emulator:** Cycle-accurate hardware simulation in Rust implementing the Sharp LR35902 CPU, scanline-based PPU rendering pipeline, tile caching, sprite compositing, and strict OAM DMA timing restrictions.
- **Intel 8080 Emulator:** Written in C++ featuring complete instruction set coverage, precise flag operations, and interrupt-driven timing synchronized to duplicate authentic *Space Invaders* arcade hardware.
- **XO-CHIP & CHIP-8 Interpreters:** Multi-language implementations across Zig, Rust, and C++ with full opcode verification, dual display planes, and 64KB memory addressing extensions.

### Audio & Hardware Utilities

#### RumbleGuard
- **Stack:** Rust
- A real-time application designed to ingest audio feed via a smartphone microphone to actively cancel out ambient car cabin frequencies.

#### Chrultrabook Tools & Configuration Ecosystem
- **Stack:** Rust, Tauri, Angular, TypeScript, C++, SQL, JSON
- **Chrultrabook-Tools:** Configuration utility handling live hardware sensor telemetry, fan curve calculations, and IPC communication.
- **Chromebook-Driver-Installer:** Automated driver utility managing chipset matches across 200+ models with dynamic metadata updates without app rebuilds.
- **croskb4-config-generator:** Dedicated repository to program and test keyboard remapping configurations for Chromebooks utilizing Coolstar's drivers.
- **AntiPop-For-Chromebooks (C++):** Low-level audio utility designed to eliminate popping artifacts when audio streams initialize on modified Chromebook hardware.
- **chromium-tools:** A collection of specialized utility tools for Chromebooks running Linux environments.

### Machine Learning & AI Research

#### Gender Bias Detection in News Headlines
- **Stack:** Python, PyTorch, Sentence-Transformers, Transformers, Scikit-Learn
- Custom NLP pipeline implementing a dual-objective training model (cross-entropy + contrastive loss) combined with a neutrosophic membership scoring function to track decision uncertainty.
- Built a two-step self-correcting LLM prompting pipeline (Few-Shot Reasoning + Verification Pass) to evaluate bias detection using SmolLM2-1.7B-Instruct.

#### ML-Algorithms
- **Stack:** C++
- From-scratch implementations of fundamental Machine Learning algorithms built entirely without external mathematical or training libraries.

#### Stock Market Predictor Engine
- **Stack:** Python, TensorFlow, TypeScript, Scikit-Learn, yfinance
- An end-to-end time-series forecasting engine utilizing stacked LSTM neural networks with checkpoint persistence for incremental training, split into a Python training backend (`Stock-Market-Predictor-ML-Model`) and a web-based dashboard configuration (`Stock-Market-Predictor-FrontEnd`).

### Other Engineering Foundations

- **OpenVoice-OpenBox (TypeScript):** A collaborative platform utility built during FOSSHACK 1.0.
- **Cherry-Labs (C#):** A custom desktop frontend client built for interacting with Gemini models.
- **BinanceTradingBot (Python):** An automated algorithmic script interface interacting with the Binance API.
- **Movie-Ticket-Booking-System (C):** A data structures and algorithms paradigm project written cleanly in C.
- **Todo_list_rust (Rust):** Minimal, high-performance command-line task management utility.

---

## Core Focus Goals

- Authoring ultra-reliable, high-performance low-level systems software and drivers using Rust and modern systems tools.
- Demystifying AI execution constraints by engineering custom compute engines, hardware acceleration layers, and performance profiles directly on hardware.
