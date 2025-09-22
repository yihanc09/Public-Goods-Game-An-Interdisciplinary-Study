# Public Goods Game: An Interdisciplinary Study

## Abstract
This repository supports **Problem Set 1 & 2** for COMSCI/ECON 206: *Computational Microeconomics (Autumn 2025)*.  
It deploys a classic linear **Public Goods Game (PGG)** in oTree and analyzes it through three complementary lenses:  

1. **Economist**: Theoretical analysis using Nash equilibrium, welfare benchmarks, and refinements.  
2. **Computational Scientist**: Reproduction of equilibria using Google Colab (NashPy/QuantEcon) and Game Theory Explorer (GTE).  
3. **Behavioral Scientist**: Experimental implementation with human participants and large language model (LLM) agents, followed by comparative analysis.
4. **Extension (Problem Set 2)**: Testing the **Winner’s Curse** phenomenon with AI agents, connecting game theory to mechanism design and auction environments.

The game features **3 players**, **8 rounds**, **endowment = 100**, and **multiplier = 1.8**.  
This setup generates a strict social dilemma: equilibrium predicts full free-riding (0 contributions), while efficiency requires full cooperation (100 contributions).

### Supplementary Materials

The full written report for this project is available as a PDF:

- [`report-PS1.pdf`](report-PS1.pdf/) — complete interdisciplinary analysis (Economist, Computational Scientist, Behavioral Scientist), including explanations, figures, screenshots, and references.
- [`report-PS2.pdf`](report-PS2.pdf/) — extended analysis for **Problem Set 2** (focus on mechanism design and Winner’s Curse experiments).  

These PDFs complement the repository by providing the **formal write-up**, while the repository folders provide **all supporting code, screenshots, and reproducible assets**.

For reproducibility, a [`requirements.txt`](requirements.txt) file is included to install all necessary Python dependencies.

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

- **Part 4 — Extension (Problem Set 2)**  
  Explore **Winner’s Curse** dynamics by designing a simple auction environment.  
  Compare predictions from mechanism design theory with simulated play by human participants and AI agents, highlighting where bounded rationality or misperception of value drives outcomes away from equilibrium.  
  Discuss implications for using AI in market design and economic experiments.

---

## Repository Structure Overview

### Problem Set 1 — Public Goods Game (PGG)

| Role / Part             | Folder / File | Contents |
|--------------------------|---------------|----------|
| **Economist**            | [`economist/`](economist/) | Equilibrium definitions, citations, references (`README.md`, `refs/`) |
| **Computational Scientist** | [`computational_scientist/`](computational_scientist/) | Jupyter notebook with payoff matrices and solver outputs (`notebook.ipynb`), screenshots, GTE exports |
| **Behavioral Scientist** | [`behavioral_scientist/`](behavioral_scientist/) | oTree app (`otree_app.zip`), screenshots of human sessions, LLM session data (`llm/` with prompts, transcripts, settings) |


### Problem Set 2 — Mechanism Design (Winner’s Curse Extension)

| Component                | Folder / File | Contents |
|--------------------------|---------------|----------|
| **Overview & Theory**    | [`mechanism_design/README.md`](mechanism_design/README.md) | Explanation of auction design, hypotheses, and link to mechanism design theory |
| **AI Simulation Setup**  | [`prompts_setup_gpt5.txt`](mechanism_design/prompts_setup_gpt5.txt), [`prompts_setup_claude.txt`](mechanism_design/prompts_setup_claude.txt) | Exact LLM prompts and interface rules |
| **Transcripts**          | [`transcript_gpt5.md`](mechanism_design/transcript_gpt5.md), [`transcript_claude.md`](mechanism_design/transcript_claude.md) | Recorded reasoning and choices from GPT-5 and Claude |
| **Decision Logs**        | [`decision_log_gpt5.csv`](mechanism_design/decision_log_gpt5.csv), [`decision_log_claude.csv`](mechanism_design/decision_log_claude.csv) | Raw outputs from simulated play (round-by-round decisions) |

### Supplementary

- [`report-PS1.pdf`](report-PS1.pdf) — complete interdisciplinary analysis (PS1)  
- [`report-PS2.pdf`](report-PS2.pdf) — mechanism design extension (PS2)  
- [`requirements.txt`](requirements.txt) — Python dependencies for reproducibility


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

5. **Mechanism Design (Problem Set 2 Extension)**  
   - See [`mechanism_design/README.md`](mechanism_design/README.md) for an overview of the auction design, theoretical motivation, and hypotheses.  
   - Prompts and setup instructions for AI simulations are provided in  
     [`mechanism_design/prompts_setup_gpt5.txt`](mechanism_design/prompts_setup_gpt5.txt) and  
     [`mechanism_design/prompts_setup_claude.txt`](mechanism_design/prompts_setup_claude.txt).  
   - Transcripts of simulated play are in  
     [`mechanism_design/transcript_gpt5.md`](mechanism_design/transcript_gpt5.md) and  
     [`mechanism_design/transcript_claude.md`](mechanism_design/transcript_claude.md).  
   - Decision logs (raw outputs in CSV format) are stored in  
     [`mechanism_design/decision_log_gpt5.csv`](mechanism_design/decision_log_gpt5.csv) and  
     [`mechanism_design/decision_log_claude.csv`](mechanism_design/decision_log_claude.csv).  
   - Together, these materials document how the Winner’s Curse experiment was conducted with AI agents and enable replication or extension of the simulations.
     
6. **Bibliography and citations**  
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
└── mechanism_design/
    ├── README.md         # Explanation of PS2 extension (Winner’s Curse, mechanism design link)
    ├── prompts_setup_gpt5.txt        # Prompts, rules, and interface setup
    ├── prompts_setup_claude.txt
    ├── transcript_gpt5.md            # Transcripts
    ├── transcript_claude.md
    ├── decision_log_gpt5.csv         # Decision log
    └── decision_log_claude.csv         
```

---

## License
This repository is for educational purposes within **COMSCI/ECON 206: Computational Microeconomics (Fall 2025)**.  
Please cite all tools and references appropriately.
