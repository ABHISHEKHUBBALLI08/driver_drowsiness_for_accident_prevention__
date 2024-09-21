Driver Safety and Obstacle Detection System 🚗🛑
Overview
This project implements a Driver Safety and Obstacle Detection System designed to monitor driver drowsiness and detect nearby obstacles to improve road safety. The system uses sensors to track the driver’s eye closure and obstacle proximity, triggering alerts and taking action if necessary.

Features:
Drowsiness Detection: Alerts when the driver’s eyes remain closed.
Obstacle Detection: Detects nearby obstacles using an ultrasonic sensor.
Buzzer Alerts: Provides auditory warnings for drowsiness or obstacles.
Motor Control: Stops the vehicle’s motor if the driver remains drowsy or an obstacle is too close.

Technologies Used:
Arduino IDE
Ultrasonic Sensor (HC-SR04)
Buzzer
Relay Module
Eye Sensor (or equivalent for drowsiness detection)
Project Components

Component	Description:
Sinput (Pin 10)	Eye sensor input for drowsiness detection.
Buzzer (Pin 3)	Alerts driver with sound warnings.
Relay (Pin 5)	Controls motor (on/off).
Trig Pin (Pin 7)	Trigger pin for ultrasonic sensor.
Echo Pin (Pin 6)	Echo pin for ultrasonic sensor to measure distance.

Circuit and Pin Setup:
Eye sensor connected to Pin 10 (Sinput).
Buzzer connected to Pin 3 for audible alerts.
Relay connected to Pin 5 for motor control.
Ultrasonic Sensor connected as follows:
Trig Pin to Pin 7.
Echo Pin to Pin 6.

How the System Works:
Eye Monitoring: The system checks if the driver's eyes are closed through the eye sensor.
Obstacle Detection: The ultrasonic sensor monitors obstacles around the vehicle.
If an obstacle is within 10 cm, the motor stops, and the buzzer is activated.
If the obstacle is within 30 cm but more than 10 cm, only the buzzer is activated as a warning.
Motor Control: The relay ensures the motor stops when drowsiness or close obstacles are detected.
