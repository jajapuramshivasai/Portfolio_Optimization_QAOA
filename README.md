# Portfolio_Optimization_QAOA

## Overview
This project is a prototype for solving a binary portfolio optimization via quantum algorithms (QAOA) .

## Approach
1. Formulate portfolio selection as a binary quadratic problem with linear constraints.  
2. Convert constrained model into an unconstrained QUBO (penalty method).  
3. Implement QAOA in PennyLane to minimize the QUBO cost Hamiltonian.  
4. Validate and benchmark with a classical heuristic (greedy + random sampling).  
5. Analyze solution quality, convergence, and scaling.

## Task Breakdown
1. Review mathematical formulation:  
   - Binary decision variables, linear constraints, quadratic objective.  
2. QUBO conversion:  
   - Embed constraints into a single unconstrained binary objective.  
3. Quantum solver implementation:  
   - Develop QAOA (or alternative VQE) routine to solve general QUBOs.  
4. Quantum solution:  
   - Apply the quantum solver to the portfolio problem.  
5. Classical validation:  
   - Solve the same instance classically for comparison.  
6. Comparison & metrics:  
   - Compare objective values, convergence curves, and runtime scaling.

## Usage
```bash
git clone https://github.com/jajapuramshivasai/Portfolio_Optimization_QAOA.git
cd Portfolio_Optimization_QAOA
pip install -r requirements.txt
jupyter notebook portfolio_optimization.ipynb
