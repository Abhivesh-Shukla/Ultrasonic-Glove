# ULTRASONIC GLOVES

This project uses an ultrasonic sensor and an Arduino to measure distances and activate a buzzer based on the proximity of an object. The buzzer sounds at different frequencies as the object gets closer, providing an auditory alert system.

## Features

- Measures distances using an ultrasonic sensor (HC-SR04).
- Activates a buzzer with varying frequencies based on object distance.
- Provides real-time distance readings via the Serial Monitor.

## Components Required

- Arduino Uno
- Ultrasonic Sensor (HC-SR04)
- Buzzer
- Jumper Wires
- Breadboard

## Circuit Diagram

![Ultrasonic dig.pdf](https://github.com/sukhum29/Ultrasonic-Glove/blob/main/Ultrasonic%20dig_page-0001.jpg)

**Arduino connection:**
- Vcc to 5V
- GND to GND
- Trig to Pin 8
- Echo to Pin 7

**Buzzer connection:**
- Positive to Pin 4
- Negative to GND


## Usage

- Connect the Arduino to your computer using a USB cable.
- Open the Arduino IDE and upload the provided code to the Arduino.
- Open the Serial Monitor (Tools > Serial Monitor) to view the distance readings.
- Place an object in front of the ultrasonic sensor and move it closer or farther away.
- Observe the buzzer sound changing frequency based on the distance to the object. The closer the object, the faster the beeping.

## Results

1. Distance Measurement: The ultrasonic sensor accurately measures distances and sends the data to the Arduino.
2. Auditory Alerts: The buzzer emits different beeping patterns based on the measured distance:
      - Distance > 50 cm: Slow beeping (200 ms interval)
      - Distance 25-50 cm: Medium beeping (100 ms interval)
      - Distance 10-25 cm: Fast beeping (50 ms interval)
      - Distance < 10 cm: Rapid beeping (25 ms interval)
3. Real-time Feedback: The distance measurements are displayed on the Serial Monitor in real-time, allowing for easy monitoring and adjustments.
