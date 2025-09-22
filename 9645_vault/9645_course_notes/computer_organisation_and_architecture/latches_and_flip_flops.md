## Types of Latch & Flip Flop
[[sr_flip_flop]]
[[d_type_flip_flop]]
## What's the difference between a 'latch' and a 'flip flop'
You may hear the term **Latch** or you may hear the term **flip flop** these are different, latches are the pure logic circuit that actually stores information, the flip flop adds additional control circuits to manage the circumstances in which the latch changes state, see the differences below in the Logic Circuit diagrams

## Active High vs Active Low
You may also hear the terms **Active High** or **Active Low** this refers to if the gate is activated when it receives a **high** or a **low** signal (High being 5v or 3.3v usually, low being 0v or close to that.)

in an **Active High** latch when the Set (S) is high (1) Q will be set High (1)
in an **Active Low** latch when the Set (S) is low (0) Q will be set High (1) 
N.B. *See this effect in the Truth Tables below*

## Rising edge and Falling Edge
You may see the term Rising Edge or Falling Edge when talking about flipflops or latches, these terms stand for:
**Rising Edge**: A brief control voltage pulse sent when a signal goes from low to high
**Rising Edge**: A brief control voltage pulse sent when a signal goes from High to Low

For Rising Edges we use this symbol ▲
For Falling Edges we use this symbol ▼

#### Logic Circuit for Rising or falling edges. 
#notinsyllabus
How do we send a brief pulse if we detect a rising edge for instance, it's actually really simple and is possible because it takes a small amount of time for energy to pass through gates.
![[Excalidraw/logic_circuit_examples.md#^group=SjTee69y|rising_edge_detector]]

```wavedrom
{ signal: [
  { name:"In", fill:"white", wave:'l.h..l.....'},
  { name:"Delayed In", fill:"white", wave:'h..l..h....'},
  { name:"Out", fill:"white", wave:'l.hl.......'},
], config: {hscale: 2, skin: 'narrow'} }
```
