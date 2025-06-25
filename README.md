Cellular Automata Simulation for AI Innovation in Manufacturing Clusters
This repository contains MATLAB code used to generate the simulation figures for the manuscript titled "Drivers of Artificial Intelligence Innovation in Manufacturing Clusters: Insights from Cellular Automata Simulations". The code implements a Cellular Automata (CA) model to simulate the evolution of AI-driven innovation within manufacturing industry clusters, focusing on the impact of cluster resources (μ), cluster networks (r), and cluster environments (ε).
Overview
The simulations model the adoption and diffusion of AI technologies in a 20x20 grid of firms, using a von Neumann neighborhood configuration. The model parameters include:

μ: Resource ownership coefficient, representing the availability of resources like human capital, financial capital, and digital infrastructure.
r: Knowledge-sharing coefficient, reflecting the degree of inter-firm collaboration.
ε: External environment factor, capturing the influence of policy, economic conditions, and market demand.
p₀: Threshold probability (0.6) for state transitions to AI adoption.

Each script generates specific figures (Figures 5–11) from the manuscript, visualizing the initial state and the impact of varying parameters on AI innovation evolution.
Repository Contents

figure_001.m: Generates Figure 5, showing the initial state of the cellular space with randomly assigned firm states (0 for non-AI-adopting, 1 for AI-adopting).
figure_002.m: Generates Figure 6, illustrating the AI innovation evolution process with different μ values (0.3, 0.5, 0.7) when r = ε = 0.5.
figure_003.m: Generates Figure 7, plotting the number of AI-innovative firms over simulation iterations for different μ values.
figure_004.m: Generates Figure 8, showing the AI innovation evolution process with different r values (0.4, 0.6, 0.8) when μ = ε = 0.5.
figure_005.m: Generates Figure 9, plotting the number of AI-innovative firms over simulation iterations for different r values.
figure_006.m: Generates Figure 10, depicting the AI innovation evolution process with different ε values (0.4, 0.6, 0.8) when μ = r = 0.5.
figure_007.m: Generates Figure 11, plotting the number of AI-innovative firms over simulation iterations for different ε values.

Prerequisites

MATLAB: Version R2019b or later is recommended to ensure compatibility with the scripts.
Toolboxes: No additional MATLAB toolboxes are required beyond the core MATLAB installation.
System Requirements: Standard computing resources (e.g., 4GB RAM, dual-core processor) are sufficient for running the simulations.

Installation and Usage


Open MATLAB:Launch MATLAB and navigate to the cloned repository folder using the MATLAB file browser or the cd command in the MATLAB command window.

Run the Scripts:

To generate a specific figure, open the corresponding .m file (e.g., figure_001.m for Figure 5) in MATLAB.
Execute the script by clicking "Run" in the MATLAB editor or typing the script name (e.g., figure_001) in the command window.
The script will generate and display the figure, which can be saved manually from the MATLAB figure window.


Expected Output:

Each script produces a figure corresponding to the manuscript’s description (e.g., Figure 5 shows a 20x20 grid with green and blue cells representing AI-adopting and non-adopting firms, respectively).
Figures 7, 9, and 11 produce line plots showing the cumulative number of AI-innovative firms over 30 simulation iterations.



Script Details

Figure 5 (figure_001.m): Initializes a 20x20 grid with random binary states (0 or 1) using the randi function, visualized with green (S=1) and blue (S=0) cells.
Figure 6 (figure_002.m): Simulates AI innovation evolution for μ = [0.3, 0.5, 0.7], with fixed r = 0.5, ε = 0.5, over 30 iterations, showing grid states.
Figure 7 (figure_003.m): Quantifies the number of AI-adopting firms (S=1) for different μ values, plotted against simulation iterations.
Figure 8 (figure_004.m): Simulates AI innovation evolution for r = [0.4, 0.6, 0.8], with fixed μ = 0.5, ε = 0.5, over 30 iterations, showing grid states.
Figure 9 (figure_005.m): Quantifies the number of AI-adopting firms for different r values, plotted against simulation iterations.
Figure 10 (figure_006.m): Simulates AI innovation evolution for ε = [0.4, 0.6, 0.8], with fixed μ = 0.5, r = 0.5, over 30 iterations, showing grid states.
Figure 11 (figure_007.m): Quantifies the number of AI-adopting firms for different ε values, plotted against simulation iterations.

Notes

The scripts assume a grid size of n=20, evolution threshold p₀=0.6, and 30 simulation steps, as specified in the manuscript.
The von Neumann neighborhood (4 neighbors: north, south, east, west) is used for cell interactions.
Random number generation in MATLAB may produce slightly different initial states for Figure 5 unless a seed is set (not implemented in the provided scripts).
For reproducibility, users can add rng(seed) (e.g., rng(42)) at the start of each script to fix the random number generator state.

Contributing
Contributions to improve the code or extend the simulations are welcome. Please submit a pull request or open an issue to discuss proposed changes.
License
This project is licensed under the MIT License. See the LICENSE file for details.
Contact
For questions or data/code availability requests, please contact the corresponding author
Citation
If you use this code in your research, please cite our manuscript

Acknowledgments
This research was funded by the Major Projects of National Social Science Fund, China (Grant No. 23&ZD090). We thank all co-authors and reviewers for their contributions to the manuscript.
