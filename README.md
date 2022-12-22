# Improving strategic games using quantum computing

[*Quantum game theory*](https://link.springer.com/article/10.1007/s11128-018-2082-8) studies how strategic interactions, also referred to as strategic games or non-cooperative games, can be improved upon when implemented on quantum computers. Non-cooperative games are ubiqituous, manifesting in biological settings when organisms compete over finite resources, in international relations when self-enforcing policies (like those for climate change) are to be drafted, in financial transactions, and in the desgin of supply-chain and network protocols. In all these settings, the fundamental solution of a non-cooperative game is the *Nash equilibrium*, a specific, stronger instance of multi-criteria optimization (MOO) in which each player's payoff in the game is the best possible, given the payoff to all other players. 

When non-cooperative games like Prisoner's Dilemma are played on a quantum computer, features of the quantum realm produce [Nash equilibria that are better paying than those possible on a conventional computer](https://doi.org/10.1103/PhysRevLett.83.3077). This phenomenon holds real-world utility in the form of better paying trades when applied to online trading. 

### Online trading on the quantum cloud
The currenct version of this project gives Qiskit code for an initial "pure strategy" implemention of Prisoner's Dilemma on IBM's quantum computer. This is a first step in modeling and implementing [high-frequency trading (HFT) as Prisoner's Dilemma using cloud-based quantum processors](https://www.frontiersin.org/articles/10.3389/frai.2021.769392/full). The final version of this project envisions deploying a HFT-on-quantum-cloud platfom. 

### Why are the Nash equilibria better? 
When a non-ccoperative game like Prisoner's Dilemma is played on a computing system, the system can be viewed as a ``referee'' who correlates the outcomes of the game in a way that is impossible when the players randmoize over their strategies independently. The referee then tells each player what strategy they should play to achieve the expected payoff from the correaltion. If each player agrees with the referee, the resulting equilibrium is called a *correlated equilibrium*. A correlated equilibrium is simply Nash equilibrium in the proper extension of a game to include correlations (see section 5 of the paper "Quantized Poker" found here - https://arxiv.org/pdf/0902.2196.pdf). Correlated equilibria can be better quality than the original Nash equilibria. 

When a game is played on a quantum computing system, the "quantum referee" can create quantum correlation that are stronger than the classical correalteion of the conventional referee, and this can result in better quality Nash equilibria in the quantum (extension of a) game. 

### Calculating Nash equilibria on a quantum computer
There exists the seperate problem of calculating Nash equilibrium, a computationally intensive process for large games. To mitigate this, quantum annealers can be used to accelarate its calculation. For example, see: https://github.com/DarkStarQuantumLab/NashEquilibrium. 

## How to run

1. In Google Collab through pip install qiskit (provided in the Notebook). The IBM Q account token may be required. 
2. Or upload the notebook to the IBM Quntum Lab (https://quantum-computing.ibm.com/). No installations are required, simply import required frameworks.
