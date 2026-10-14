# m-m-fringe-counter
photodiode transimpedance amplifier stages for quadrature phase sensing on custom PCB, interfaced with Teensy 4.0 for circular fringe counting data on Michelson-Morely interferometer undergraduate labs

UCSB Physics 128L lab consists of experiments with the Michelson-Morley interferometer by Pasco (https://web.physics.ucsb.edu/~phys128/experiments/interferometry/Precision-Interferometer-Manual-OS-9255A.pdf). 

The helium-neon laser has a wavelength of 632.8 nm...some notes about what is going on in the interferometer and what I am aiming to do. 

## Fringe Counter Circuit Design

Input is output laser light from the interferometer, which would need a photodiode to convert the light into a current. The current is transformed into a readable voltage via transimpedance amplifier and then sent into a AC/DC converter in the Teensy 4.0. This will then count the fringes and display via an OLED screen. 
