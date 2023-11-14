# Line-Follower-Robot
A Robot that can follow a line using L293D motor with Arduino Uno R3 and Infared LED

![robot](https://github.com/BruceTee23/Line-Follower-Robot/assets/149126740/74f09545-eac4-479c-b68b-4c96ade952c4)


**What you need:**
+ 1 x Arduino Uno R3
+ 1 x L293D DC Motor Driver Shield
+ 1 x Car chassis
+ 2 x Gear motor
+ 2 x Car tire
+ 2 x Speed encoder
+ 4 x Fastener
+ 1 x Universal wheel 
+ 1 x AA Battery box 
+ 4 AA Battery
+ Switch
+ 2 x Infrared Obstacle Avoidance Sensor
+ 3 x Jumper wires
+ Electrical tape
+ USB 2.0 A Male to B Male 28/24AWG Cable
+ Optional: 22 - 24 AWG wire, Soldering gun, soldering wire
+ All necessary screw and nut. Typically M3 nuts and bolts. 


**Hardware Setup:**
Follow the circuit diagram for details


**Software Setup:**
+ Arduino IDE
+ Adafruit Motor Shield Library Master (Arduino IDE/Library Manager/Search Shield-Install Adafruit Motor Shield Library)


**How does it work?**
+ Using IR sensors, we can take advantage of the light reflections to control the movement of the robot.
+ For example, if the robot rests on a surface, both sensors will receive lights reflected from that surface, signaling the LED next to it to lights on. This signals the robot to move straight forward. But when the surface is something like a black tape that can absorbs light, there will be no reflected light, resulting in no popup LED. If the left sensor does not receive reflected light, and so does with the right sensor. This way, the line can stay between the sensors, keeping the robot to stays on the line.
+ *Note: the key is to calibrate the sensors correctly so the second LEDs do not stay on all the time, but only enough to receive the refleted light and off when receive nothing**

**Advantages**
+ The robot satisfied the task to stay on the line to its final destination
+ Simplicity

**Disadvantages**
+ The robot does not move straight in a line

