# Quantum_Computing_with_Qiskit
A collection of quantum computing exercises for coding in IBM's Qiskit platform.

#### Exercise 1:

IBM Q Experience (https://quantum-computing.ibm.com) is a quantum cloud service and software plat-
form, which allows users to run experiments even on real quantum computing hardware. For this exercise you
should create a personal account and familiarize yourself with the service.
IBM Q offers a graphical Circuit Composer and Qiskit Notebooks as interface, which are Jupyter Python
notebooks using the Qiskit open-source framework (https://qiskit.org). Both can be conveniently accessed
online via a web browser; alternatively, you can also install Qiskit locally via pip install qiskit. An
introduction to Qiskit is available at 
https://qiskit.org/documentation/tutorials/fundamentals/1_
getting_started_with_qiskit.html.

(a) Use the Circuit Composer to construct the quantum entanglement circuit together with measure-
ment operations:
Note that the Circuit Composer stores the measurement results in a classical register. You can view the
corresponding OPENQASM code in the Circuit editor. Now run your circuit using 1024 \shots" (repetitions)
to collect a statistical distribution of measurements.

(b) Construct the circuit again using Qiskit, and execute the circuit via Aer's qasm simulator (1024 shots as
above).

#### Exercise 2:

(a) By the principle of deferred measurement, measurement operations can always be moved to the end of the
circuit, and classically controlled operations by conditional quantum operations. Verify this statement for the
following controlled-U circuit, by inserting a random qubit and computing the intermediate states.

(b) For the purpose of simulating the quantum teleportation circuit, we can exploit the principle of deferred
measurement to omit the measurements altogether. Construct the circuit in the IBM Q Circuit Composer. 
Insert a rotation operation at the beginning to prepare the initial qubit rotated in y-axis by π/3.
  
#### Exercise 3:

Implement the partial trace operation for arbitrary dimensions using Python/NumPy. Specifically, you should
write a function with signature partial_trace(rho, dimA, dimB), where rho is the density matrix of the
composite quantum system, and dimA, dimB specify the dimensions of subsystems A and B, respectively. (Thus
rho is a dimA · dimB×dimA · dimB matrix.) The function should return a tuple (ρ^A, ρ^B) containing the reduced
density matrices ρ^A = trB[rho] and ρ^B = trA[rho].

(b) Apply your function to the density operator with the given Bell state.

(c) Test your implementation by constructing a random density matrix ρ on the composite system and a random
observable M on subsystem A, and then numerically verifying that tr[M ρA] = tr[(M ⊗ I)ρ] (up to numerical
rounding errors).

#### Exercise 4: 
Three-qubit quantum Fourier Transform.

#### Exercise 5:
Reduction of factoring to order-finding.
