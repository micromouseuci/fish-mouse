# fish-mouse

<details><summary> 3D Renders </summary> 
 
![alt text](https://i.gyazo.com/6f8037a90cf6d5079d7c5b4d399169a1.png "top")
![alt text](https://i.gyazo.com/6857428b345924a1912f8933cdfc5366.png "side")
![alt text](https://i.gyazo.com/76046006bc29e7ea5711500e6e7092ed.png "front")
</details>

<details><summary> PCB traces </summary> 
  
![alt text](https://i.gyazo.com/c64162fd798aef0fdc69f54d9545e707.png "pcb traces")
</details>

<details><summary> Schematic </summary> 
  
![alt text](https://i.gyazo.com/9caa049c938e77acb3995b97b3d5b04c.png "schematic")
</details>

<h2> Parts </h2>

* __SN754410NE__ _(U2)_ - Motor driver, used to control the speed and direction of the two motors.
* __Teensy 3.2__ _(U1)_- Processor, will run code.
* __IR Emitters__ _(D0-D3)_ - Send an IR signal. Each is connected to a digital pin on the Teensy, allowing them to individual turn on and off.
* __IR Reciever__ _(Q0-Q3)_ - Reads how strong the IR signal is, depending on the value it reads it is able to detect if there is a wall, and how may cells away it is.
* __Pololu 3081__ _(U5, U4)_ - Motor encoders, used to keep track of wheel rotations.
* __LM1084__ _(U3)_ - Voltage regulator, a LDO regulator that gives a 5V source from the LiPo.
* __Switch__ _(SW1)_, __Buzzer__ _(BZ1)_, __LEDs___ _(D4, D5)_ - Used for interfacing with the mouse.
* __...Ω__ _(R0, R1, R2, R3)_ - Current limiting resistors for Emitters.
* __...Ω__ _(R4, R5, R6, R7)_ - Current limiting resistor for Recievers.
* __...Ω__ _(R11)_ - Pull Up resistor for switch.
* __...Ω__ _(R8, R9)_ - Current limiting resistors for LEDs.

Switch socket is designed for a mechanical keyboard switch
LED size so .... will work
Buzzer pin spacing is ....

<h2> Building Notes </h2>

1. Use header pins and sockets for the Teensy and Motor driver to make replacing parts easier.
1. With the ir emitters and receievers short end is positive.
1. When connecting wires to the motor encoder, make sure none of the wires are rubbing against the magnetic disk.
1. When connecting the encoder make sure to double check 


Software
()
