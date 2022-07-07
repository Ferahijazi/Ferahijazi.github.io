---
layout: post
title:  PCB Design
date:   2022-06-07
image:  
tags:   PCB Kicad

---

**Defining Goals** :

* Make a PCB board using Kicad
* Play around with the design to make it look more expressive, shaped like a cat for example

---

After watching the video from the electronics design week and getting familiarized a little bit with the different **components** and what they do.

**Some of the components mentioned** :

* **Ribbon Cable** (wires in a ribbon) and is graded by what is called **AWG** which refers to the gauge of the diameter. Gauge is a measure of the size of a wire which correlates with how much current you can put through the wire.

![]({{ site.baseurl }}/images/ribbon_cable.webp){: width="40" }{: height="40" }

* **IDC Connector**

* **Slide Switch** can be used as a configuration switch or a low power switch. 
* **Resistor** used for limiting the flow of current
* **Capacitor** used for local charge storage
* **Polarized capacitors** is a component that is been a capacitor and a battery, they can store large amounts of power
* **Crystal/Resonator** are used to determine time. Mainly used to determine high resolution timing/high accuracy
* **Inductor** when a current flows through it, it creates a magnetic field
* **Diods** the current can go only in one direction. There are two sides to the diod, one is called anode and the other cathode
* **LEDs** are a particular kind of diod. LEDs have a particular indication for direction. For instance, if you see a green line on one side and it is on the cathode side. You always use an LED with a current limiting resistor and the resistor will determine how bright the LED is going to be
* **Transistor** there are bipolar ones, which we are not going to use. Mosfits are one of the key components in the class, there is a P mosift (source of current) and an N mosfit(sink of current). There is a drain and a source on one side and the gate on the other. RDS is the resistence between the drain and the source. Both are used to control things that take a lot of current like motors or speakers.
* **Regulators** are regulated by current input voltage and output voltage. You need a capacitor on the right side
* **Amplifiers** are now built into the processor, you can pick them in software and you don't need a seperate component.
* **Micro-controllers** are a world of their own, there is so much to cover and learn about.

---

#### Circuits!

I figured I should first familiarized myself a little bit with circuits so I watched a few videos explaining Ohms law. I already got an introduction to electricity thanks to the arduino course, there are more videos to watch yet I will revisit them later.

Drawing circuits is called EDA which stands for electronics design automation
The drawings need to be hirarchical and parametric 
There are *footprints*
*Kirchhoff's current law* 

**REFDES** is a combination of numbers and letters used to identify electrical components on a board
---

#### Learning kicad

As an excerise I followed along *an intro to Kicad* Series on youtube. I created a local library and created a symbol inside of it. Then 

Putting the datasheet & the schematic desing side by side can be useful



--- 
#### Steps :

* First, I installed the fab academy library which can be found on the electronics design week and added it to kicad.


https://www.youtube.com/watch?v=c2niS9ZRBHo


