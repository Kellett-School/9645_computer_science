A D Type Flip Flop is just an SR Flip Flop that cannot get itself into an invalid state, this is achieved simply by attaching set and reset to the same line (data line) and inverting the input for reset.

Therefore the D Type can never have set and reset be $1$ $1$ or $0$ $0$.

The D Type also extends the **Enable** line by commonly adding a [[rising_edge_pulse_detector]]

## Logic Circuit
![[Excalidraw/logic_circuit_examples.md#^group=zu8osHV3BQAEexwjD6fOC|d_type_flip_flop]]
## Truth Table

| E (CLK) | $D$ | $Q_{n+1}$ | $\overline Q_{n+1}$ |       State       |
| :-----: | :-: | :-------: | :-----------------: | :---------------: |
|  1 (▲)  |  0  |     0     |          1          |       Reset       |
|  1 (▲)  |  1  |     1     |          0          |        Set        |
|    0    |  ?  |   $Q_n$   |   $\overline Q_n$   | Store (No Change) |
