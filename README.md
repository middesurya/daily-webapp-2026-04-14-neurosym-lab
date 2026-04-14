# NeuroSym Lab — Interactive Neuro-Symbolic AI Reasoning Laboratory

An in-browser laboratory that lets you **see, build, and compare** hybrid neuro-symbolic AI reasoning pipelines. Watch how combining neural perception with symbolic logic produces reasoning that's more accurate, explainable, and up to 100× more energy-efficient.

## Why Neuro-Symbolic AI?

In April 2026, researchers demonstrated that combining neural networks with symbolic reasoning can slash AI energy use by **100×** while **improving accuracy**. This lab makes that breakthrough interactive and visual.

## Features

### Reasoning Arena
Three interactive challenges comparing pure neural vs neuro-symbolic approaches:
- **Visual Sudoku**: CNN reads digits → constraint propagation solves logically
- **Scene Reasoning**: Object detection → first-order logic inference
- **Word Problems**: NLP parsing → algebraic equation solving

### Pipeline Builder
Drag-and-drop neural and symbolic modules to compose custom reasoning pipelines. Watch data flow through CNNs, transformers, SAT solvers, Prolog engines, and more.

### Energy Dashboard
Real-time comparison of compute costs (FLOPs, memory, latency) with CO₂ impact visualization and scaling curves showing how the efficiency gap grows with problem complexity.

### Knowledge Graph Explorer
Interactive force-directed knowledge graphs with symbolic inference. Watch transitivity, inheritance, and abduction rules fire in real-time.

## Tech Stack

- Single HTML file (~70KB)
- D3.js for graph visualizations
- Pure JavaScript symbolic reasoning engines
- No external data fetches — fully self-contained
- Dark theme with glassmorphism UI

## Live Demo

[neurosym-lab.vercel.app](https://neurosym-lab.vercel.app)

## Inspiration

- [Neuro-symbolic AI achieves 100× energy reduction](https://www.sciencedaily.com/releases/2026/04/260405003952.htm)
- [IBM-MIT Watson AI Lab Neuro-Symbolic Research](https://mitibmwatsonailab.mit.edu/category/neuro-symbolic-ai/)
- [ICLR 2026 Mechanistic Interpretability](https://arxiv.org/pdf/2510.02917)

## License

MIT — Built with Claude Code 🤖
