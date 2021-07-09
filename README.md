# Motor-drive-design-and-implementation-for-two-wheel-robot-base

This circuit design moving two motors using H brage l298, I used tinkercad website online to design it, The Circuit consists of : 
1. Arduino. 
2. one H brage l298. 
3. one battery 9 volts. 
4. two DC Motors.


# Diagram Of The Circuit : 

![image](https://user-images.githubusercontent.com/86571348/125125089-cb7b3b80-e101-11eb-8914-133c847888cb.png)


# C Of The Circuit : 

void setup()
{
  pinMode(11, OUTPUT);
  pinMode(10, OUTPUT);
  pinMode(7, OUTPUT);
  pinMode(6, OUTPUT);
}

void loop()
{
  digitalWrite(11, HIGH);
  digitalWrite(7, HIGH);
  
  delay(1000); // Wait for 1000 millisecond(s)
  
  digitalWrite(11, LOW);
  digitalWrite(7, LOW);
  
  delay(1000); // Wait for 1000 millisecond(s)
  
  digitalWrite(10, HIGH);// Moving clockwise
  digitalWrite(6, HIGH);// Moving clockwise

  delay(1000); // Wait for 1000 millisecond(s)

  digitalWrite(10, LOW);// Moving counterclockwise
  digitalWrite(6, LOW);// Moving counterclockwise

  delay(1000); // Wait for 1000 millisecond(s)

  
}
