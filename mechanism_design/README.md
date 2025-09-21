# Mechanism Design — AI Auction Experiments

This folder contains the materials for **Part 2: From Game Theory to Mechanism Design — Testing Winner’s Curse on AI Agents** of the COMSCI/ECON 206 Problem Set.  
It documents the design, setup, and results of first-price sealed-bid auction simulations run with two large language models (LLMs): **GPT-5** (OpenAI) and **Claude 3** (Anthropic).  

## Contents

- **Prompts and Setup Instructions**  
  Detailed prompts and interface setup for running the auction with LLMs are provided in:  
  - [`mechanism_design/prompts_setup_gpt5.txt`](/prompts_setup_gpt5.txt)  
  - [`mechanism_design/prompts_setup_claude.txt`](/prompts_setup_claude.txt)  

- **Transcripts of Simulated Play**  
  Full conversation transcripts showing reasoning and bid decisions for each model:  
  - [`mechanism_design/transcript_gpt5.md`](mechanism_design/transcript_gpt5.md)  
  - [`mechanism_design/transcript_claude.md`](mechanism_design/transcript_claude.md)  

- **Decision Logs**  
  Structured outputs of numeric bids recorded in CSV format:  
  - [`mechanism_design/decision_log_gpt5.csv`](mechanism_design/decision_log_gpt5.csv)  
  - [`mechanism_design/decision_log_claude.csv`](mechanism_design/decision_log_claude.csv)  

## Experiment Overview

- **Auction format:** First-price sealed-bid auction with private values \( v_i \sim U[0,100] \).  
- **Control group:** 5 bidders (\(n=5\)).  
- **Treatment group:** 10 bidders (\(n=10\)).  
- **Objective:** Test the hypothesis that larger bidder pools increase the likelihood of the *Winner’s Curse*.  
- **Agents:** GPT-5 and Claude were each tested as a bidder under both control and treatment conditions.  

## Notes

- Prompts were standardized across models to ensure comparability.  
- GPT-5 generally followed the symmetric Bayes–Nash equilibrium bidding rule closely.  
- Claude also followed equilibrium logic but introduced slight conservative adjustments, reflecting a more risk-averse style of play.  
- These contrasts illustrate how AI agents can replicate equilibrium play while also echoing human-like behavioral tendencies.  

