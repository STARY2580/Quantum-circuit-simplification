# Quantum-circuit-simplification  
(1) Quantum circuits can be simplified, rules can be added independently, and five rules are already built-in.
(2) The five rules are: 1. The initial CNOT gate can be removed; 2. The initial Rz gate can be removed; 3. One of two consecutive CNOT gates can be removed; 4. Two identical rotation gates can be merged with their phases added together; 5. More than three single-qubit gates can be represented by a universal U gate.
(3) There is also a swap rule: Rz can swap positions with the control bit of the CNOT gate, and Rx can swap positions with the target bit of the CNOT gate.
(4) The input quantum currently only supports Rz, Rx, and CNOT gates. The input circuit format follows the example: [('rx', 0), ('rz', 1), ('cx', 0, 1)] in list form, and the parameters are also input in the order of the list of quantum gates. The CNOT gate has no parameters, so the parameter list has fewer items than the structure list by the total number of CNOT gates.
