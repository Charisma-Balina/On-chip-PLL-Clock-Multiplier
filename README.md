# PLL-Clock-Multiplier
Characterization of 8x PLL Clock Multiplier on Skywater 130nm **sf** process corner at room temperature.\

## Phase Locked Loop Block Diagram

Cloning the Git Repo https://github.com/lakshmi-sathi/avsdpll_1v8.git

<img width="546" alt="1" src="https://user-images.githubusercontent.com/72096419/108540621-6caa5680-7307-11eb-8ffc-c421e2461c45.PNG">

In the sky130nm.lib file, we can find the library file corresponding to the **tt** corner.\
Change the corner to **sf**.

<img width="548" alt="2" src="https://user-images.githubusercontent.com/72096419/108540889-c448c200-7307-11eb-9ae2-8ac2c1de829f.PNG">
<img width="534" alt="3" src="https://user-images.githubusercontent.com/72096419/108540892-c579ef00-7307-11eb-8c6e-8f5d4ab42b47.PNG">

In the sky130_Primitives file, we can find the corner.spice files of the corresponding corners.

