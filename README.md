📌 Overview

This project simulates a traffic light system with a pedestrian crossing button using Arduino.

Normal operation cycles through Green → Yellow → Red

When the push button is pressed, the system switches to pedestrian mode, stopping traffic and allowing safe crossing

🧰 Components Required

-Arduino Uno (or compatible board)

-3 LEDs (Red, Yellow, Green)

-1 Push Button

-Resistors (220Ω for LEDs, 10kΩ for button if needed)

-Breadboard & Jumper Wire

⚙️ Working Principle

🚦 Normal Mode (Button NOT Pressed)

-Green ON → 4 sec

-Yellow ON → 4 sec

-Red ON → 4 sec

-Repeats continuously

🚶 Pedestrian Mode (Button Pressed)

-Displays message: "Please WAIT, PEDESTRIAN CROSSING"

-Red ON → 6 sec (vehicles stop)

-Yellow ON → 4 sec

-Green ON → 4 sec
