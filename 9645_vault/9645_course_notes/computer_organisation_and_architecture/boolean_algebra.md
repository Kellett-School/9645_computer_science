Algebra for logic, boolean algebra is used to check that circuits are equivalent or simplify circuits. 

## Rules or Laws
There are several laws of boolean algebra that you should memorize for your examinations, however many of these laws are quite intuative if you think about them.

**P.S.** You **do not** need to memorize the names of the laws

Drawing out the law as a logic circuits or comparing truth tables of some of these helps with understanding.

|     Name     |                      And form                       |                       Or form                       |
| :----------: | :-------------------------------------------------: | :-------------------------------------------------: |
|   Identity   |                   $1 \cdot A = A$                   |                     $0 + A = A$                     |
|     Null     |                   $0 \cdot A = 0$                   |                     $1 + A = 1$                     |
|  Idempotent  |                   $A \cdot A = A$                   |                     $A + A = A$                     |
|   Inverse    |              $A \cdot \overline A = 0$              |                $A + \overline A = 1$                |
| Commutative  |               $A \cdot B = B \cdot A$               |                   $A + B = B + A$                   |
| Associative  |     $A \cdot (B \cdot C) = (A \cdot B) \cdot C$     |             $A + (B + C) = (A + B) + C$             |
| Distributive |       $A + B \cdot C = (A + B) \cdot (A + C)$       |      $A \cdot (B + C) = A \cdot B + A \cdot C$      |
|  Absorption  |                $A \cdot (A + B) = A$                |                 $A + A \cdot B = A$                 |
| De Morgan's  | $\overline {A \cdot B} = \overline A + \overline B$ | $\overline {A + B} = \overline A \cdot \overline B$ |

## Intuitive Laws
Most of the laws above are pretty intuitive, and can be figured out in an exam if you've forgotten, just try drawing them as [[logic_circuits]] and follow them through with the inputs and outputs, OR try writing out the truth tables (don't rely on this, it's better to just memorize them)

For example, the identity laws:

|                                                                 And form                                                                  |                                                                  Or form                                                                  |
| :---------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------: |
|                                                              $1 \cdot A = A$                                                              |                                                                $0 + A = A$                                                                |
|                           ![[Excalidraw/logic_circuit_examples.md#^group=iNbTgqzjZUZOf2a_rjP_c\|identity_and]]                            |                            ![[Excalidraw/logic_circuit_examples.md#^group=2fIP7ieuicTjIrSOAFXge\|identity_or]]                            |
| if the input A is 1 the output is going to be 1, if the input A is 0 then the output is going to be 0, that's the same as just A (a wire) | if the input A is 1 the output is going to be 1, if the input A is 0 then the output is going to be 0, that's the same as just A (a wire) |

For example, the Absorption law:

| And form                                                                                                                                                                                                                                                                       | Or form                                                                                                                                                                                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| $A \cdot (A + B) = A$                                                                                                                                                                                                                                                          | $A + A \cdot B = A$                                                                                                                                                                                                                                                             |
| ![[Excalidraw/logic_circuit_examples.md#^group=mVdto-dQpXLIZqZfWwXPy\|absorption_and]]                                                                                                                                                                                         | ![[Excalidraw/logic_circuit_examples.md#^group=Ewq9ysFyc00eWoRaZSBkN\|absorption_or]]                                                                                                                                                                                           |
| if A is 1 then the AND will have an input of 1, therefore we need to check the output of the OR, but the OR must output 1 because one of it's inputs is a 1, it doesn't matter what B is. if A is 0 then we don't even need to check the other input, the output has to be a 0 | if A is 0 then the OR will have an input of 0, therefore we need to check the output of the AND, but the AND must output 0 because one of it's inputs is a 0, it doesn't matter what B is. if A is 1 then we don't even need to check the other input, the output has to be a 1 |

## Applying the laws step by step
Boolean Algebra questions come in two 'flavours' in the exam, 'show that' and 'simplify'

**Show that** will have an equals symbol with two logic statements either side, it's your job to use boolean algebra to prove that one statement is the same as the other

**Simplify** expects you to use the laws to find the most simple possible configuration of logic.

in both cases you **must show your working out** because this is where you gain marks, and interestingly you are marked line by line **until you make a mistake** therefore you need to make sure that you show all steps and that you check that you're right on each step.

**N.B.** you **do not** need to name the steps, but you **must** show each step.

### Examples:

#### Question:
Simplify $X = \overline {A \cdot B + A} + B \cdot \overline A + A$
#### Working out:
$$\displaylines{
X = \overline {A \cdot B + A} + B \cdot \overline A + A\\
X = \overline {A} + B \cdot \overline A + A\\
X = \overline {A} + A\\
X = 1
}$$
1. OR form of absorption applied
2. OR form of absorption applied
3. OR form of inverse applied


#### Question:
Simplify $X = \overline A + B + B \cdot (A + \overline B)$
#### Working out:
$$\displaylines{
X = \overline A + B + B \cdot (A + \overline B)\\
X = \overline A + B +  B \cdot A + B \cdot \overline B\\
X = \overline A + B +  B \cdot A + 0\\
X = \overline A + B +  B \cdot A \\
X = \overline A + B \\
}$$
1. OR form of distributive applied
2. AND form of inverse applied
3. And form of identity applied
4. Or Form of Absorption applied

