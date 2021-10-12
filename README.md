# line-follower
Concepts of Line Follower Concept of working of line follower is related to light. We use here the behavior of light at black and white surface. When light fall on a white surface it is almost full reflected and in case of black surface light is completely absorbed. This behavior of light is used in building a line follower robot.



# code:
int pin=8;
int pin1=2;
int pin2=3;
int pin3=4;
int pin4=5;
int value;
void setup() {
Serial.begin(9600);
pinMode(pin,INPUT); 

pinMode(pin1,OUTPUT);
pinMode(pin2,OUTPUT);
pinMode(pin3,OUTPUT);
pinMode(pin4,OUTPUT);// put your setup code here, to run once:

}

void loop() {
 value=digitalRead(pin);
 
if (digitalRead(pin)==0)
{
digitalWrite(pin1,HIGH);
digitalWrite(pin2,HIGH);
}
else
digitalWrite(pin1,LOW);
digitalWrite(pin2,LOW);
}
# explaination
In this arduino based line follower robot we have used IR Transmitters and IR receivers also called photo diodes. They are used for sending and receiving light. IR transmits infrared lights. When infrared rays falls on white surface, it’s reflected back and catched by photodiodes which generates some voltage changes. When IR light falls on a black surface, light is absorb by the black surface and no rays are reflected back, thus photo diode does not receive any light or rays.

Here in this arduino line follower robot when sensor senses white surface then arduino gets 1 as input and when senses black line arduino gets 0 as input.
![image](https://user-images.githubusercontent.com/92295704/136910676-ba8f143d-53e4-424f-bd74-d5cfc91f87b1.png)

