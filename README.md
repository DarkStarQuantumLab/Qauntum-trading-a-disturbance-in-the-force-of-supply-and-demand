# Qiskit implementation of the Eisert, Wilkens, and Lewewnstein (EWL) protocol for executing the non-cooperative game Prisoner's Dilemma on a quantum computer

*Quantum game theory* studies how strategic interactions (non-cooperative games) can be improved when implemented using the emerging technology of quantum computers. Non-cooperative games are ubiqituous, manifesting in biological settings when organisms compete over finite resources, in international relations when self-enforcing international policies (like those for climate change) are to be drafted, in financial transactions, and in the desgin of supply-chain and network protocols. In all these settings, the fundamental solution of a non-cooperative game is the *Nash equilibrium*, a specific, stronger form of multi-criteria optimization (MOO) where each player's payoff in the game is the best possible given the payoff of all other players. 

Calculating Nash equilibrium can be a computationally intensive problem for large games (many players with many strategies). To mitigate this, quantum computers can be used to accelarate its calculation (see https://github.com/DarkStarQuantumLab/NashEquilibrium). 

A more dramatic aspect of quantum game theory can be observed when a non-cooperative game is played or implenented on a quantum computer. In this case, features of the quantum realm conspire to produce Nash equilibria (there can be more than one) that are better paying than those possible on a conventional computer (https://doi.org/10.1103/PhysRevLett.83.3077). This phenomenon has immediate utility in practical non-cooperative games like online (high-frequency) trading (https://www.frontiersin.org/articles/10.3389/frai.2021.769392/full) where the quantum computational implementation can produce better paying trades for the players. 



## How to run

1. In Google Collab through pip install qiskit (provided in the Notebook). The IBM Q account token may be required. 
2. Or upload the notebook to the IBM Quntum Lab (https://quantum-computing.ibm.com/). No installations are required, simply import required frameworks.
