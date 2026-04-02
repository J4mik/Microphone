# Design

## CAD
<img width="1136" height="634" alt="Screenshot 2026-04-02 125531" src="https://github.com/user-attachments/assets/c658bb70-4bf2-49ae-a37d-09abddedd273" />
<img width="1180" height="619" alt="Screenshot 2026-04-02 125512" src="https://github.com/user-attachments/assets/3ec3b3fd-fed8-4020-8ce3-0562572a43f7" />
The microphone shell was designed in onshape. The step file will be included in the repo. 


## PCB
<img width="1031" height="788" alt="Screenshot 2026-04-02 125434" src="https://github.com/user-attachments/assets/e96eb1cd-b5ef-4b2f-8962-265949b7751f" />
<img width="1309" height="439" alt="Screenshot 206-04-02 125303" src="https://github.com/user-attachments/assets/e7664adc-c35f-4d65-af02-830ec2c799dd" />
<img width="1382" height="445" alt="Screenshot 2026-04-02 124855" src="https://github.com/user-attachments/assets/fe09349e-a938-426e-aa9d-76eba6ccd450" />

The components on the left of the PCB are the complementary components for the [microphone capsule](https://www.digikey.co.uk/en/products/detail/primo-company-limited/EM415N/25873214). see the [datasheet](https://www.primocorp.co.jp/product-corp/fileview/30/EM415N.pdf) for more details
The capacitors on the right of the schematic are buffering capacitors used to reduce transient voltage spikes and smooth out the voltage.

The EasyEDA files for the PCB will be included in the repo

# BOM

| item | price | quantity | link |
| ---- | ----- | -------- | ---- |
| Microphone arm | 18.63$ | 1 | [Aliexpress](https://www.aliexpress.com/item/1005007097415626.html?spm=a2g0o.cart.0.0.5cc338dadaYcHK&mp=1&pdp_npi=6%40dis%21USD%21USD%2019.82%21USD%2018.63%21%21USD%2018.63%21%21%21%40211b80f717751297886618414e93eb%2112000056010576149%21ct%21UK%214617185825%21%211%210%21) |
| Foam Windscreen | 6.00$ | 1 | [Aliexpress](https://www.aliexpress.com/item/1005009561527498.html?spm=a2g0o.productlist.main.16.477fe533sd0Kow&algo_pvid=e2f2edab-4be3-4773-93d4-60ee0e0f2838&aem_p4p_detail=202604010629124364545112152100001619661&algo_exp_id=e2f2edab-4be3-4773-93d4-60ee0e0f2838-15&pdp_ext_f=%7B%22order%22%3A%2255%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21GBP%215.12%214.81%21%21%216.58%216.18%21%402103846917750501522426650e7109%2112000049466405873%21sea%21UK%214617185825%21X%211%210%21n_tag%3A-29919%3Bd%3Ad87f1b19%3Bm03_new_user%3A-29895%3BpisId%3A5000000203423557&curPageLogUid=8va68lgm0drq&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005009561527498%7C_p_origin_prod%3A&search_p4p_id=202604010629124364545112152100001619661_4) |
| Microphone Capsule | 21.63$ | 1 | [DigiKey](https://www.digikey.co.uk/en/products/detail/primo-company-limited/EM415N/25873214) |

Other component were also used. This inmcludes capacitors, resistors and an aux port

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

I added a chamfer to the front of the shell so the windscreen will fit easier

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
