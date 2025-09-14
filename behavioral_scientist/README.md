# Behavioral Scientist — Part 3

This folder documents the **Behavioral Scientist part** of Problem Set 1 for COMSCI/ECON 206 (*Computational Microeconomics, Fall 2025*).  
It covers the experimental deployment of the Public Goods Game (PGG) in **oTree**, alongside replication with **LLM agents**.

---

## Contents

- `pgg.otreezip` — Ready-to-run oTree app for the 3-player, 8-round PGG (endowment = 100, multiplier = 1.8).  
- `screenshots/` — Game pages (instructions, decision, results) and session outcomes with classmates.  
- `llm/` — Prompts (`prompts.txt`), transcripts (`transcript.md`), and session settings (`settings.json`) for LLM-based play.  

---

## Deployment Steps

1. **Install oTree**  
   ```bash
   pip install otree
   ```

2. **Unzip and run the app**
   ```bash
   unzip pgg.otreezip -d otree_pgg
   cd otree_pgg
   otree devserver
   ```

3. **Access the game**
   - Open [http://localhost:8000](http://localhost:8000) in your browser.  
   - Use the provided session configuration (see below).

---

## Session Configuration

- **Players**: 3  
- **Rounds**: 8  
- **Endowment**: 100 tokens  
- **Multiplier**: 1.8 (MPCR = 0.6)  
- **Groups**: Randomly assigned or fixed by session setup  
- **Recorded Data**: Individual contributions, payoffs, and round-by-round history  

---

## LLM “ChatBot” Session

- Prompts and role instructions are documented in `llm/prompts.txt`.  
- Session transcript with reasoning and choices is in `llm/transcript.md`.  
- Exact model settings are recorded in `llm/settings.json`.  

Comparisons are made across:
1. **Equilibrium predictions (theory)**  
2. **Human experiment session (screenshots)**  
3. **LLM session (transcript)**  

---

## Ethics Note

- **Human subjects**: All classmates gave informed consent; data was anonymized and collected for educational purposes only.  
- **AI agents**: Large Language Models (LLMs) are not considered research subjects under institutional review, but their use is documented transparently.  
- **Data sharing**: Screenshots and transcripts are provided strictly for course replication and must not be redistributed beyond this class without permission.  

---

## References (Selected)

- Ledyard, J. O. (1995). *Public goods: A survey of experimental research*. In J. Kagel & A. Roth (eds.), **Handbook of Experimental Economics**, pp. 111–194. Princeton University Press.  
- Savani, R., & von Stengel, B. (2015). *Game Theory Explorer – Software for the Applied Game Theorist*. **Computational Management Science**, 12, 5–33.  
- Problem Set 1 Instructions — COMSCI/ECON 206 (Fall 2025).  
