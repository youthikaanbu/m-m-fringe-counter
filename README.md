# m-m-fringe-counter
photodiode transimpedance amplifier stages for quadrature phase sensing on custom PCB, interfaced with Teensy 4.0 for circular fringe counting data on Michelson-Morely interferometer undergraduate labs

UCSB Physics 128L lab consists of experiments with the Michelson-Morley interferometer by Pasco (https://web.physics.ucsb.edu/~phys128/experiments/interferometry/Precision-Interferometer-Manual-OS-9255A.pdf). 

The helium-neon laser has a wavelength of 632.8 nm...some notes about what is going on in the interferometer and what I am aiming to do. 

## Hardware Notes

Input is output laser light from the interferometer, which would need a photodiode to convert the light into a current. The current is transformed into a readable voltage via transimpedance amplifier and then sent into a AC/DC converter in the Teensy 4.0. This will then count the fringes and display via an OLED screen. 

Photodiode options to test: 

• Advanced Photonix PDB-C139: A standard through-hole PIN photodiode. Its clear plastic T-1 3/4 package allows maximum visible light entry, making it highly responsive to red laser beams. It serves as an excellent low-cost option (~$5) for prototyping. Available on DigiKey.

• Advanced Photonix PDB-C142: Optimized as a blue-enhanced silicon photodiode tailored for high performance across visible wavelengths. It provides excellent, highly predictable linear responsivity right around the 633 nm range. Available on DigiKey.

• Vishay Semiconductor BPV10: A high-speed, high-sensitivity silicon PIN photodiode housed in a 5mm leaded package. If your laser signal is being modulated or pulsed and you need a fast response time without breaking the bank, this sub-$2 part is ideal. Available on DigiKey.

## LT Spice Simulation 
do an LT spice sim for each of the photodiodes 

## Breadboard design 

## KiCad Schematic 

## KiCad PCB Design 

## Soldering the Fringe Counter 

## Software Setup
