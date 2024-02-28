# Grover's-Quantum-Search-Algorithm

Project Overview:
This repository hosts the implementation of the Grover Search algorithm, a quintessential quantum algorithm known for its ability to perform database searches with quadratic speedups over classical counterparts. Developed for the CMPE-789 Quantum Computing course, this project leverages IBM's Qiskit environment to construct and simulate Grover's algorithm on both 2-qubit and 3-qubit systems, with an extension to a 4-qubit system.

Grover's Algorithm:
Grover's algorithm stands as a monumental achievement in the field of quantum computing, showcasing a remarkable ability to outperform classical search methodologies. At its core, Grover's algorithm is designed to efficiently search through unsorted databases, accomplishing tasks with quadratic speedup compared to the best possible classical algorithms. This quantum algorithm, developed by Lov Grover in 1996, has not only solidified its place as a cornerstone in quantum computing but also serves as a clear demonstration of quantum advantage for specific computational problems.

The elegance of Grover's algorithm lies in its utilization of the fundamental principles of quantum mechanics, such as superposition, entanglement, and interference, to amplify the probability amplitude of the desired state, thereby significantly reducing the number of operations needed to find the target item. Unlike classical search algorithms that require a linear increase in operations with the size of the database, Grover's algorithm achieves its task in approximately the square root of the number of operations required by classical counterparts.

Grover's algorithm is structured around two key quantum operations: the oracle and the diffusion operator. The oracle is a quantum gate that inverses the phase of the state corresponding to the target item, effectively marking it within the quantum superposition of all possible states. The diffusion operator, often described as a form of quantum interference, then amplifies the probability amplitude of the marked state while de-amplifying the others, bringing the quantum system closer to the target state with each iteration. Remarkably, after a specific number of iterations—proportional to the square root of the database's size—the algorithm ensures that the measurement of the quantum system will yield the target state with high probability.

The implications of Grover's algorithm extend far beyond mere database searching. It has laid the groundwork for the development of more sophisticated quantum algorithms and has applications in solving a wide array of problems, including cryptography, optimization, and pattern recognition, where it can offer substantial computational speedups. Additionally, Grover's algorithm serves as a vital benchmark for demonstrating the capabilities of quantum processors, pushing the boundaries of what is computationally feasible and guiding the ongoing evolution of quantum computing technology.

Features:

1. 2-Qubit Grover Search: Implementation of Grover's algorithm to search a database of four elements, demonstrating the algorithm's ability to find a marked item with a single query.
2. 3-Qubit Grover Search: Extension of the Grover Search to a 3-qubit system, enabling the search within an eight-element database. This section includes the implementation of custom oracles and diffusion operators, along with adjustments in the number of iterations to optimize for the increased system size.
3. 4-Qubit Grover Search (Extra Credit): An advanced implementation that extends the Grover Search to a 16-element database, showcasing the scalability of the algorithm and the use of Qiskit's tools to manage more complex quantum systems.
4. Custom Oracles: Development of specific oracles for targeting different states within the quantum database, each accompanied by detailed linear algebra proofs and Qiskit circuit implementations.
5. Optimization Techniques: Insights into the optimization of the Grover iteration count based on the system size, including a discussion on finding the ideal number of iterations to maximize the probability of measuring the target state.
