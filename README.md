# PLL-Clock-Multiplier
Characterization of 8x PLL Clock Multiplier on Skywater 130nm **sf** process corner at room temperature.

## Phase Locked Loop Block Diagram

The phase-locked loop (PLL) block is a feedback control system that automatically adjusts the phase of a locally generated signal to match the phase of an input signal. They are used to create stable system clocks in microprocessors.

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

Performing the simulations using ngspice at temperature T=27C

## Phase Frequency Detector

Command: ngspice PD.cir

<img width="472" alt="9 PD cir" src="https://user-images.githubusercontent.com/72096419/108542571-ec392500-7309-11eb-81c5-00d0f981273d.PNG">

<img width="481" alt="9-1" src="https://user-images.githubusercontent.com/72096419/109003004-e8701e80-76cc-11eb-98ce-2df02267c7f6.PNG">


**Blue** = Clock 1\
**Red**  = Clock 2\
**Orange** = UP Signal\
**Green**  = DOWN Signal

## Charge Pump

Command: ngspice CP.cir

<img width="469" alt="8 CP cir" src="https://user-images.githubusercontent.com/72096419/108542610-f5c28d00-7309-11eb-8bed-e4b279c3425e.PNG">

**Red** = Charge Pump Output Voltage

## Voltage Controlled Oscillator

Command: ngspice VCO.cir

<img width="483" alt="10 VCO cir" src="https://user-images.githubusercontent.com/72096419/109002205-e8bbea00-76cb-11eb-9ad8-199849386c37.PNG">

**Red**  = Input\
**Blue** = Output

## Frequency Divider 

Command: ngspice FD.cir

<img width="472" alt="7 FD cir" src="https://user-images.githubusercontent.com/72096419/108542654-0541d600-730a-11eb-80de-e95f050caf07.PNG">

**Blue** = Input Clock\
**Red**  = Output Clock

## PLL OUTPUT

Command: ngspice PLL_PreLay.cir

![0](https://user-images.githubusercontent.com/72096419/110016857-8908b300-7d4b-11eb-9ff3-8c7627d728a2.png)

Changing the transient time values

180us to 450us


### Output








