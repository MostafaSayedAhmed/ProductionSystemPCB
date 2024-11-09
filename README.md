# Production System PCB
Internship final project for Embedded system track internship offered by Egypt Makes Electronics company
## Desciption
### 1- Prerequisites
Design a system that simulates a production process in a factory using the following
hardware:
• Two microcontrollers.
• LCD
• Keypad
• Temperature Sensor
• LDR Sensor
• Fan
### 2- System Description:

Design a multi-function machine that can do the following using modes with only one
switch to switch between the modes of operation.
To Enter the operation mode, the user must Enter his password first [1,2,3,4]
Then using a single switch, the user can switch between the following modes as follow:
The first press on the switch → will go to Mode A
The second press on the switch → will go to mode B
The third press on the switch → will go to mode B
<dl>
  <dt>Mode A: ‘Calculator’</dt>
  <ds>
On Microcontroller 1: ‘
Implement a calculator, Numbers should be from 0 to 9, and the operation is (+ -
\* / )
Display on the first MCU LCD.
</ds>
  <dt>Mode B: ‘Alarm System’</dt>
<ds>On Microcontroller 1:
User need an alarm system for a server room, A led toggle every 1 sec “flashing”,
and the value of the temp. sensor control the flashing of the led.
<ul>
<li> if the value increased than 50c:
  <ul>
    <li>
 The led will be flash every 100msec, buzzer will on and off every
100 msec
    </li>
    <li>
Send Signal to Microcontroller 2 to move the motor in CW
direction with maximum speed. Using any communication
protocol (i.e. UART)
  </li>
  </ul>
  </li>
<li>
 If the value is lower than 50c:
  <ul>
  <li>
The led will be flash every 1 sec, buzzer and motor are turned
off.
</li>
  <li>
 Send Signal to Microcontroller 2 to move the motor in CCW
direction with half speed. Using any communication protocol
(i.e. UART)
On Microcontroller 2:
Controller the motor speed according to the received signal

</li>
</li>
</ul></ul>
</ds>
<dt>Mode C: ‘Sun light indication’ </dt>
<ds>
  On Microcontroller 2
<ul>
<li>if LDR detect the high amount of light:
The Led will turned off and the second MCU will send txt to be print on
LCD “Morning” of the first MCU through UART. </li>
  <li>if LDR detect the Low amount of light:
The led will turned on and the second MCU will send txt to be print on LCD
“Night” of the first MCU through UART.</li>
</ul>
</ds>
</dt>

<p>
  
</p>
