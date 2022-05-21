
KEYPAD LOCK Door Unlock

-: Mentor :-
Avichal Gupta
Ritik Raj
-: Team :-
Kaushik Patil
Sambit Prabhu
Harshwardhan Raghu
Abhijith Reddy Dasari
Devansh Kumar



Problem Description
Nowadays, our society is facing a lot of issues and one of the prime issues to ponder upon is security. People tend to look for a solution that is reliable, sturdy, long-lasting, and also cost-effective. Modern technologies are expensive and therefore there are very few affordable security solutions in the market for people to buy for making their homes and valuables secure.

Objective
Our aim is to make an affordable, easy to use, reliable security door lock using Arduino and a keypad lock.

Components Required

1. ARDUINO:
Arduino Uno is a microcontroller board based on the ATmega328P.It has 14 digital input/output pins (of which 6 can be used as PWM outputs), 6 analog inputs, a 16 MHz ceramic resonator (CSTCE16M0V53-R0), a USB connection, a power jack, an ICSP header and a reset button. It contains everything needed to support the microcontroller; simply connect it to a computer with a USB cable or power it with an AC-to-DC adapter or battery to get started. It is an important component used in electronics and robotics projects.
 
2.BREADBOARD:
A breadboard is a solderless device for temporary prototype with electronics and test circuit designs. Most electronic components in electronic circuits can be interconnected by inserting their leads or terminals into the holes and then making connections through wires where appropriate. 
 

3. SERVO MOTOR:
A servo motor is a type of motor that can rotate with great precision. Normally this type of motor consists of a control circuit that provides feedback on the current position of the motor shaft, this feedback allows the servo motors to rotate with great precision.
     
4. JUMPER CABLES: 
A  jumper cable is an electrical wire, or group of them in a cable, with a connector or pin at each end, which is normally used to interconnect the components of a breadboard or other prototype or test circuit, internally or with other equipment or components, without soldering. Jumper Cables form an integral part of any electronics project. It makes all the connections between necessary components.
 
              
5. BUZZER:      
A buzzer or beeper is an audio signalling device, which may be mechanical, electromechanical, or piezoelectric (piezo for short). Typical uses of buzzers and beepers include alarm devices, timers, and confirmation of user input such as a mouse click or keystroke.                      
 

6.LED BULBS:
A light-emitting diode (LED) is a semiconductor light source that emits light when current flows through it. Electrons in the semiconductor recombine with electron holes, releasing energy in the form of photons. A very commonly used device in electronics.                                
          

7 .16×2 LCD DISPLAY:                 
Liquid Crystal Display or LCD is a flat, electronic device generally used as a screen in televisions, computers, smartphones and display signs for producing still and movable images. LCD is composed of liquid crystal particles. Liquid crystals generally do not emit light on their own rather they are illuminated by a fluorescent backlight.
 
8. KEYPAD LOCK:
Keypad systems are one of the best ways to go keyless and safeguard a property. Often, they operate in connection with access control systems. For this project we are using a 4x4 keypad.
How a Keypad Locks Work
Instead of a key, this type of lock system requires a numerical code to grant entry to a facility or property. The code is punched in by users via a numerical pad, similar to those on a basic calculator that one uses. If the correct code is entered, the door lock should be released. Some mechanisms require batteries or a small electrical current in order to unlock.
Some keypad locks have an integrated security feature that keeps the door locked for a set amount of time ( 15 seconds or  1 minute ) after several incorrect attempts to enter the code.
a. Keyless Entry and Exit
The convenience of keyless entry is perhaps the most outstanding benefit of using a keypad lock. No fumbling around with keys when you’re trying to unlock your door at night, no calling a locksmith when you’re locked out of your house, no frantic search for your keys when you’re rushing to get out the door, no need for keys, period. Simply punch in your PIN number on the keypad and voila–you’re inside with no fuss and no muss. When it’s time to leave the house, a keypad lock will automatically lock behind you, essentially eliminating that all-too-common scenario where you’re halfway to work and wondering whether you locked the front door or not.
b. Time-Determined Locking and Unlocking Schedules
Time-determined access control, “scheduling”, is one of the most outstanding benefits of using a keypad lock. Business owners can schedule time periods for doors to be locked or unlocked in order to keep strict control over employee access to certain areas of the premises. Homeowners can ensure that their doors are always locked at night without having to make the nightly rounds to do so. The ability to set time-determined locking and unlocking schedules will save both time and money, and it will ensure a higher degree of safety and convenience versus using traditional locks and keys.
c. Increased Security
Traditional locks are subject to both lock picking and lock bumping, the latter of which leaves no signs of forced entry, making it difficult to collect from your insurance company should a theft occur.
d. Additional Safety for Kids
Keypad locks eliminate the need for your child to keep up with a house key if they come home from school before you come home from work. During a busy school day, it’s relatively easy for a child to accidentally drop or otherwise misplace a house key, and if they’re locked out of the house when they come home from school, this poses a potential risk to their safety. With a keypad lock, all your child needs to have is their personal security code, and they can enter it into the keypad to unlock the front door. Once they’re inside, the keypad lock will automatically lock behind them. 
e. Better Durability
Traditional locks can get worn down and eventually malfunction due to frequent or heavy use. If you’ve ever had to deal with a lock that requires you to jiggle or shimmy the key just to get it to work, you know how aggravating it can be. Accidentally breaking a key off inside the lock can also be a pain to deal with. Keypad locks are remarkably durable because they don’t sustain the repetitive friction of inserting and turning keys; pressing a few buttons on the keypad is all that’s required to engage the lockset and open the door.
 

Working
1.	Firstly, we make the necessary connections among Arduino, breadboard, keypad lock, lcd screen, servo motor, buzzer and LED bulbs. For the code, we used some necessary libraries like <LiquidCrystal.h>, <Keypad.h>, <string.h>, <Servo.h> required for the components we used. 
The connections are as follows:
a)	All the analog pins (A0-A5) are connected to the LCD screen via the breadboard. Arduino controls all the output on the screen.
b)	The digital pin 11 is connected to the servo motor which locks and unlocks the door.
c)	The digital pins 2-9 are connected to the keypad lock for taking the input from it.
 

We set the system initially in such a way that it remains locked all the time until we open it with a proper passcode/ password.

 


2.	Now, we set a password for the door to unlock in the keypad lock ( here ABC123). Then, if we type the password correctly, the door will unlock with a message on  the lcd screen-“Unlocked” otherwise it will show “locked”. 

3.	Also on pressing the key ‘*’ on the keypad, the door gets locked instead of an automatic locking mechanism where usually the person must enter inside within a stipulated time interval ( the idea of fixing a stipulated time for the lock is not going to be good when multiple people need to enter the house where they need to unlock the door multiple times with the password). Clicking ‘#’ invokes master control over the device when the master key is entered. Now, required changes can be made to the device ( like changing password etc.).
 

The circuit diagram is as follows:
 
As for the software simulation, we can do it on tinkercad circuit simulator as it has all the required components like Arduino, keypad lock, breadboard etc.

Feasibility in online mode

We believe that this project is feasible in the online mode because simulation software is available for Arduino hardware, and once the simulation is completed, assembling the hardware should be a relatively straightforward job for one person.


