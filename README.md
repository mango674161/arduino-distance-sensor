# Arduino Distance Sensor

A simple Arduino project that scans the surroundings using a servo-mounted ultrasonic sensor and gives feedback with LEDs and a buzzer.

## Features

* 180° servo sweep 
* Real-time distance sensing
* Multi-level alerts based on distance
* LED + buzzer feedback
* Continuous back-and-forth motion

## How It Works

The servo sweeps from 0° to 180° while the ultrasonic sensor measures distance at each angle.

* **Far (> 40 cm):** Green LED, no sound
* **Medium (10–40 cm):** Green + Red LED, low buzzer tone
* **Close (< 10 cm):** Red LED, high buzzer tone

It  behaves like a simple radar that reacts to nearby objects in real time.

## Tech Used

* Arduino (C/C++)
* Servo motor (`Servo.h`)
* HC-SR04 ultrasonic sensor
* Buzzer
* LEDs
* Breadboard + jumper wires

## Pin Setup

* Servo → Pin 3
* Trig → Pin 10
* Echo → Pin 11
* Buzzer → Pin 9
* Red LED → Pin 4
* Green LED → Pin 5
* Blue LED → Pin 6

## What I Practiced

* Servo control and sweeping motion
* Ultrasonic distance measurement
* Threshold-based decision making
* Using multiple outputs together (sound + light + motion)
* Basic embedded systems timing

## Possible Upgrades

* Add LCD/OLED distance display
* Smooth readings with averaging
* PC radar visualization
* Better buzzer scaling instead of fixed tones
* Bluetooth or data logging output
