# Arduino
//MIKE LOOK ARDUINO CODE THIS IS THE BUTTON
/*
  Button: Turns an LED on or off when pressed
  13 = Pin for LED
  2 = Pin for Button
  
  source:  http://www.arduino.cc/en/Tutorial/Button
*/



// variables will change:
int buttonState = 0;         // variable for reading the pushbutton status

void setup() {
 
  pinMode(13, OUTPUT);
  // initialize the pushbutton pin as an input:
  pinMode(2, INPUT);
}

void loop() {
  buttonState = digitalRead(2); //reads button state: HIGH or LOW

  // check if the pushbutton is pressed. If it is, the buttonState is HIGH:
  if (buttonState == HIGH) {
    // LED turns on:
    digitalWrite(13, HIGH);
  } else {
    // LED turns off:
    digitalWrite(13, LOW);
  }
}
