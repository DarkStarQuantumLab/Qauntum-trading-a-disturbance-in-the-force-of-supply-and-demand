# Qiskit implementation of the Eisert, Wilkens, and Lewewnstein (EWL) protocol for playing Prisoner's Dilemma on a quantum computer

*Quantum game theory* studies how strategic interactions (non-cooperative games) can be improved when implemented using the emerging technology of quantum computers (a review of quantum game theory: https://link.springer.com/article/10.1007/s11128-018-2082-8). Non-cooperative games are ubiqituous, manifesting in biological settings when organisms compete over finite resources, in international relations when self-enforcing international policies (like those for climate change) are to be drafted, in financial transactions, and in the desgin of supply-chain and network protocols. In all these settings, the fundamental solution of a non-cooperative game is the *Nash equilibrium*, a specific, stronger form of multi-criteria optimization (MOO) where each player's payoff in the game is the best possible given the payoff of all other players. 

Calculating Nash equilibrium can be a computationally intensive problem for large games (many players with many strategies). To mitigate this, quantum computers can be used to accelarate its calculation (see https://github.com/DarkStarQuantumLab/NashEquilibrium). 

When non-cooperative games are played on a quantum computer, features of the quantum realm conspire to produce Nash equilibria (there can be more than one) that are better paying than those possible on a conventional computer (https://doi.org/10.1103/PhysRevLett.83.3077). This phenomenon has immediate utility in practical non-cooperative games like online trading where the quantum computational implementation can produce better paying trades for the players. A proposal for implementng high-frequency trading (HFT) using cloud-based quantum processors appears in https://www.frontiersin.org/articles/10.3389/frai.2021.769392/full. The ultimate goal of this project to implement HFT on a quantum cloud.



## How to run

1. In Google Collab through pip install qiskit (provided in the Notebook). The IBM Q account token may be required. 
2. Or upload the notebook to the IBM Quntum Lab (https://quantum-computing.ibm.com/). No installations are required, simply import required frameworks.
