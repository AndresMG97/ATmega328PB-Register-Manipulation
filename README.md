# ATmega328PB-Register-Manipulation
 Employed Microchip Studios to execute diverse operations on the ATmega328PB microcontroller. Leveraged the microcontroller’s data sheet and reference manual to manipulate registers effectively for various functionalities.

UseOfEEPROM: This program uses the EEPROM of the Atmega328PB mini board in order to change variables in the code when it is only connected and disconnected from a power source.

Potentiometer-ChangeLEDBrightness: This program uses timers and an ADC to change the brightness of the LED on the Atmega328PB mini board by rotating a potentiometer that is connected to it. Some of the variables and timers were dependent on the last 3 digits of my Red Id. X=0 Y=5 Z=5.

4x4Keypad-ChangeBrightness: Using the keypad connected to the Atmegaboard, depending on what button I press from 0-9, it will change the brightness of the LED on the Atmega328PB board. Some of the variables in the lab are dependent on the last 3 digits of my Red Id. X=0, Y=5, Z=5.

4x4KeypadTransmittingFrequencies: Program scans a 4x4 keypad connected to the USART ports on the Xplained mini board. Depending on the button pressed, the keypad will send a certain timing onto the mini board to represent a frequency. Then, the frequency is then outputted onto the aux cord adapter connected to the mini board as well. The aux adapter will then transmit the frequency onto a connected speaker that will produce the sound. 

LEDSlowBrightness: 	This program makes the LED brightness go from 0 to 100% in about a second and then loses the brightness slowly until it is off once the button is not being pressed. This is done by setting up a timer using the clock from the debug processor ,setting the duty cycle, and generating a PWM waveform. 

4x4Keypad-TransmittingCharacters: This program scans a 4x4 keypad connected to the USART port on the Atmega328PB in order to transmit the ASCII characters. Once the USART is initiated through the program, it runs a loop that is always scanning for the button pressed on the keypad. Once this happens, the character is transmitted and shown through the data visualizer.

TransmittingCharacters: This program uses the built in USART port on the Xplained Atmega328PB board to transmit the characters in my red id. While the mini board worked as the transmitter, I had to set up my computer to use the PUTTY software and the FT232R hardware to receive the serial string that contained my red id.
