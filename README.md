# Quantum Many-Body Spin Systems using Variational Quantum Eigensolver (VQE)

## Overview

This project studies the ground state properties and quantum correlations in a one-dimensional spin system using variational quantum algorithms. In particular, we analyze the **Transverse Field Ising Model (TFIM)** and investigate signatures of quantum phase transitions using the Variational Quantum Eigensolver (VQE).

The goal is to demonstrate how near-term quantum algorithms can be used to extract physically meaningful properties of quantum many-body systems.
## Physical Model
We consider the Transverse Field Ising Model (TFIM), described by the Hamiltonian:
H = -J Σ σᶻᵢ σᶻᵢ₊₁ - h Σ σˣᵢ
where:
- J is the interaction strength between neighboring spins  
- h is the transverse magnetic field  
- σᶻ and σˣ are Pauli matrices  
This model exhibits a **quantum phase transition** at:
h ≈ J
- For h < J → ordered phase  
- For h > J → disordered phase  
## Methodology
We use the **Variational Quantum Eigensolver (VQE)** to approximate the ground state of the system.
Additional methods explored for excited state of the system:
- VQD (Variational Quantum Deflation)
- SSVQE
- QSE (Quantum Subspace Expansion)
## Results
### 1. Ground State Energy vs Transverse Field
- The ground state energy varies smoothly with the field strength h
- The behavior changes near the critical region (h ≈ 1)
### 2. Excietd State Energy vs Transverse Field
- VQD,the curve isn't even linear
- SSVQE,the curve is linear and smooth but not close with the correct values
- QSE,give smooth and most accurate with correct values
### 2. Entanglement Entropy vs Transverse Field
- Entanglement entropy increases near the critical point
- A peak in entropy is observed around h ≈ 1
- This indicates strong quantum correlations at the phase transition
## Physical Interpretation
The peak in entanglement entropy near h ≈ 1 is a signature of a **quantum phase transition** in the system. At this point, the system undergoes a transition between ordered and disordered phases, leading to enhanced quantum correlations.
The VQE algorithm successfully captures this qualitative behavior, demonstrating its capability to study many-body quantum systems even with approximate methods.
## Key Insights
- VQE can approximate ground state properties of many-body systems
- QSE has provided better results for excited state than 
- Entanglement entropy serves as a strong indicator of critical behavior  
- Quantum phase transitions can be detected using variational methods  
## Tools and Technologies
- Python  
- Qiskit  
- NumPy  
- Matplotlib  
## Future Work
- Study larger system sizes and scaling behavior  
- Improve ansatz design for better accuracy  
- Analyze energy gap and correlation functions  
- Extend to other quantum many-body models  
## Conclusion
This project demonstrates how hybrid quantum-classical algorithms like VQE can be used to study fundamental phenomena in quantum many-body physics, including quantum phase transitions and entanglement structure.
## Author

Dheena Dhayalan  
Undergraduate Physics Student  
