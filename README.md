# NE_MultiDrive
NextEngine MultiDrive  based on an Arduino Uno using a 28BYJ-48 stepper motor/ULN2003 stepper driver.

NextEngine(c) is property of NextEngine and is not affiliated with this project or code.
All NextEngine data was acquired with an i2c bus sniffer. No disassembly or code analysis
was performed on any NextEngine hardware or software. Thanks to dot_bob for helping me
with some of the i2c data analysis.

Some code based on I2C Scanner from Arduino.cc.
Attribution to Krodal, Nick Gammon, Anonymous

This sketch uses the AccelStepper library by Mike McCauley, which can be found:
http://www.airspayce.com/mikem/arduino/AccelStepper/
This implementation is easy enough to modify to use other stepper libraries, but I
chose this one because it can easily be modified to use step/dir or "wave drive" motor control
and it supports acceleration and decceleration.

_NOTE_
This is a first attempt at a MultiDrive controller using an inexpensive Arduino Uno.  This is the "second" part of the MultiDrive as you will also need the Rotary Axis [https://github.com/1bigpig/NE_RotaryTable] to make the project.  Also, the Arduinos will have to linked via I2C connections and on mine, will require pull up resistors on the SDA and SCL lines.  Also, the Arduino 5v regulator is not powerful enough to run 2 Arduinos and 2 steppers motors.  I have added a 7805 to help, otherwise the Arduinos will not run or will "brown out" and reset.

THIS IS A WORK IN PROGRESS

Bruce Clark
02/22/2021
