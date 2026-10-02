# STM32-Based Ultrasonic Distance Measurement Using TIM2, UART and FreeRTOS

📌 Project Overview

This project is an STM32-based ultrasonic distance measurement system. It measures the distance between the ultrasonic sensor and an object using reflected ultrasonic waves.

🔧 Components Used

- STM32 Microcontroller
- Ultrasonic Sensor
- LED
- UART
- TIM2 32-bit Timer
- FreeRTOS

🔌 Ultrasonic Sensor Pins

- VCC – Power supply
- GND – Ground
- TRIG – Sends ultrasonic wave
- ECHO – Receives the reflected wave

⚙️ Working

1. The STM32 sends a trigger pulse to the ultrasonic sensor.
2. The sensor sends an ultrasonic wave towards the object.
3. The wave reflects back when it hits the object.
4. The ECHO pin receives the reflected wave.
5. TIM2 measures the Echo pulse duration.
6. STM32 calculates the distance using the time-of-flight principle.
7. The calculated distance is displayed through UART on the serial monitor.
8. FreeRTOS is used to manage the tasks.

📐 Distance Calculation

Distance = (Time × Speed of Sound) / 2

The value is divided by 2 because the measured time represents the to-and-fro travel of the ultrasonic wave.

💻 Software Used

- STM32CubeIDE
- STM32 HAL Library
- FreeRTOS
- Embedded C

🎯 Applications

- Object distance measurement
- Obstacle detection
- Embedded system learning
- Robotics and automation



Through this project, I gained hands-on experience with STM32, GPIO, TIM2 Timer, UART, Ultrasonic Sensor, FreeRTOS, and Embedded C programming.
