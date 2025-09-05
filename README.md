This example shows how to solve the classic Knapsack Problem in Excel using Solver. The goal is to maximize total value while keeping total weight within capacity.

Please Read Steps:
Set Up Data: List items with values, weights, and a row for binary decision variables (0 = not selected, 1 = selected).

Formulas:
Total Value = SUMPRODUCT(Optimal Solution, Values)
Total Weight = SUMPRODUCT(Optimal Solution, Weights)

Enable Solver: File > Options > Add-ins > Solver Add-in.

Solver Setup:
Objective: maximize total value cell.
Variables: decision variable row.
Constraints: total weight ≤ capacity, variables = binary.
Solve: Choose GRG non Linear → Solve.
Result: Solver finds the best combination (e.g., value = 944, weight = 343 ≤ 350).

This method models optimization problems easily in Excel without programming.


