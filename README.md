AeroTactical Neural OS: Tactical Edge-SLM Autonomous Runtime & Model Harness
A production-ready, air-gapped Open-Weight Small Language Model (SLM) & Edge Computer Vision Harness engineered for high-density, mission-critical autonomous edge computing (NVIDIA Jetson Orin AGX, NPU/AVX-512 heterogeneous architectures, RK3588, and air-gapped field workstations)
1. Open-Weight Model Harness & GBNF Grammar Compiler (Structured JSON Tools)
Formal GBNF Grammar Compilation: Compiles JSON Schema Draft-07 specifications directly into formal llama.cpp GGML BNF grammar rules (root ::= ...), enforcing 100% mathematical zero-drift determinism by constraining the token generation distribution.
AST Branch & Grammar Size Profiler: Dynamically measures branch complexity, recursion depth, and file size in KB. Includes instant schema formatting and copy capabilities.
Adversarial Injection & 100x Fuzzing Engine: Synthetic fuzzing benchmark that subjects the GBNF-constrained harness to prompt injection attacks (e.g. attempting to force non-JSON output or invalid pin mappings), verifying 100% schema conformance.
Hardware Execution & IPC Dispatch: Live UNIX socket broker stream (/tmp/tactical_slm_broker.sock), memory-mapped I/O (/dev/gpiomem), register state verifications, and an interactive CLI test runner.
2. Local SLM Agent Harness & Airgap RAG Engine (Local Checkpoints)
Open-Weight Checkpoint Orchestration: Dynamic model switcher supporting Llama-3.2-3B-Instruct (Q4_K_M), Phi-3.5-mini-3.8B (Q5_K_S), and Qwen2.5-Coder-3B (Q4_0), updating VRAM allocation, TTFT, and generation velocity in real time.
Interactive Chat Transcript & Streaming Tokens: Interactive prompt terminal with simulated token velocity, TTFT timers, and expandable Chain-of-Thought (CoT) internal reasoning steps.
Interactive Tool Dispatch: Formats recommended remediation scripts (e.g. /opt/uav/recal_pwm_neutral.sh -f 140hz) with an executable "DISPATCH FIX" trigger.
Offline Vector RAG Memory (SQLite-vec style): Real-time cosine similarity search across pre-ingested aerospace engineering manuals (MIL-STD-810H.pdf, Propulsion_Diag_RevC.md, Radio_Crypto_CheatSheet.txt).
Live Document Ingestor: "INGEST LOCAL ASSET" modal allows operators to paste or load custom operational manuals, automatically segmenting text into 384-dimensional vector chunks.
Decoding & Guardrail Controls: Interactive sliders for Temperature (0.00 to 1.00) and Top_P, plus toggles for Tactical Safety Filter, Offline RoPE Context Compression, and Memory Spillover Traps.
3. Multimodal Edge Vision & Tactical HUD (Mission Feeds)
Multi-Spectrum Sensor Switching: Instant toggling between FLIR-W (White Hot Infrared), FLIR-B (Black Hot Infrared), and EO-RGB (Full Spectrum Optical) with custom contrast and radiometric filters.
Optical Zoom Levels: Instant magnification between 1x, 4x FLIR, and 10x ULTRA.
Interactive Bounding Reticles: Clickable detection boxes for BAY_POD::01, HYDRAULIC ACTUATOR FAULT (with critical alert pulse and thermal hotspot tags), and EMITTER_NODE. Selecting any box feeds telemetry directly into the SLM reasoner.
6-Frame Anomaly Timeline Filmstrip: Interactive frame selector (Thermal Spike, Stress Fracture, Component Match, Heat Exchanger, RF Transmitter, Sys Baseline). Clicking any frame swaps the optical feed and triggers real-time SLM re-assessment.
Direct Multimodal Query Terminal: Operators can query the local SLM about specific MTBF degradation curves, vibration harmonic dampening, or seal failures.
Airgap Mission Report Exporter: Generates and exports encrypted JSON mission reports with SHA-256 seal signatures.
4. Hardware Telemetry & Heterogeneous Offload Engine (System Log Stream)
Jetson Orin AGX Hardware Matrix: Live telemetry for Compute Load (with 10-bar segmented meter), Unified LPDDR5 VRAM stacked allocation (Weights, KV cache, Vision, System, Free), SoC Thermal & TDP power envelopes, and TTFT latency benchmarks.
Interactive 28-Layer Offload Visualizer: Clickable layer blocks (L0 through L27) allowing operators to dynamically reassign layers between NPU Tensor Cores and CPU AVX-512 fallback, updating PCIe Gen4 DMA bandwidth readouts.
Quantization Tradeoff Profiler: Comparative perplexity, memory footprint, and latency matrices across Q4_K_M, Q5_K_M, and Q8_0 with an AWQ tensor recalculator.
Continuous Run Thermals & RF Kill Switches: Real-time SVG thermal drift graph tracking SoC die temperature against the 75°C throttle trippoint, paired with physical RF cut switches for Wi-Fi 6E, Bluetooth BLE, and Starlink Tactical.
Emergency Airgap Lockdown Switch: Master kill switch in the top header that toggles airgap isolation mode with visual alert notifications.
