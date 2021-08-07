# Bell-and-GHZ
Implementation of Bell and GHZ states using Qiskit


The famous Bell state is the simplest example of quantum entanglement, where two qubits are intertwined until decoherence separates them. If one is measured as zero, so is the other, if one is measured as 1, so is the other. However, we do not know which of the states will be measured.
The circuit to create the Bell state (|00> + |11>)/sqr(2) is shown below. It uses only a Hadamard and a controlled X.

![](https://miro.medium.com/max/1400/0*wFUwF4KjbQmOXcay)

The GHZ state is similar, for three qubits: (|000> + |111>)/sqr(2). In terms of circuit, it has one more qubit, and one more CX.

![](https://miro.medium.com/max/2400/0*89N0OUgXPdd4nfeg)


(See https://en.wikipedia.org/wiki/Greenberger%E2%80%93Horne%E2%80%93Zeilinger_state )


And to do the same thing but with 4 qubits? We want to arrive at (|0000> + |1111>)/sqr(2) — that is, if one of the qubits is drawn as zero, all the others will also be drawn.
By the pattern above, just add one more CX between the last previous qubit and the new qubit.

![](https://miro.medium.com/max/677/0*KTgYPiecHkpEwpzn)


Then, to generalize, just add a loop.


![](https://miro.medium.com/max/2400/0*WtacgYsaNcqLBhbc)

