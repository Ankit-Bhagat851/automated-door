# automated-door
We have used IR sensor connected with Arduino UNO.
Components used: Arduino Uno , IR sensor, servo motor, breadboard, jumper wires, LED, 9V battery.
The IR sensor consists of IR Emitter LED and IR Receiver. The emitter transmits a signal which is then reflected back from human/object and received by receiver. The range of the IR sensor can be increased or decreased based on our requirement via a potentiometer (attached to IR sensor).
The IR sensor connected on breadboard sends a signal with a particular address. The sensor give an input of 1 if a human or an object comes in its range, and 0 if a human or an object is not in its range. These signals are then received by Arduino UNO, which is coded to decode signals with a particularad dress. 
After the signal is decoded, when input is 1 then LED glows (if already glowing, it will keep glowing until 0 input is passed) , and when input is 0 then the LED is turned off (if already turned off it will remain off until 1 input is passed).
Simultaneously when input is 1 and LED is glowing the servo motor will open the door(at a particular angle which is already set in the coding). And if the input is 0 and LED is turned off the servo motor will close the door.
