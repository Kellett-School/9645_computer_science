this [[logic_circuits|logic circuit]] can add together **three** binary numbers and returns a remainder if the result is larger than 1 bit. This extends the functionality of the [[half_adder]]

The full adder takes three inputs **Cin** (Standing for **Carry In**), A and B and has two outputs, It's output's names are significant **S** stands for **SUM** as it represents the sum of A and B in binary, **Cout** stands for **CARRY out** as it represents the carry of a binary addition between A and B.
## Logic Circuit
Constructed with two Half adders and an OR gate to OR the carries of the two Half Adders, notice how the sum of one half adder feeds into the sum of the other, now we can sum three binary digits Cin, A and B

### Abstract Representation
The internal configuration of the Full Adder can be [[abstraction|abstracted]] meaning that we do not see it's internals, instead we can represent it as a box labeled as **FA** standing for **Full Adder**

![[Excalidraw/logic_circuit_examples.md#^group=M92-tm04JXQK2QgncSFql|full_adder_abstracted]]

### The Full Logic Circuit
And without the abstraction it looks like this:
![[Excalidraw/logic_circuit_examples.md#^group=afw-KJ8HQjwn-Y7eRVw4C|full_adder_gates]]


## Truth Table

| Cin | **A** | **B** | **Cout** | **S** |
| :-: | :---: | :---: | :------: | :---: |
|  0  |   0   |   0   |    0     |   0   |
|  0  |   0   |   1   |    0     |   1   |
|  0  |   1   |   0   |    0     |   1   |
|  0  |   1   |   1   |    1     |   0   |
|  1  |   0   |   0   |    0     |   1   |
|  1  |   0   |   1   |    1     |   0   |
|  1  |   1   |   0   |    1     |   0   |
|  1  |   1   |   1   |    1     |   1   |
As you can see S contains the **binary sum** of Cin, A and B, Cout contains the **remainder** or **carry** of the **sum** of Cin, A and B. Arranging the Truth Table in the order A,B,C,S shows the binary sum of columns A and B in columns C and S
