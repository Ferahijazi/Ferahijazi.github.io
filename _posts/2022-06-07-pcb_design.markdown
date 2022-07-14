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

* Note : **learning arduino** helps with prototyping, you can create your prototype to understand which components you need for your project as well as how to connect them. Then you can take the prototype and recreate it in kicad.
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

**REFDES** which stands for *reference designator* is a combination of numbers and letters used to identify electrical components on a board. 
---

#### Learning kicad

As an excerise I followed along *an intro to Kicad* Series on youtube. I created a local library and created a symbol inside of it.  

Note: Putting the datasheet & the schematic desing side by side can be useful



--- 
#### Steps :

* First, I installed the **fab academy library** which can be found on the electronics design week and added it to kicad.

https://gitlab.fabcloud.org/pub/libraries/electronics/kicad

* Go to preferences > Manage Symbol Libraries
* This will open **symbol library** > add "fab.kicad_sym" there
* Go to preferences > Manage Footprint Libraries
* Add "fab.pretty" there
* Go to preferences > Configure Paths and add variable named **FAB** that points to the installation directory of the fab library as in where you saved the library on your computer.

---

##### Starting a new project

* File > new project
* Name your project and save it in a suitable folder
* Two files will pop up on the left side > the schematic file & a blank pcb file


https://www.youtube.com/watch?v=c2niS9ZRBHo

##### Running the library editor 

 ![]({{ site.baseurl }}/images/steps_kicad.png)

* Go to tools > symbol editor and press ok to load the library 

* File > new library > project > local and create a new library for the components

* **Note** if you want to store your component in a larger library that is accessible by all your projects you can choose global. The advantage of having your library assigned to a project specific (local) is that it becomes easier to share your custom parts if you were to upload your project to say something like GitHub

* Add a new symbol : following the tutorial, the component was named as 7555 which is an intigrated circuit derived from 555 made back in the 70s. The older version was made with bipolar transistors intended for things like oscillators and pulse generators. The 7555 works just like the 555 but instead of bipolar transistors, it uses CMOS. CMOS can operate at lower voltages, for our project it will be powered by a 3 volt coin cell battery 

* Google the reference designator. There we can see that intigrated circuits like our example 7555 is references by the letter U

 ![]({{ site.baseurl }}/images/reference_desig.png)

 * Save it! 

 * Click the add pins button and add GND, number 1 following the datasheet and do the same for the others.
 Keep in mind that the way to name active low pins is by typing ~{NAME}

 *  Look at the **Data Sheet** for specifics

  ![]({{ site.baseurl }}/images/datasheet_7555.png)
  *Active low pins are specified by the dash on top of the name*

  * **Advice** putting the datasheet and the library editor side by side can be helpful

  * Then go to http://www.555-timer-circuits.com/flashing-led.html and keep this schematic next to your library editor in order to know how to place your pins. Using move and rotate (r on keyboard) fix them accordingly

    ![]({{ site.baseurl }}/images/schematic_led_7555.png)
    *Add a rectangle around it once you are done!*

    * At the end of this part, you should have this schematic 

     ![]({{ site.baseurl }}/images/schematic_symbol_7555.png)

---

##### Schematic Capture/Editor

* Some information, the numbers and letters in between the boarders are a way to refer to sections. For instance you could refer to an issue located at b4 and other engineers can know where to look.


![]({{ site.baseurl }}/images/b4.png)
