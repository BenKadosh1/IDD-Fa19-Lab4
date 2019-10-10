# Paper Puppets

*A lab report by Ben Kadosh*

## In this Report

## Part A. Actuating DC motors

[Actuating DC Motor Vibrating - Youtube Link](https://www.youtube.com/watch?v=6Hyex5jV6mY&feature=youtu.be)


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

for (pos = 0; pos <= 180; pos += 1)  
{  
  myservo.write(pos);  
  delay(15);                       
}

The snipet below adjusts the code above to give the servo a narrower range of motion, as well as faster changes in positions. 


for (pos = 0; pos <= 90; pos += 1)  
{  
  myservo.write(pos);  
  delay(5);  
}

I uploaded videos of both sets of code for context below.

[Original Servo Sweep](https://www.youtube.com/watch?v=7oR3E7tIOlw&feature=youtu.be) 

[Adjusted Servo Sweep](https://www.youtube.com/watch?v=qBB4fSvNwlg&feature=youtu.be)

Another item to note, as mentioned on the Arduino website's Servo library overview, "Standard servos allow the shaft to be positioned at various angles, usually between 0 and 180 degrees." This explains why the Servo motor was not completing 360 degrees of motion when attempted. 

[Arduino - Servo Library Reference](https://www.arduino.cc/en/reference/servo)


## Part C. Integrating input and output

**Include a photo/movie of your raw circuit in action.**

Link

## Part D. Paper puppet

**a. Make a video of your proto puppet.**

## Part E. Make it your own

**a. Make a video of your final design.**

In an effort to add a bit of humor to this lab, my brother and I challenged eachother to a dance-off with our puppets. We added embarassing photos to the puppets as well. Links below!
