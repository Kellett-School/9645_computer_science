Logic gates are used to evaluate logical operations between one or two operands, there are 6 gates you should be aware of:

## AND

### Symbol
[link to image](https://www.basictables.com/media/and-gate-icon.png)
### Notation
∧ or ·
### Truth Table

| **A** | **B** | **X** |
| ----- | ----- | ----- |
| 0     | 0     | 0     |
| 0     | 1     | 0     |
| 1     | 0     | 0     |
| 1     | 1     | 1     |

## OR

### Symbol
[link to image](https://www.basictables.com/media/or-gate-icon.png)
### Notation
∨ or +
### Truth Table

| **A** | **B** | **X** |     |
| ----- | ----- | ----- | --- |
| 0     | 0     | 0     |     |
| 0     | 1     | 1     |     |
| 1     | 0     | 1     |     |
| 1     | 1     | 1     |     |

## NOT

### Symbol
[link to image](https://www.basictables.com/media/not-gate-icon.png)
### Notation
¬ or ‾
### Truth Table

| **A** | **X** |     |
| ----- | ----- | --- |
| 0     | 1     |     |
| 1     | 0     |     |

## XOR
### Symbol
[link to image](https://www.basictables.com/media/xor-gate-icon.png)
### Notation
⊻ or ⊕
### Truth Table

| **A** | **B** | **X** |     |
| ----- | ----- | ----- | --- |
| 0     | 0     | 0     |     |
| 0     | 1     | 1     |     |
| 1     | 0     | 1     |     |
| 1     | 1     | 0     |     |

## NAND
### Symbol
[link to image](https://www.basictables.com/media/nand-gate-icon.png)
### Notation
⊼ or $X=\overline{A \cdot B}$
### Truth Table

| **A** | **B** | **X** |
| ----- | ----- | ----- |
| 0     | 0     | 1     |
| 0     | 1     | 1     |
| 1     | 0     | 1     |
| 1     | 1     | 0     |

## NOR
### Symbol
[link to image](https://www.basictables.com/media/nor-gate-icon.png)
### Notation
⊽ or $X=\overline{A + B}$
### Truth Table

| **A** | **B** | **X** |
| ----- | ----- | ----- |
| 0     | 0     | 1     |
| 0     | 1     | 0     |
| 1     | 0     | 0     |
| 1     | 1     | 0     |

## Logic Statements

This is an example of a logic statement:
$$X=\overline{A \cdot B} + B \cdot \overline A$$
These require some inputs to be solved (find the value of X)
for example if the inputs were:
$$A=0, B=1$$
then the answer would be:
$$\displaylines{
X = \overline {0 \cdot 1} + 1 \cdot \overline 0 \\
X = \overline 0 + 1 \cdot 1 \\
X = 1 + 1 \\
X = 1
}$$
This process of simplification is called [[boolean_algebra|boolean algebra]]
