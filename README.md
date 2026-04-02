Design




# Journal

## 4/2/2026 - finish off the project

### CAD
Firstly, to finish off the project, I finished the CAD model. I designed it in a way that it can be attached to a microphone arm that I will talk about later

![image](https://stasis.hackclub-assets.com/images/1775130097189-0qdjjv.png)


###  Microphone arm
I decided to get a plug-and-play microphone arm, as designing one to be 3D printed will be near impossible the axial forces might break the plastic parts and the shock absorbion might not be as good.

![image](https://stasis.hackclub-assets.com/images/1775130295043-6diobc.png)

## 4/1/2026  Rerouted the pcb


![image](https://stasis.hackclub-assets.com/images/1775078755625-bjpzzh.png)
I changed the order in which the pins are connected to the aux port to follow the standard pinout sound cards use. This will make my microphone compatible with most sound cards. This change also makes routing easier.

![image](https://stasis.hackclub-assets.com/images/1775078783777-st621v.png)
Rerouted the PCB so that connections are more direct and follow straight lines. This should improve the signal quality slightly

## 4/1/2026 - Picked out components for the mic and modified the CAD drawing


![image](https://stasis.hackclub-assets.com/images/1775053274756-niejdc.png)

![image](https://stasis.hackclub-assets.com/images/1775053516647-crvrvr.png)

edit: I realised I don't need the USB-C to USB-C converter or USB-C to aux 3.5mm as most audio cards will solve all of my issues, I also realised the some audio cards have power delivery through the aux cable. this will mean I will be unable to add an external volume knob, however that is ok because the project complexity will be much lower

## 4/1/2026 - Designed the microphone shell

![image](https://stasis.hackclub-assets.com/images/1775050706255-04zjp5.png)

![image](https://stasis.hackclub-assets.com/images/1775050722339-qj8pqq.png)

![image](https://stasis.hackclub-assets.com/images/1775050737996-ul1eby.png)

I imported the PCB I designed into onshape and used the dimentions on the microphone capsules to design a shell for the microphone, The hollow inside will be filled with foam to prevent unwanted resonances. 

### key features

- a aux hole at the back. While this wont use the aux port as intended; it will deliver power and carry the audio sygnal
- a TPU microphone capsule holder to prevent unwanted vibrations
- a semi hollow front to keep a foam from rigid while allowing sound to pass through

## 4/1/2026 - Microphone PCB

![image](https://stasis.hackclub-assets.com/images/1775037161850-poms1c.png)


![image](https://stasis.hackclub-assets.com/images/1775037177565-wma784.png)

I designed the PCB I mentioned in the previous journal entry, except for a new resistor and capacitor, and a few value changes

### Updated schematic

![image](https://stasis.hackclub-assets.com/images/1775037281832-19hl4k.png)

## 4/1/2026 - Microphone chematic

![image](https://stasis.hackclub-assets.com/images/1775034137213-tvm2x9.png)


I made a simple schematic that repurposes an aux cable to a power delivery and audio carrying cable.
I will design another PCB that can deliver the 5V and recieve audio. then it will regulate the output volume using a op-amp and a potentiometer.

![image](https://stasis.hackclub-assets.com/images/1775035090080-noa17x.png)

I also designed a small capacitor bank to smooth the voltage and prevent voltage ripples
