# ARDUINO-IDE
Blinking code, chasing light effect

int leds[] = {6, 7, 8, 9};

void setup() {
  for (int i = 0; i < 4; i++) {
    pinMode(leds[i], OUTPUT);
  }
}
 void loop(){
  for (int i = 0; i < 4; i++) {
    digitalWrite(leds[i], HIGH);
    delay(100);                                              /* Select delay(time) To change blinking speed fast and slow */      
    digitalWrite(leds[i], LOW);
  }
 }/*Sketch uses 968 bytes (3%) of program storage space. Maximum is 32256 bytes.
Global variables use 17 bytes (0%) of dynamic memory, leaving 2031 bytes for local variables. Maximum is 2048 bytes.
avrdude: ser_open(): can't open device "\\.\COM3": Access is denied.*/
