# 📘 JTPMath Research

> *Mathematics in structural motion.*

This repository hosts the research, proofs, and LaTeX development pipeline for **[JTPMath.com](https://jtpmath.com)**.

---

## 🔭 Purpose

The **research** repository is the mathematical workspace for:

- 📄 LaTeX papers and drafts (Burns Law, RH, BSD Resolution, etc.)  
- 🧮 Equations, simulations, and analytic derivations  
- 🧠 Notes and intuition logs generated during AI-assisted exploration  
- 🧰 Tools and scripts used in theorem verification and visualization  

Each project is versioned and documented to preserve both **proof structure** and **discovery process**.

---

## 🧩 Structure

```

research/
│
├── papers/            # Complete or draft LaTeX papers
│   ├── burns-law/
│   ├── riemann-disproof/
│   └── bsd-resolution/
│
├── notes/             # AI-assisted and manual research logs
│   ├── field-journals/
│   └── idea-snapshots/
│
├── figures/           # Graphs, visualizations, simulation outputs
│
└── tex-template/      # Shared LaTeX macros and document skeletons

````

---

## ⚙️ Workflow

1. **Exploration:**  
   Research begins in dialogue — with human intuition and AI computation producing conjectures and structural insights.

2. **Verification:**  
   All results are re-derived manually or symbolically until rigor is confirmed.

3. **Archival:**  
   When a paper or proof is complete, it’s tagged as `published` and mirrored on [JTPMath.com](https://jtpmath.com).

---

## 🧪 Reproducibility

### 🔧 Requirements

- **TeX distribution:** TeX Live or MiKTeX  
- **Editor:** Overleaf, TeXstudio, or VS Code with LaTeX Workshop  
- **Build tools:** `pdflatex`, `biber`, and `makeglossaries`  
- **Python (optional):** for analytic plots or symbolic checks  
  - Recommended libraries: `sympy`, `numpy`, `matplotlib`

---

### 🧮 Build Instructions

Each paper can be built independently:

```bash
cd papers/burns-law
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
````

For Python-backed computations (if present):

```bash
python3 compute.py
```

This regenerates data tables or figures referenced in the paper.

---

### 📁 Environment Replication

If you want to recreate the full LaTeX + computation environment:

```bash
git clone https://github.com/jtpmath/research.git
cd research
# Compile any paper
make burns-law
```

You can also install the lightweight environment via:

```bash
conda env create -f environment.yml
conda activate jtpmath
```

*(The `environment.yml` will include TeX build tools, Python packages, and symbolic computation libraries.)*

---

## ✍️ Author

**Jasmine Burns**
Founder of [JTPMath.com](https://jtpmath.com)
Mathematician and independent researcher in analytic number theory, ergodic systems, and structural recursion.

---

## 🧠 Philosophy

> “Mathematics is not computation but structure recognizing itself.”
> — *JTPMath Principle*

This repository embodies that principle: AI and human reasoning working together to accelerate intuition, preserve rigor, and document discovery as it unfolds.

---

## 📜 License

All original research and LaTeX source files are © Jasmine Burns 2025.
For collaboration or citation inquiries, contact via [JTPMath.com/contact](https://jtpmath.com/contact).
