We connect LED to a digital pin of Arduino and control it using code.
Pin Connections
LED Connection
LED positive (long leg) → Arduino pin 13
LED negative (short leg) → GND (through 220Ω resistor)

LED Blinking 

int ledPin = 13;

void setup() {
  pinMode(ledPin, OUTPUT);
}

void loop() {
  digitalWrite(ledPin, HIGH);
  delay(1000);
  digitalWrite(ledPin, LOW);
  delay(1000);
}

 in this code,
 int ledPin = 13;  //this stores the LED pin number in a variable.

pinMode(ledPin, OUTPUT);  //tells Arduino that LED is an output device.

digitalWrite(ledPin, HIGH);  //turns LED ON.

delay(1000);  //waits for 1000 milliseconds (1 second).

digitalWrite(ledPin, LOW);  //turns LED OFF.

The loop() function runs again and again, so the program written above run again and again which keeps LED blinking.

the LED is connected to pin 13 of the Arduino. The pin is set as an output in the setup function. Inside the loop function, the LED is turned ON and the program waits for one second. After that, the LED is turned OFF and again waits for one second. Since the loop function runs continuously, the LED keeps blinking with a delay of one second.

Use Button to Turn LED ON/OFF

int ledPin = 13;
int buttonPin = 7;

void setup() {
  pinMode(ledPin, OUTPUT);
  pinMode(buttonPin, INPUT_PULLUP); 
}

void loop() {
  int buttonState = digitalRead(buttonPin);

  if (buttonState == LOW) {  
    digitalWrite(ledPin, HIGH);
  } else {
    digitalWrite(ledPin, LOW);
  }
}

In this code,
pinMode(buttonPin, INPUT_PULLUP);  //uses Arduino’s internal resistor, so no external resistor needed.

int buttonState = digitalRead(buttonPin);  //reads button value:

LOW →  button is pressed

HIGH → button is not pressed

if (buttonState == LOW)  // it tells when button is pressed → LED turns ON.
else LED turns OFF

Here, a push button is used to control the LED. The LED is connected as an output and the button is connected as an input using the internal pull-up resistor. When the button is pressed, the input pin reads LOW and the LED turns ON. When the button is not pressed, the input pin reads HIGH and the LED remains OFF.


Change Blinking Speed using Delay

int ledPin = 13;
int delayTime = 500;

void setup() {
  pinMode(ledPin, OUTPUT);
}

void loop() {
  digitalWrite(ledPin, HIGH);
  delay(delayTime);
  digitalWrite(ledPin, LOW);
  delay(delayTime);
}

In this code, smaller the delay faster is the blinking speed and larger the delay slower is the blinking speed.Changing the delay time varies the speed.
The delay time is stored in a variable. By changing the value of the delay variable, the blinking speed of the LED can be increased or decreased. Smaller delay values make the LED blink faster, while larger values make it blink slower.