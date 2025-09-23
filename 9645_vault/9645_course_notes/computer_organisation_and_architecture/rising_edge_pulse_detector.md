#notinsyllabus 
A Rising Edge Pulse is when a signal goes from low to high, the point at which this happens is called a rising edge.

A rising edge is represented using the symbol ▲

How do we send a brief pulse if we detect a rising edge for instance, it's actually really simple and is possible because it takes a small amount of time for a current to pass through several gates.

![[Excalidraw/logic_circuit_examples.md#^group=SjTee69y|rising_edge_detector]]

```wavedrom
{ signal: [
  { name:"In", fill:"white", wave:'l.h..l.....'},
  { name:"Delayed In", fill:"white", wave:'h..l..h....'},
  { name:"Out", fill:"white", wave:'l.hl.......'},
], config: {hscale: 2, skin: 'narrow'} }
```

Here you can see that when *IN* is low, that Delayed In is high, if *IN* goes high then it takes a short while for *Delayed IN* to go low, during this time both inputs *IN* and *Delayed IN* to an AND gate are high, and therefore the output is high for this time. Once the current 'catches up' and the *Delayed IN* goes low, then both inputs are no longer high and so the and gate's input now dips to low.

You can see this effect on the timing graph above (light mode)