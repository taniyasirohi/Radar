# Radar Project

## Overview
This project is a radar system designed using an ultrasonic sensor, Arduino, and a graphical user interface for real-time object detection and visualization. The system scans its surroundings and displays detected objects on a radar-like interface. The project is ideal for understanding the integration of hardware and software in embedded systems.

## Features
- **Real-time Object Detection**: Uses an ultrasonic sensor to detect objects in a specified range.
- **Graphical Representation**: Displays detected objects in a radar-like interface.
- **Servo-controlled Scanning**: The ultrasonic sensor is mounted on a servo motor for a wide range of detection.
- **Arduino-based System**: Uses an Arduino microcontroller for controlling the sensor and processing data.
- **Serial Communication**: Data transmission between Arduino and the computer via a serial interface.
- **Processing GUI**: A graphical user interface (GUI) created using Processing for visualizing the radar data.

## Components Required
1. **Hardware:**
   - Arduino Uno (or compatible board)
   - Ultrasonic Sensor (HC-SR04)
   - Servo Motor (SG90 or similar)
   - Jumper Wires
   - Breadboard (optional)
   - USB Cable for Arduino

2. **Software:**
   - Arduino IDE
   - Processing IDE (for GUI visualization)

## Circuit Diagram
- Connect the **VCC** of the HC-SR04 sensor to the **5V** pin on the Arduino.
- Connect the **GND** of the HC-SR04 to the **GND** on the Arduino.
- Connect the **Trigger (Trig)** pin of the HC-SR04 to **Arduino Digital Pin 9**.
- Connect the **Echo** pin of the HC-SR04 to **Arduino Digital Pin 10**.
- Connect the **Servo Motor's VCC** to **5V**, **GND** to **GND**, and **Control Signal** to **Digital Pin 6** on Arduino.

## Installation and Setup
1. **Arduino Code Upload:**
   - Open the Arduino IDE and install necessary libraries if required.
   - Upload the Arduino code to your board.
   - Ensure correct COM port and board settings in the Arduino IDE.

2. **Processing Setup:**
   - Install Processing IDE.
   - Run the Processing script for graphical visualization.
   - Make sure the correct COM port is used for serial communication.

## Usage
- Power up the Arduino and connect it to the PC.
- Run the Processing sketch to visualize the radar.
- The servo motor moves the ultrasonic sensor, scanning its surroundings.
- Detected objects will be displayed on the radar interface in real time.

## Code Explanation
- **Arduino Code:**
  - Controls the servo motor to move in a sweeping motion.
  - Sends trigger signals to the ultrasonic sensor.
  - Reads the echo time to calculate the distance.
  - Sends data via serial communication.

- **Processing Code:**
  - Reads serial data from Arduino.
  - Converts distance measurements into graphical points on a radar screen.
  - Updates the display in real time for continuous scanning.

## Troubleshooting
- **No data on Processing GUI?**
  - Check if the correct COM port is selected.
  - Ensure the Arduino is properly connected and powered.
  - Verify that the Arduino code is running correctly.

- **Servo Motor Not Moving?**
  - Check the wiring of the servo motor.
  - Make sure the correct pin is defined in the Arduino code.
  - Try using an external power source if the servo does not get enough power.

- **Incorrect Distance Readings?**
  - Ensure the ultrasonic sensor is properly wired.
  - Make sure there are no obstructions blocking the sensor.
  - Adjust the delay between sensor readings for better accuracy.

## Future Enhancements
- Add a larger range for object detection.
- Implement an advanced graphical interface with better visualization.
- Introduce wireless communication for remote radar monitoring.
- Improve accuracy by using multiple sensors.

## Conclusion
This radar project provides a fundamental understanding of how sensors, motors, and microcontrollers work together to create a real-time scanning system. It can be expanded and improved for various applications such as security, robotics, and automation.

## License
This project is open-source. Feel free to use, modify, and distribute it as per your requirements.

---
**Author:** Taniya Sirohi 
**GitHub Repository:** https://github.com/taniyasirohi/Radar.git

