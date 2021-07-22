# Control-the-motors-by-using-potentiometer
```
#include <Servo.h>
#define SERVOS 1
Servo myservo[SERVOS];  
int servo_pins[SERVOS] = {3}; 
int potpin = A0;
int pot_pin_val;  
 
void setup() {
   
  for(int i = 0; i < SERVOS; i++) {
       
  }
}
  
void loop() {
 
 
  pot_pin_val = analogRead(potpin);            
  pot_pin_val = map(pot_pin_val, 0, 1023, 0, 180);
  for(int i = 0; i < SERVOS; i++) {
   
    myservo[i].write(pot_pin_val); 
    delay(15);    
   }  
}    
```
