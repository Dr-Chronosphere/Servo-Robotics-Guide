** Unit ß **
# *Coding*

## Motors/Sensors

### Motors- types of motors

* **Claw motor** - retracts and closes. Speed ranges between 0 and 127. 0 being no speed and 127 being maxed speed.
* **Normal motor** - rotates back and forth. Speed ranges between 0 and 127. 0 being no speed and 127 being maxed speed.

### Sensors

* **Light sensor** - also known as the reflection sensor. Returns values ranging between 0 and 4095. 0 being the lightest reading and 4095 being the darkest. Measures light through the sensors.
* **Potentiometer** - returns an analog value between 0 and 1023. Measures rotation in electrical devices to restrict or control movement. Rotates 265 degrees in total.
* **Line follower** - returns values ranging between 0 and 4095. 0 being the lightest and 4095 being the darkest. Measures the black/white lines in an area.
* **Bump switch** - measures digital value. “1” means that it is a closed circuit and “0” means the circuit is open.
* **Limit switch** - measures digital value. “1” means that it is a closed circuit and “0” means the circuit is open.
* **Sonar sensor** - returns an analog value in centimeters, millimeters, inches or raw data. A value of “-1” means the sensor does not receive a “reflection”. The sonar sensor requires an input wire to   be attached to the digital port directly following the main port of the sonar sensor. Used to measure range.
* **Raw Value** - returns an analog value between 0 and 1023- used for testing new sensors or reading raw data from sensors
* Reflection - returns an analog value between 0 and 1023
* **Touch** - returns a digital value. A “1” means the sensor is being used and a “0” means the sensor is not being used.
* **Rotation** - a digital sensor that returns a counter value keeping track of how many “counts” the encoder has seen. The sensor will increment regardless of direction. The ZEX rotation sensor uses this type of sensor.
* **Sonar** - returns an analog value in inches. A value of “-1” means the sensor does not receive a “reflection”. TIP: the sonar sensor requires the “input” wire to be attached to the interrupt port int1 and int2 to function properly.
* **Digital in** - this will make the sensor port act as just a digital input.
* **Digital out** - this will cause the sensor port to send out a digital signal.

## Coding

### Commands:
* As its name implies, the motor command allows you to change the power level of a motor connected to your robot. The VEX cortex has 10 motor ports; you specify the motor port that you want to access by typing its name between the pair of square brackets of the motor command.
* For example: in the command below, it is a simple command for motor. The value 127 is the speed of the motor, and port3 is the place that the vortex is plugged in. the bracket “{“ is the start of the command, and “}” is the end of the commands.

```
Task main()
{
Motor[port3] = 127;
wait1Msec (3000);
}
```

* The sensor is used to tell the computer what it should do when it reaches a certain value. So different sensors have different commands for them. Here is an example for a touch sensor. Look at the command below. This command also included the value part. You can see the number 63 after code “forward”, this means the robot will stop the project.

```
Task main()
{
robotType(recbot);
forward(63);
untilTouch(dgtl6);
stop();
}
```

* **Statement**- the statement is a short paragraph that we write at the beginning of the whole code. It is used to tell us what we need to do in that project.

* **Pseudocode**-  pseudocode is part of a programming language that tells, in your own words, what each line of coding is doing

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTYzMDY0MjAwMywtMTYxNTI0OTUyOSwtMT
AwMTAyMjQ3M119
-->