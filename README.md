# IOT_controlled_Boat



This project enables control of two DC motors (forward/reverse) and a servo motor using the Blynk IoT platform and an ESP32 board. It uses virtual pins for motor direction and a slider for servo position control.

## 📱 Features

- 🔌 **Wi-Fi Connectivity** via ESP32
- 🕹️ **Motor Control** using Blynk buttons (Forward and Reverse)
- 🎛️ **Servo Angle Control** via Blynk slider (0–180 degrees)
- 📲 **Remote Operation** using Blynk mobile app

## 🧰 Hardware Used

- ESP32 Dev Board  
- L298N or similar motor driver (for IN1–IN4 control)
- Servo Motor (connected to GPIO 18)
- Two DC Motors  
- Power Supply  
- Smartphone with Blynk App
- Buck Converter/Voltage Regulator(for ESP32)
- Plastic chassis(eg..pepsi bottle) for buoyancy
- Waterproofing(Sealant,hot glue,tape)

## 🧑‍💻 Software Used

- [Arduino IDE](https://www.arduino.cc/en/software)
- [Blynk IoT Platform](https://blynk.io/)
- Blynk Libraries (`BlynkSimpleEsp32`, `ESP32Servo`, etc.)

## 🔧 Wiring Overview

| ESP32 GPIO | Description        |
|------------|--------------------|
| 4 (IN1)    | Motor A - Input 1  |
| 5 (IN2)    | Motor A - Input 2  |
| 12 (IN3)   | Motor B - Input 1  |
| 13 (IN4)   | Motor B - Input 2  |
| 18         | Servo Signal Pin   |

> Note: Make sure the motor driver and servo motor are powered appropriately.

## 📲 Blynk Configuration

In the **Blynk app**, set up the following widgets:

- **Button (V1):** Motor Forward
- **Button (V2):** Motor Reverse
- **Slider (V3):** Servo Position (0 to 180)

### Blynk Template Info (Update with yours if different):

```cpp
#define BLYNK_TEMPLATE_ID "TMPL3-4iXBqaV"
#define BLYNK_TEMPLATE_NAME "DM"
#define BLYNK_AUTH_TOKEN "V8385YNtixTCjmD8ncExwCMhsaVZcc_i"
