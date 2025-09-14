# Economist — Public Goods Game (Part 1)

This folder documents the **Economist part** of Problem Set 1 for COMSCI/ECON 206.  
It focuses on **theoretical analysis** of the Public Goods Game (PGG) with 3 players, 8 rounds, endowment = 100, multiplier = 1.8.

---

## Equilibrium Concept

- **Choice of concept**: Nash Equilibrium (NE) in pure strategies is the most appropriate since the game is simultaneous-move and complete-information.  
- **Definition**: A strategy profile $s^* \in S$ is a Nash equilibrium if for every player $i \in N$, u<sub>i</sub>(s<sub>i</sub><sup>*</sup>, s<sub>-i</sub><sup>*</sup>) ≥
u<sub>i</sub>(s<sub>i</sub>, s<sub>-i</sub><sup>*</sup>) for all
s<sub>i</sub> ∈ S<sub>i</sub>
(Osborne & Rubinstein 1994, Ch. 2, p. 14).

- **Existence theorem**:  
  - Nash (1950, *PNAS*, p. 48–49) proves that every finite game admits at least one mixed-strategy equilibrium.  
  - Glicksberg (1952, *PAMS*, p. 170–174) extends the result to compact, convex action sets and continuous payoffs.  
  - Existence follows from Kakutani’s fixed point theorem (Shoham & Leyton-Brown 2008, Sec. 2.2, pp. 35–37).

---

## Analytical Solution

- **Best response logic**: With MPCR = m / n = 0.6 < 1, contributing reduces private payoff by 0.4 per unit.  
  Thus the dominant strategy is g<sub>i</sub><sup>*</sup> = 0 for all players.

- **Equilibrium outcome**:  
  (g<sub>1</sub><sup>*</sup>, g<sub>2</sub><sup>*</sup>, g<sub>3</sub><sup>*</sup>) = (0, 0, 0)

- **Efficiency**:  
  - **NE welfare**: W<sub>NE</sub> = 300  
  - **Social optimum**: W<sub>opt</sub> = 540 at full contribution (100, 100, 100).

- **Fairness**:  
  - NE is equal but inefficient.  
  - At asymmetric profiles, inequality and strategic envy emerge.  
  - Full cooperation maximizes utilitarian welfare but is not stable under NE reasoning.

---

## Interpretation

- **Realism**: NE predicts free-riding only, but experiments (Ledyard 1995, Handbook, pp. 111–194) show humans often contribute positively in early rounds.  
- **Multiplicity**: At MPCR = 1, multiple equilibria exist; refinements like correlated equilibrium (Aumann 1974, *JME*, p. 67–96) or trembling-hand perfection (Selten 1975, *IJGT*, p. 25–55) apply.  
- **Bounded rationality (Week 1)**: Agents use heuristics like reciprocity or fairness norms, leading to transient cooperation beyond NE.  
- **Computational tractability (Week 2)**:  
  - Simple here (unique NE easily derived).  
  - In general, computing NE is **PPAD-complete** (Daskalakis, Goldberg & Papadimitriou 2009, *SIAM J. Comput.*, p. 195–259).  
  - Tools like Game Theory Explorer and NashPy help overcome tractability in practice.

---

## References

- Aumann, R. (1974). *Subjectivity and correlation in randomized strategies*. **Journal of Mathematical Economics**, 1(1): 67–96.  
- Daskalakis, C., Goldberg, P. W., & Papadimitriou, C. H. (2009). *The complexity of computing a Nash equilibrium*. **SIAM Journal on Computing**, 39(1): 195–259.  
- Glicksberg, I. L. (1952). *A further generalization of the Kakutani fixed point theorem, with applications to Nash equilibrium*. **Proceedings of the American Mathematical Society**, 3: 170–174.  
- Ledyard, J. O. (1995). *Public goods: A survey of experimental research*. In J. Kagel & A. Roth (eds.), **Handbook of Experimental Economics**, pp. 111–194. Princeton University Press.  
- Nash, J. F. (1950). *Equilibrium points in n-person games*. **Proceedings of the National Academy of Sciences**, 36: 48–49.  
- Osborne, M. J. & Rubinstein, A. (1994). *A Course in Game Theory*. MIT Press. (Ch. 2, p. 14)  
- Selten, R. (1975). *Reexamination of the perfectness concept for equilibrium points in extensive games*. **International Journal of Game Theory**, 4: 25–55.  
- Shoham, Y. & Leyton-Brown, K. (2008). *Multiagent Systems: Algorithmic, Game-Theoretic, and Logical Foundations*. Cambridge University Press. (Sec. 2.2, pp. 35–37)
