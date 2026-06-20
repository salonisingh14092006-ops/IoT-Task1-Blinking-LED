# IoT-Task1-Blinking-LED# Task 1 - Blinking LED

## Objective
To control an LED using an Arduino board and make it blink at a 1-second interval.

## Components Used
- Arduino Uno
- LED
- 220 Ohm Resistor
- Breadboard
- Jumper Wires
- USB Cable

## Circuit Connections
- LED Anode (+) → Pin 13 through 220Ω resistor
- LED Cathode (-) → GND

## Working Principle
The Arduino sends a HIGH signal to Pin 13, turning the LED ON.
After 1 second, it sends a LOW signal, turning the LED OFF.
This process repeats continuously.

## Code

```cpp
void setup() {
  pinMode(13, OUTPUT);
}

void loop() {
  digitalWrite(13, HIGH);
  delay(1000);

  digitalWrite(13, LOW);
  delay(1000);
}
