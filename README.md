# Arduino-Ultrasonic-Parking-Sensor
Arduino-based ultrasonic parking sensor using HC-SR04 and LED distance indication
Arduino Ultrasonic Parking Sensor 🚗

An Arduino-based parking sensor that uses an HC-SR04 ultrasonic sensor to detect the distance between the vehicle and an obstacle and provides visual distance indication using LEDs.

📌 Project Overview

This was one of my first electronics projects, built to understand how an ultrasonic sensor can be interfaced with a microcontroller for a practical application.

The system continuously measures the distance of an obstacle in front of the sensor and changes the LED indication according to the detected distance.

🛠️ Components Used

- Arduino Nano
- HC-SR04 Ultrasonic Sensor
- 3 × LEDs
- 3 × Current-limiting resistors
- Breadboard
- Jumper wires
- USB cable / power supply

⚙️ Working Principle

The HC-SR04 sends an ultrasonic pulse and measures the time taken for the reflected pulse to return.

The Arduino uses this time to calculate the approximate distance:

Distance = (Time × Speed of Sound) / 2

The division by 2 is required because the ultrasonic wave travels to the obstacle and then returns to the sensor.

The measured distance is then used to control the LEDs.

🔌 Main Connections

Component| Arduino Pin
HC-SR04 Trig| Digital pin
HC-SR04 Echo| Digital pin
LED 1| Digital pin
LED 2| Digital pin
LED 3| Digital pin
VCC| 5V
GND| GND

«Exact pin assignments are available in the Arduino source code.»

💡 Features

- Ultrasonic distance measurement
- Real-time obstacle detection
- LED-based distance indication
- Simple and low-cost hardware
- Arduino-based implementation

🧪 Testing

The project was tested on a breadboard with different obstacle distances.

During testing, variations in ultrasonic readings were observed. This helped me understand that real-world sensor measurements are not always perfectly stable and may require techniques such as averaging and threshold handling.

📚 What I Learned

- Basics of ultrasonic distance measurement
- Interfacing HC-SR04 with Arduino
- Digital GPIO control
- LED control using distance thresholds
- Breadboard circuit assembly
- Debugging hardware and wiring problems
- Understanding sensor measurement fluctuations
- Documenting an electronics project on GitHub

🚀 Future Improvements

- Add averaged sensor readings for more stable measurements
- Add a buzzer for audio warning
- Improve the distance-threshold logic
- Add an LCD/OLED display
- Design a compact PCB version

👨‍💻 Author

Pratham Palande

Electronics & Telecommunication Engineering Student

---

⭐ This project was built as a hands-on learning project to strengthen practical electronics and embedded-system fundamentals.
