# SMOKE-DETECTION-SYSTEM
A smart safety prototype that monitors air quality and triggers visual and auditory alarms when smoke or gas is detected.
📝 Project Overview
This project is a prototype of a smart smoke detection system designed to ensure home or industrial safety. Built and simulated entirely within Autodesk Tinkercad, it uses an Arduino Uno to process data from a gas sensor.

When smoke or flammable gas concentrations exceed a pre-defined safety threshold, the system immediately alerts the user by activating a loud piezo buzzer and flashing a red warning LED. Under normal conditions, a green LED indicates that the air is safe.

This project serves as an excellent introduction to analog sensor reading, conditional logic in C++, and output control using Arduino.

✨ Key Features
Real-time Monitoring: Continuously reads analog data from the gas sensor.

Dual-Alarm System: Utilizes both auditory (buzzer) and visual (Red LED) cues for alerts.

Safe State Indicator: A Green LED provides constant reassurance when air quality is good.

Adjustable Threshold: The sensitivity of the smoke detection can be easily tuned within the code to suit different environments.

Fully Simulated: No physical hardware required; runs entirely in the browser via Tinkercad.

🛠️ Hardware Components (Simulated)
Arduino Uno R3

Gas Sensor (Simulates MQ-2/MQ-5)

Piezo Buzzer

Red LED (Alarm)

Green LED (Safe status)

Resistors (220Ω for LEDs, 4.7kΩ for sensor pull-down if required by specific Tinkercad setup)

Breadboard and Jumper Wires

🧠 How It Works
The Gas Sensor acts as a variable resistor. As gas concentration increases around the sensor, its resistance changes, resulting in a higher analog voltage output.

The Arduino Uno reads this analog voltage on an analog input pin (e.g., A0), converting it into a digital value between 0 and 1023.

The code compares this real-time value against a defined Threshold Variable (e.g., 400).

IF the sensor value > threshold: The Arduino sets the Red LED pin HIGH and activates the Buzzer.

ELSE: The Arduino keeps the Red LED/Buzzer LOW and sets the Green LED pin HIGH.

🚀 How to Run the Simulation
You don't need to download any code to see this in action!

Click the Tinkercad link below:

https://www.tinkercad.com/things/4UMnJ9gIIVC/editel?returnTo=%2Fdashboard

Click the green "Start Simulation" button in Tinkercad.

Click on the Gas Sensor. A small cloud of "smoke" will appear. Drag this cloud towards the sensor to simulate a smoke event and trigger the alarm.

📸 Screenshots  <img width="1366" height="510" alt="smoke detection system" src="https://github.com/user-attachments/assets/53a2ca73-dae1-4265-bf1f-15085de41553" />
