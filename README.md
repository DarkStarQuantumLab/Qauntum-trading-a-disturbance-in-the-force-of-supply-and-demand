# Improving strategic games using quantum computing

[*Quantum game theory*](https://link.springer.com/article/10.1007/s11128-018-2082-8) studies how strategic interactions, also referred to as strategic games or non-cooperative games, can be improved upon when implemented on quantum computers. Non-cooperative games are ubiquitous, manifesting in biological settings when organisms compete over finite resources, in international relations when self-enforcing policies, [like those for climate change](https://blogs.cornell.edu/info2040/2019/09/24/nash-equilibrium-and-climate-change/#:~:text=With%20climate%20change%20in%20theory,not%20care%20about%20carbon%20emission2) are to be drafted, in financial transactions, and in the design of supply-chain and network protocols. In all these settings, the solution of a non-cooperative game is the *Nash equilibrium*, a specific, stronger instance of multi-criteria optimization (MOO) in which each player's payoff in the game is the best possible, given the payoff to all other players. 

When non-cooperative games like Prisoner's Dilemma are played on a quantum computer, features of the quantum realm produce [Nash equilibria that are better paying than those possible on a conventional computer](https://doi.org/10.1103/PhysRevLett.83.3077). This phenomenon holds real-world utility in the form of better paying trades when applied to online trading. 

### Online trading on the quantum cloud
The current version of this project gives Qiskit code for playing Prisoner's Dilemma on IBM's quantum computer. This is a first step in modeling and implementing [high-frequency trading (HFT) as Prisoner's Dilemma using cloud-based quantum processors](https://www.frontiersin.org/articles/10.3389/frai.2021.769392/full). The final version of this project envisions deploying a HFT-on-quantum-cloud platform. 

### Why are quantum computed Nash equilibria better? 
When a non-cooperative game like Prisoner's Dilemma is played on a computing system, the system can be viewed as a ''referee'' who correlates the outcomes of the game in a way that is impossible when the players randomize over their respective strategies independently. The referee then tells each player what strategy they should play to achieve the expected payoff from the correlation. If each player agrees with the referee, the resulting equilibrium is called a *correlated equilibrium*. A correlated equilibrium is simply Nash equilibrium in the proper extension of a game to include a referee-enabled correlations. Correlated equilibria can be better quality than the original Nash equilibria. 

**When a game is played on a quantum computing system, the "quantum referee" can create quantum correlation that are stronger than the classical correlation of the conventional referee, and this can result in better quality Nash equilibria in the quantum (extension of a) game**. 

### Calculating Nash equilibria on a quantum computer
There exists the separate problem of calculating Nash equilibrium, a computationally intensive process for large games. To mitigate this, quantum annealers can be used to accelerae its calculation. See: https://github.com/DarkStarQuantumLab/NashEquilibrium. 

## How to run

1. In Google Collab through pip install qiskit (provided in the Notebook). The IBM Q account token may be required. 
2. Or upload the notebook to the IBM Quantum Lab (https://quantum-computing.ibm.com/). No installations are required, simply import required frameworks.

# License
This work is licensed under the [Apache 2 License](https://www.apache.org/licenses/LICENSE-2.0) and is owned by [Dark Star Quantum Lab Inc](https://www.darkstarquantumlab.com/)

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

# References

1. [Khan FS, Bao N. Quantum Prisoner's Dilemma and High Frequency Trading on the Quantum Cloud. Front Artif Intell. 2021 Nov 3;4:769392. doi: 10.3389/frai.2021.769392. PMID: 34805975; PMCID: PMC8596374.](https://pubmed.ncbi.nlm.nih.gov/34805975/)

2. [J. Eisert, M. Wilkens, M. Lewenstein. Quantum Games and Quantum Strategies. Phys. Rev. Lett. 83, 3077 (1999). Sep 1999.](https://arxiv.org/abs/quant-ph/9806088)

3. [J. Eisert, M. Wilkens. Quantum Games. J. Mod. Opt. 47 (2000) 2543. Apr 2000.](https://arxiv.org/abs/quant-ph/0004076)

4. [Adrian P. Flitney, Lloyd C. L. Hollenberg. Nash equilibria in quantum games with generalized two-parameter strategies. Phys. Lett. A 363 (2007) 381-388. Oct 2006.](https://arxiv.org/abs/quant-ph/0610084)

5. [The Qiskit Tutorials: The Density Matrix and Mixed States. IBM Q.](https://qiskit.org/textbook/ch-quantum-hardware/density-matrix.html)



