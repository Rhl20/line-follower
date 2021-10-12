# line-follower
Concepts of Line Follower Concept of working of line follower is related to light. We use here the behavior of light at black and white surface. When light fall on a white surface it is almost full reflected and in case of black surface light is completely absorbed. This behavior of light is used in building a line follower robot.




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
