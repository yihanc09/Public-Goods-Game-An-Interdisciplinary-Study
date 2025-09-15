# Public Goods Game: An Interdisciplinary Study

## Abstract
This repository supports **Problem Set 1** for COMSCI/ECON 206: *Computational Microeconomics (Autumn 2025)*.  
It deploys a classic linear **Public Goods Game (PGG)** in oTree and analyzes it through three complementary lenses:  

1. **Economist**: Theoretical analysis using Nash equilibrium, welfare benchmarks, and refinements.  
2. **Computational Scientist**: Reproduction of equilibria using Google Colab (NashPy/QuantEcon) and Game Theory Explorer (GTE).  
3. **Behavioral Scientist**: Experimental implementation with human participants and large language model (LLM) agents, followed by comparative analysis.  

The game features **3 players**, **8 rounds**, **endowment = 100**, and **multiplier = 1.8**.  
This setup generates a strict social dilemma: equilibrium predicts full free-riding (0 contributions), while efficiency requires full cooperation (100 contributions).

### Supplementary Materials

The full written report for this project is available as a PDF:

- [`report-LaTeX.pdf`](report-LaTeX.pdf/) — complete interdisciplinary analysis (Economist, Computational Scientist, Behavioral Scientist), including explanations, figures, screenshots, and references.

This PDF complements the repository by providing the **formal write-up**, while the repository folders provide **all supporting code, screenshots, and reproducible assets**.


---

## Task Summary
This project demonstrates the interdisciplinary workflow for deploying and analyzing a strategic game:

- **Part 1 — Economist**:  
  Define the equilibrium concept, prove existence, solve analytically, and discuss efficiency and fairness.

- **Part 2 — Computational Scientist**:  
  Simulate and compute equilibria with open-source tools (NashPy, QuantEcon, GTE). Provide normal-form payoff matrices and extensive-form trees.

- **Part 3 — Behavioral Scientist**:  
  Run oTree sessions with classmates, deploy an LLM “ChatBot” as a rational agent, and compare outcomes to equilibrium predictions.  
  Propose refinements (Heuristic-Nash Equilibrium, Linguistically Framed Equilibrium) to capture human vs. AI divergences.

---

## Reproduction Steps
To reproduce the results in this repository:

1. **Clone the repository**  
   ```bash
   git clone https://github.com/yihanc09/Public-Goods-Game-An-Interdisciplinary-Study.git
   cd PublicGoodsGame-AnInterdisciplinaryStudy

2. **Economist (theory & welfare)**  
   - Read [`economist/`](economist/) for definitions, citations, and references.  
   - Contains LaTeX writeups with rigorous notation and proofs.

3. **Computational Scientist (coding & tools)**  
   - Open [`computational_scientist/notebook.ipynb`](computational_scientist/notebook.ipynb) in Google Colab or Jupyter.  
   - Requirements: `nashpy`, `quantecon`.  
   - Explore the GTE screenshots under [`computational_scientist/screenshots/`](computational_scientist/screenshots/).

   Example Colab run:
   ```python
   !pip install nashpy quantecon
   # Load and run notebook.ipynb

4. **Behavioral Scientist (experiment & AI)**  
   - Run the oTree app in [`behavioral_scientist/pgg.otreezip`](behavioral_scientist/pgg.otreezip).  
   - Instructions and screenshots of the 8-round human session are in [`behavioral_scientist/screenshots/`](behavioral_scientist/screenshots/).  
   - LLM transcripts, prompts, and settings are stored in [`behavioral_scientist/llm/`](behavioral_scientist/llm/).

5. **Bibliography and citations**  
   - All references (textbook, software, and literature) are in [`refs/`](economist/refs/) in Chicago (author-date) style.  
   - Required software citations include:  
     - Thomas J. Sargent and John Stachurski (2021). *Quantitative Economics (Python)*, Version 0.5.1.  
     - Vincent Knight (2021). *Nashpy: A Python library for the computation of equilibria of 2-player strategic games*, Version 0.0.28.  
     - Rahul Savani and Bernhard von Stengel (2015). *Game Theory Explorer – Software for the Applied Game Theorist*.  

---

## Repository Structure

```bash
PublicGoodsGame-AnInterdisciplinaryStudy/
│── README.md
│
├── economist/
│   ├── README.md        # Definitions, citations, references
│   └── refs/            # PDFs, BibTeX files
│
├── computational_scientist/
│   ├── notebook.ipynb   # Colab export
│   ├── README.md        # How-to-run + screenshots
│   └── gte/             # Optional GTE exports
│
├── behavioral_scientist/
│   ├── otree_app.zip    # oTree deployment
│   ├── screenshots/     # Human session screenshots
│   ├── llm/             # Prompts, transcript, settings
│   └── README.md        # Deployment steps + ethics note
│
└── refs/                # Central references (if consolidated)
```

---

## License
This repository is for educational purposes within **COMSCI/ECON 206: Computational Microeconomics (Fall 2025)**.  
Please cite all tools and references appropriately.
