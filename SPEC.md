# NeuroSym Lab — Interactive Neuro-Symbolic AI Reasoning Laboratory

## Vision
An in-browser laboratory that lets users **see, build, and compare** hybrid neuro-symbolic AI reasoning pipelines. Users witness how neural perception modules extract features and symbolic logic engines apply rules — side by side — and see why this hybrid approach is up to 100x more energy-efficient than pure neural brute force.

## Why Now (April 2026)
- Researchers unveiled neuro-symbolic AI achieving 100x energy reduction with improved accuracy
- IBM-MIT Watson AI Lab driving neuro-symbolic research
- ICLR 2026 featured mechanistic interpretability papers bridging neural and symbolic
- Bay Area robotics (NVIDIA GTC 2026) using neuro-symbolic for embodied AI planning

## Core Features

### 1. Visual Reasoning Arena (Main Tab)
Three interactive challenges where users compare pure-neural vs neuro-symbolic:

**Challenge A: Visual Sudoku Solver**
- Neural module: CNN reads handwritten digits from a 4x4 grid image
- Symbolic module: Constraint propagation solver applies Sudoku rules
- Pure neural baseline: End-to-end transformer tries to solve directly
- Visualization: Confidence heatmaps, constraint propagation animation, step-by-step proof

**Challenge B: Scene Graph Reasoning**
- Neural module: Object detector identifies entities (cat, table, box)
- Symbolic module: First-order logic infers spatial relationships
- Query interface: "Is the cat on the table?" → see the full reasoning chain
- Visualization: Scene → detected objects → knowledge graph → logical inference

**Challenge C: Arithmetic Word Problems**
- Neural module: NLP parser extracts entities, quantities, relationships
- Symbolic module: Algebraic equation builder & solver
- Visualization: Text highlighting → extracted variables → equation tree → solution

### 2. Pipeline Builder (Tab 2)
- Drag-and-drop neural & symbolic modules onto a canvas
- Connect them with data flow edges
- Available neural modules: CNN, Transformer, Embedding, Attention
- Available symbolic modules: SAT Solver, Constraint Propagation, Prolog Engine, Graph Reasoner
- Run the pipeline on sample inputs and watch data flow through

### 3. Energy & Compute Dashboard (Tab 3)
- Real-time comparison: FLOPs, memory, latency for neural vs neuro-symbolic
- Animated bar charts showing the 100x efficiency gap
- Scaling curves: How efficiency gap grows with problem complexity
- CO₂ equivalent visualization (neural = burning X gallons of gas, neuro-symbolic = charging a phone)

### 4. Knowledge Graph Explorer (Tab 4)
- Interactive force-directed knowledge graph
- Add entities and relationships
- Run inference rules (transitivity, inheritance, abduction)
- Watch how symbolic reasoning propagates through the graph
- Compare with neural graph embedding approaches

## Tech Stack
- Single HTML file with embedded CSS/JS
- D3.js for graph visualizations and force layouts
- Canvas API for neural network activation visualizations
- No external data fetches — all data embedded inline
- Tailwind CSS via CDN for responsive layout
- Custom symbolic reasoning engine in pure JavaScript

## Architecture
```
index.html
├── Styles (Tailwind + custom CSS)
├── App Shell (tab navigation, dark mode)
├── Visual Reasoning Arena
│   ├── Sudoku Challenge (CNN sim + constraint solver)
│   ├── Scene Graph Challenge (object detection sim + FOL engine)
│   └── Word Problem Challenge (NLP parser sim + algebra solver)
├── Pipeline Builder (drag-and-drop canvas)
├── Energy Dashboard (animated charts)
└── Knowledge Graph Explorer (D3 force graph)
```

## Design
- Dark theme with neon accent colors (neural = cyan, symbolic = magenta, hybrid = gold)
- Glassmorphism panels
- Smooth animations for data flow visualization
- Split-screen comparisons with racing progress bars
- Mobile-responsive with collapsible panels
