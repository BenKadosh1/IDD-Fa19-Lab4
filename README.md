# Paper Puppets

*A lab report by Ben Kadosh*

## In this Report

## Part A. Actuating DC motors

**Link to a video of your virbation motor**

## Part B. Actuating Servo motors

### Part 1. Connect the Servo to your breadboard

**a. Which color wires correspond to power, ground and signal?**

Red --> Power

Brown --> Ground

Orange --> Signal

### Part 2. Connect the Servo to your Arduino

**a. Which Arduino pin should the signal line of the servo be attached to?**

As can be seen in line 18 of the Arduino code for Sweep, the signal line of the servo should be attached to pin 9.

Code below: 
myservo.attach(9);  // attaches the servo on pin 9 to the servo object

**b. What aspects of the Servo code control angle or speed?**

In the code snipet below (lines 22-30 from Sweep) we can see that pos will determine the position the servo moves to, so when we provide pos from 0 - 180 we are giving it a range of 180 degrees. Furthermore, the delay factor controls the speed at which the servo changes position.

for (pos = 0; pos <= 180; pos += 1) { 

  myservo.write(pos);
  
  delay(15);                       
}

The snipet below adjusts the code above to give the servo a wider range of movement, as well as faster change in positions. 


for (pos = 0; pos <= 90; pos += 1) { 

  myservo.write(pos);     
  
  delay(5); 
}

Original Video
Adjusted video


## Part C. Integrating input and output

**Include a photo/movie of your raw circuit in action.**
Link

## Part D. Paper puppet

**a. Make a video of your proto puppet.**

## Part E. Make it your own

**a. Make a video of your final design.**
 
