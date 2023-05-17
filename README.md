# LCDandKEYPAD
o use Atmega 8052 microcontroller to create a simple calculator, by entering numbers and symbols in 4*4 keypad, and  watching the results being displayed on 16×2 lcd.

# Introduction 
We aim to use Atmega 8052 microcontroller to create a simple
calculator, by entering numbers and symbols in 4*4 keypad, and 
watching the results being displayed on 16×2 lcd.
Project function is simple when anyone presses the button on 
keypad the character associated with that button will be displayed 
on the screen of 16×2 lcd, and when press the character “=”, the 
result of the arithmetic operation will be displayed on the screen 
too.

# Components and the usage of each one:
• 16×2 lcd to display the outputs.

• 4×4, numeric keypad to enter the input.

• 8051(89c52) Microcontroller

• Power supply (5 volts) to provide power to lcd.

• Crystal Oscillator (12 MHz) responsible for supplying the clock signals in microcontroller.

• Bread board (To build circuit)

• Potentiometer (Variable Resistor) To adjust Lcd contrast.

• 2 capacitors (22 pF) to be connected with crystal, used to 
oscillate it.

• 10 K ohm Resistor and 10 uF capacitor, used to create 
standard reset circuitry (connected to Pin 9 (RST) is the 
reset PIN).


#circuit connections

we connected Port-1 of 89c52 microcontroller to our 4×4
keypad data pins(P1.0-P1.7). 
where rows of 4×4 keypad connected to Port-1 pins5,6,7,8 
Connect columns of it to Port-1 pins 0,1,2,4.
Then we connected Port-2 pins of 89c52 microcontroller to 
our 16×2 lcd data pins(D0-D7). 
We connected:
enable pin of lcd with Port-3 to the third pin. 
RS(register select) pin of lcd with Port-3 pin 5.
RW(read-write)pin of lcd to 8051 Port-3 pin 4.
Connect Rest of the connections are manual which we do 
in our all circuits. 
Ground Pin 20. 
Apply 5 volts to pin 31 and VDD pin in Lcd. 
Connect Oscillator with pin#19(XTAL-1) and 18(XTAL-2) 
of 8051 in parallel to two 22 pF capacitors. 
reset button with pin#9(reset) of 89c52 microcontroller with 
10 Kohm Resistor and 10 uF capacitor.
Connecting a potentiometer to VEE to control the contrast 
of the LCD.

# hardware implementation 
![image](https://github.com/khloodmontaser/LCDandKEYPAD/assets/113125527/431ff9a7-8d7b-4e02-9cdc-2329ee42d1f6)
