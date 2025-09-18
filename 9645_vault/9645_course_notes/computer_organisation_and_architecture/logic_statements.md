
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

## Order of precedence
the order in which you simplify or calculate logic matters, ensure you consider this when calculating an answer or simplifying.

1. Brackets (NOT over multiple operands is like having brackets)
2. NOT
3. AND
4. OR and XOR

remember that in BODMAS, BIDMAS, PEDMAS, PODMAS etc.
**Multiplication** (often represented with a central-dot $\cdot$ ) comes first
**Addition** (often represented by a + plus symbol.) comes after
In logic ANDs are like Multiplication and ORs are like Addition
you can use this to remember that the same rules apply in Logic
think about it in terms of the truth tables:

### AND

| A   | B   | X   | Multiply            |
| --- | --- | --- | ------------------- |
| 0   | 0   | 0   | $0 \cdot 0 = 0$     |
| 0   | 1   | 0   | $0 \cdot 1 = 0$<br> |
| 1   | 0   | 0   | $1 \cdot 0 = 0$<br> |
| 1   | 1   | 1   | $1 \cdot 1 = 1$<br> |
### OR

| A   | B   |  X  |    Add     |
| --- | --- | :-: | :--------: |
| 0   | 0   |  0  | $0+0 = 0$  |
| 0   | 1   |  1  | $0+1 = 1$  |
| 1   | 0   |  1  | $1+0 = 1$  |
| 1   | 1   |  1  | $1+1 = 2$  |
(the last addition is >1 however in logic we consider >1 to be True, this is called [[truthyness]])