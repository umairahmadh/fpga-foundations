# 01 · Foundations

**Part of [FPGA Journey](https://github.com/umairahmadh/fpga-journey)**

> Building the mental model that makes everything else click: number systems, Boolean logic, sequential circuits, and the nand2tetris computer build.

No HDL here yet. No tools to install. This is pencil-and-paper + the nand2tetris simulator — the fastest way to stop thinking like a programmer and start thinking like a hardware designer.

---

## 🎯 Learning Objectives

- Fluency in binary, hex, and two's complement (especially **fixed-point** — you'll use this forever in DSP)
- Boolean algebra: simplification, De Morgan's laws, Karnaugh maps
- How combinational logic is built from gates → half adder → full adder → ALU
- Sequential logic: latches, flip-flops, registers, synchronous design
- Finite State Machines (Mealy vs. Moore) — think in states, not in loops
- Why clocks matter and what "timing" means at an intuitive level

---

## 📁 Structure

```
fpga-01-foundations/
├── 01_number_systems/
│   ├── notes.md            # Binary, hex, two's complement, fixed-point
│   └── exercises.md        # Worked problems with answers
├── 02_boolean_algebra/
│   ├── notes.md
│   └── kmap_examples.md    # Karnaugh map simplification examples
├── 03_combinational_logic/
│   ├── notes.md            # Gates → mux → adder → ALU concepts
│   └── diagrams/           # Hand-drawn or draw.io block diagrams
├── 04_sequential_logic/
│   ├── notes.md            # Flip-flops, registers, clocks, reset
│   └── timing_diagrams/    # Waveform timing drawings
├── 05_finite_state_machines/
│   ├── notes.md
│   ├── traffic_light_fsm.md    # Worked FSM example with state diagram
│   └── vending_machine_fsm.md
└── 06_nand2tetris/
    ├── notes.md            # Chapter-by-chapter notes
    ├── projects/
    │   ├── 01_boolean_logic/   # HDL solutions for nand2tetris project 1
    │   ├── 02_boolean_arith/   # Project 2
    │   └── 03_sequential/      # Project 3
    └── reflections.md      # What each project taught you
```

---

## ✅ Project Checklist

- [ ] Number systems — binary/hex/two's complement drilled
- [ ] Fixed-point representation — understand Q format (e.g., Q1.15)
- [ ] Boolean algebra — simplification by hand
- [ ] K-maps — 2, 3, and 4-variable examples
- [ ] nand2tetris Project 1 — Basic gates (And, Or, Mux, DMux…)
- [ ] nand2tetris Project 2 — Arithmetic (half-adder → ALU)
- [ ] nand2tetris Project 3 — Sequential (Bit → Register → RAM8 → PC)
- [ ] FSM design — traffic light (Moore), sequence detector (Mealy)
- [ ] FSM design — vending machine (full state table + diagram)

---

## 🛠️ Tools

| Tool | Purpose | Link |
|------|---------|------|
| nand2tetris simulator | Run HDL projects 1–3 | [nand2tetris.org](https://www.nand2tetris.org) |
| draw.io | Block diagrams, state diagrams | [diagrams.net](https://app.diagrams.net) — free, browser-based |
| Pen + paper | Timing diagrams, K-maps | Your desk |

---

## 📖 Resources

- [nand2tetris](https://www.nand2tetris.org) — free course + simulator. Do chapters 1–3.
- *Digital Design and Computer Architecture* (Harris & Harris) — chapters 1–3 as reference
- [Ben Eater's 8-bit computer series](https://www.youtube.com/c/BenEater) — optional but excellent intuition builder

---

## 💡 Key Insight from this Phase

> *HDL is not code that runs. It is a description of wires and gates that exist in parallel. Everything in a hardware design is always "executing" simultaneously — there is no sequential flow unless you explicitly build it with clocks and state.*

Write this on a sticky note and put it on your monitor.

---

**Next →** [02 · HDL / SystemVerilog](https://github.com/YOUR_USERNAME/fpga-02-hdl-sv)
