# Computational Scientist — Part 2

This folder documents the **Computational Scientist part** of Problem Set 1 for COMSCI/ECON 206 (*Computational Microeconomics, Fall 2025*).  
It reproduces equilibria for the **3-player Public Goods Game** (endowment = 100, multiplier = 1.8) using open-source computational tools.

---

## Contents

- [`notebook.ipynb/`](notebook.ipynb/) — Google Colab export with normal-form payoff matrices, Nash equilibrium computations, and solver outputs.  
- [`gte/`](gte/) — Game Theory Explorer files (extensive-form tree + SPNE solution).  
- [`screenshots/`](screenshots/) — Captures of payoff matrices, solver output, and GTE solution panels (with captions).  

---

## How to Run

### 1. Open the Notebook
Run in **Google Colab** or locally via Jupyter.

Colab (recommended):  
```bash
# In Colab, first install dependencies
!pip install nashpy quantecon
```
Then upload or open `notebook.ipynb` and execute cells.

---

### 2. Required Libraries

- [NashPy](https://nashpy.readthedocs.io/en/stable/) — equilibrium solver for 2-player games (Knight 2021).  
- [QuantEcon](https://quantecon.org/quantecon-py/) — computational economics library (Sargent & Stachurski 2021).  
- Python 3.9+ recommended.

---

### 3. Outputs

The notebook includes:

- Display of **normal-form payoff matrices**.  
- Computation of **Nash equilibria** via NashPy.  
- Visualization of solver outputs and welfare comparison.  

---

## Game Theory Explorer (GTE)

<img width="1144" height="657" alt="1" src="https://github.com/user-attachments/assets/ee58331d-8f64-4bde-936e-37a0fe9e372c" />

In addition to the notebook:

- The **extensive-form representation** of the PGG was built in [Game Theory Explorer](http://www.gametheoryexplorer.org/).  
- Players, histories, and information sets are labeled.  
- **SPNE solution** was computed using GTE’s built-in tool.  
- Screenshots in `screenshots/` include:  
  1. Game tree with labeled histories.  
  2. SPNE solution panel.  

<img width="421" height="574" alt="3" src="https://github.com/user-attachments/assets/c21efd5b-ea1e-4e3d-ab1b-018c905be75e" />

**Interpretation:** The SPNE outcome coincides with the Nash equilibrium of the simultaneous normal form (all players contribute 0), illustrating that refinements do not alter predictions under this payoff structure.

---

## Reproducibility Notes

- Ensure Python libraries are installed before running the notebook.  
- All GTE exports are included in `gte/` for reproducibility.  
- Screenshots are annotated with captions for clarity.  
- Software tools used must be cited in final reports:  
  - Thomas J. Sargent and John Stachurski (2021). *Quantitative Economics (Python)*, Version 0.5.1.  
  - Vincent Knight (2021). *Nashpy: A Python library for the computation of equilibria of 2-player strategic games*, Version 0.0.28.  
  - Rahul Savani and Bernhard von Stengel (2015). *Game Theory Explorer – Software for the Applied Game Theorist*. *Computational Management Science*, 12: 5–33.  

---

## References (Selected)

- Shoham, Y. & Leyton-Brown, K. (2008). *Multiagent Systems: Algorithmic, Game-Theoretic, and Logical Foundations*. Cambridge University Press.  
- Osborne, M. J. & Rubinstein, A. (1994). *A Course in Game Theory*. MIT Press.  
- Roughgarden, T. (2016). *Twenty Lectures on Algorithmic Game Theory*. Cambridge University Press.  
- Problem Set 1 Instructions — COMSCI/ECON 206 (Fall 2025).  

