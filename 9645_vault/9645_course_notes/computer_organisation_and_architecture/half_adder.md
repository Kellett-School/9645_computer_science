this [[logic_circuits|logic circuit]] can add together two binary numbers and returns a remainder if the result is larger than 1 bit.

The half adder takes two inputs A and B and has two outputs, It's output's names are significant **S** stands for **SUM** as it represents the sum of A and B in binary, **C** stands for **CARRY** as it represents the carry of a binary addition between A and B.

Two half adders can be combined to make a [[full_adder]]
## Logic Circuit
![[Excalidraw/logic_circuit_examples.md#^group=p4AoQJ7GMmAcCEtIWKjl6|half_adder]]

## Abstract Representation
The internal configuration of the Half Adder can be [[abstraction|abstracted]] meaning that we do not see it's internals, instead we can represent it as a box labeled as **HA** standing for **Half Adder**
![[Excalidraw/logic_circuit_examples.md#^group=GuwwqFP4CX5z4k10NsI3O|half_adder_abstract]]
## Truth Table

| **A** | **B** | **C** | **S** |
| :---: | :---: | :---: | :---: |
|   0   |   0   |   0   |   0   |
|   0   |   1   |   0   |   1   |
|   1   |   0   |   0   |   1   |
|   1   |   1   |   1   |   0   |
As you can see S contains the **sum** of A and B, C contains the **remainder** or **carry** of the **sum** of A and B. Arranging the Truth Table in the order A,B,C,S shows the binary sum of columns A and B in columns C and S
