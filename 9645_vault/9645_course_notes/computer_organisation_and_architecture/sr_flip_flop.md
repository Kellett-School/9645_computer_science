**N.B.** #notinsyllabus
The SR flip flop is not included in the 9645 syllabus, however it's a crucial building block of the [[d_type_flip_flop]] which is in the syllabus, therefore it's worth knowing about. Please be aware that you will not need to memorize any of this.

The SR flip flop is a very simple way to arrange logic gates to create a simple block of [[memory]]. However the SR flip flop has issues, for instance it can get into an **indeterminate state** where $Q$ and $\overline Q$ are the same, this should not be able to happen.

## Logic Circuits and Truth Tables

### SR Latch (NAND version) (Active Low)
![[Excalidraw/logic_circuit_examples.md#^group=4-wbYttAFxTg9Q3H7GKI4|sr_latch_nand]]

| $\overline S$ | $\overline R$ | $Q_{n+1}$ | $\overline Q_{n+1}$ |       State       |     |
| :-----------: | :-----------: | :-------: | :-----------------: | :---------------: | --- |
|       0       |       0       |     ?     |          ?          |   Indeterminate   |     |
|       0       |       1       |     1     |          0          |        Set        |     |
|       1       |       0       |     0     |          1          |       Reset       |     |
|       1       |       1       |   $Q_n$   |   $\overline Q_n$   | Store (No Change) |     |
### SR (RS) Latch (NOR version) (Active High)
![[Excalidraw/logic_circuit_examples.md#^group=71XLrao8CQdaU-9rzZwSO|sr_latch_nor]]

| $R$ | $S$ | $Q_{n+1}$ | $\overline Q_{n+1}$ |     State     |
| :-: | :-: | :-------: | :-----------------: | :-----------: |
|  0  |  0  |   $Q_n$   |   $\overline Q_n$   |     Store     |
|  0  |  1  |     1     |          0          |      Set      |
|  1  |  0  |     0     |          1          |     Reset     |
|  1  |  1  |     ?     |          ?          | Indeterminate |
### SR Flip Flop (NAND Version) (Active High)
![[Excalidraw/logic_circuit_examples.md#^group=H8byqv5d0MF8Lxo4ZhdxW|sr_flip_flop]]

| E (CLK) | $R$ | $S$ | $Q_{n+1}$ | $\overline Q_{n+1}$ |       State       |
| :-----: | :-: | :-: | :-------: | :-----------------: | :---------------: |
|  1 (▲)  |  0  |  0  |   $Q_n$   |   $\overline Q_n$   | Store (No Change) |
|  1 (▲)  |  0  |  1  |     1     |          0          |        Set        |
|  1 (▲)  |  1  |  0  |     0     |          1          |       Reset       |
|  1 (▲)  |  1  |  1  |     ?     |          ?          |   Indeterminate   |
|    0    |  ?  |  ?  |   $Q_n$   |   $\overline Q_n$   |     No Change     |
