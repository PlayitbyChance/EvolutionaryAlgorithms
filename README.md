# EvolutionaryAlgorithms

An evolutionary algorithm is implemented and explored in this project. As a test case, the travelling salesman problem is used, as follows: given a list of cities, what is the minimal distance path the salesman can take while visiting each city once?

This problem has no known polynomial time solution which makes is scale fairly poorly when the number of cities grows large. A simple search algorithm (with some dynamic programming to bring it down from factorial time to exponential time) is given to demonstrate the exact solution approach. This is used as a baseline for comparing to the evolutionary algorithm. 

Using an evolutionary algorithm, resulting solutions are generally reasonably close to the optimal while being much faster at higher numbers of cities. For example, in one test using 20 cities, the exact solution took 122 seconds to compute while the evolutionary algorithm approach took 2 seconds and was within 7% of the optimal solution. Furthermore, the exact solution approach was limited to under 30 cities (primarily due to memory restrictions) while the evolutionary algorithm could be used a much higher number of cities (12 minutes for 1000 cities). 
