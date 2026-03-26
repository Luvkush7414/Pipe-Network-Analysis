# Pipe-Network-Analysis
A Python algorithm to compute discharge in a 20-pipe hydraulic network using the Hardy Cross method, featuring automated loop detection via spanning trees.
HARDY CROSS PIPE NETWORK PROBLEM SOLVER
Overview:- This repository contains a Python-based computational algorithm developed to analyze flow distribution in a 20-pipe hydraulic network using the Hardy Cross method. The program automates the iterative process of balancing heads, strictly satisfying mass balance and energy conservation laws with a convergence precision of 0.001.
Project Details:- 
Author: Lovekush Meena
Roll Number: 23CE10030 
Course: WATER RESOURCES AND GEOTECHNICAL ENGINEERING SESSIONAL - CE39204
Technical Features & MethodologyThe script is designed to handle complex network topologies by dynamically building the system parameters and automatically identifying loops.Initial Flow Assignment: The algorithm uses a Breadth-First Search (BFS) to automatically find a path from the source node (A) to the exit node (G) to assign the specific inflow value of 144.0 m^{3}/s$\ and satisfy Continuity.Spanning Tree & Loop Detection: Instead of manual loop entry, the program uses Spanning Tree logic to find fundamental loops automatically. Any pipe not included in the spanning tree acts as a chord that closes one of the 14 fundamental loops.Resistance Calculation: Computes resistance (R) dynamically using the pipe length, diameter, and friction factor.Automated Solver: Iteratively calculates the required flow correction (\Delta Q) across all loops until the maximum correction is less than the 0.001 error limit.
Results:-
The algorithm successfully resolved the complex network topology, converging in exactly 57 iterations. The final output generates a comprehensive table detailing the finalized flow magnitudes and directions for all 20 branches of the system.
Academic Context & Literature:- This computational implementation bridges the gap between classic hydraulic theory and digital application. It builds upon the foundational "balancing of heads" method proposed by Hardy Cross in 1936, utilizing modern Python automation to eliminate human error and handle the intensive iterative load required for high-precision water resources engineering.
