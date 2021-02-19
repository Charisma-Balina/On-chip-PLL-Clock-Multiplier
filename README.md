# PLL-Clock-Multiplier
Characterization of 8x PLL Clock Multiplier on Skywater 130nm **sf** process corner at room temperature.

## Phase Locked Loop Block Diagram

<img width="454" alt="pll" src="https://user-images.githubusercontent.com/72096419/108541874-0292b100-7309-11eb-9251-c46aa69c5b5f.PNG">

Cloning the Git Repo https://github.com/lakshmi-sathi/avsdpll_1v8.git

<img width="546" alt="1" src="https://user-images.githubusercontent.com/72096419/108540621-6caa5680-7307-11eb-8ffc-c421e2461c45.PNG">

In the sky130nm.lib file, we can find the library file corresponding to the **tt** corner.\
Change the corner to **sf**.

<img width="548" alt="2" src="https://user-images.githubusercontent.com/72096419/108540889-c448c200-7307-11eb-9ae2-8ac2c1de829f.PNG">
<img width="534" alt="3" src="https://user-images.githubusercontent.com/72096419/108540892-c579ef00-7307-11eb-8c6e-8f5d4ab42b47.PNG">

In the sky130_Primitives file, we can find the corner.spice files of the corresponding corners.

<img width="542" alt="4" src="https://user-images.githubusercontent.com/72096419/108541893-09b9bf00-7309-11eb-9b87-19f00139606a.PNG">
<img width="541" alt="5" src="https://user-images.githubusercontent.com/72096419/108541900-0b838280-7309-11eb-97b2-5c43a67a7947.PNG">

# Pre-Layout Simulations

<img width="540" alt="6" src="https://user-images.githubusercontent.com/72096419/108542535-e2172680-7309-11eb-88f6-2066a3788639.PNG">

Performing the simulations using ngspice.

## Phase Frequency Detector

<img width="472" alt="9 PD cir" src="https://user-images.githubusercontent.com/72096419/108542571-ec392500-7309-11eb-81c5-00d0f981273d.PNG">

<img width="230" alt="9-2 zoom" src="https://user-images.githubusercontent.com/72096419/108542576-ecd1bb80-7309-11eb-9081-0497678455c2.PNG">


## Charge Pump


## Voltage Controlled Oscillator

## Frequency Divider 


