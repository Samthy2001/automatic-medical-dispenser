# Automatic Medicine Dispenser

<img width="1983" height="793" alt="ChatGPT Image Sep 30, 2026, 02_28_41 AM" src="https://github.com/user-attachments/assets/ada9c385-3284-47dc-8e29-fdf56c4d686f" />

## Overview

The **Automatic Medicine Dispenser** is an embedded healthcare automation system developed to improve medication management by automatically dispensing pills according to predefined schedules.

The system is designed to assist users by providing accurate medication timing, controlled pill dispensing, and notification features.

The project integrates **embedded systems, automation, real-time control, and IoT communication** using an **Arduino Mega 2560**, **RTC DS3231**, **servo motor-based dispensing mechanism**, and **ESP8266 wireless communication module**.

The system allows users to configure medication schedules through a keypad interface, displays information through an LCD module, and provides visual, audio, and remote notifications during dispensing operations.

---

# Project Objectives

- Develop an automated medicine dispensing system.
- Dispense medication according to scheduled times.
- Reduce missed medication and human errors.
- Improve medication management for elderly and chronic patients.
- Provide a user-friendly interface for schedule configuration.
- Implement remote notification capabilities.
- Demonstrate healthcare automation using embedded systems.

---

# System Architecture and Data Flow

The system consists of multiple modules including:

- User Input Module
- Control and Processing Module
- Real-Time Clock Module
- Medicine Dispensing Module
- Display Module
- Alert Module
- Wireless Communication Module
- Power Supply Module


<img width="1536" height="1024" alt="ChatGPT Image Sep 30, 2026, 02_29_42 AM" src="https://github.com/user-attachments/assets/4d1157cd-6f5b-41c7-93d8-1fdd3e2d4ee9" />

## Data Flow

```
                User Input
              (4x4 Keypad)
                    |
                    ↓
            Arduino Mega 2560
          (Processing & Control)
                    |
        ----------------------------
        |            |             |
        ↓            ↓             ↓

    RTC DS3231    LCD Display   ESP8266
   Time Control   Information   Communication
        |
        ↓
 Medication Schedule Check
        |
        ↓
 Servo Motor Control
        |
        ↓
 Medicine Dispensing Mechanism
        |
        ↓
 Medicine Collection Tray

                    |
                    ↓

          LED + Buzzer Alert

                    |
                    ↓

          Remote Notification
          (User / Caregiver)
```

---

# Hardware Components

| Component | Purpose |
|---|---|
| Arduino Mega 2560 | Main control and processing unit |
| RTC DS3231 Module | Accurate real-time scheduling |
| SG90 Servo Motors | Control medicine dispensing mechanism |
| 4x4 Keypad | User input and schedule configuration |
| 16x2 LCD Display | Display medication information |
| ESP8266 Module | Wireless notification system |
| LED Indicator | Visual alert |
| Buzzer | Audio alert |
| Buck Converter | Voltage regulation |
| Mechanical Frame | System structure |
| Medicine Containers | Storage compartments |

---

# Software Technologies

- Arduino IDE
- Embedded C/C++
- I2C Communication
- SPI Communication
- Serial Communication
- EEPROM Data Storage


---

# Working Principle


## 1. User Schedule Setup

The user enters medication details through the 4x4 keypad.

The system allows configuration of:

- Medicine selection
- Dispensing time
- Dosage information


---

## 2. Real-Time Monitoring

The RTC DS3231 continuously tracks the current time.

The Arduino Mega compares the current time with the stored medication schedule.


---

## 3. Medicine Dispensing

When the scheduled time is reached:

1. Arduino sends control signals to the servo motor.
2. The servo rotates the dispensing gate.
3. Required pills are released into the collection tray.


---

## 4. Display and Alerts

After dispensing:

- LCD displays medication information.
- LED provides visual indication.
- Buzzer provides audio notification.


---

## 5. Remote Notification

The ESP8266 module sends dispensing information to users or caregivers through wireless communication.


---

# Main Features


## Automatic Scheduled Dispensing

The system automatically releases medication at predefined times.


## Multiple Medicine Storage

The dispenser contains multiple medicine compartments controlled by individual servo motors.


## User Interface

The keypad and LCD allow easy medication schedule configuration and monitoring.


## Alert System

LED and buzzer provide immediate notification when medication is dispensed.


## Remote Monitoring

ESP8266 enables wireless notification of dispensing activities.


---

# Medicine Dispensing Mechanism

The system uses multiple medicine containers with servo-controlled dispensing gates.

Each servo motor controls a separate medicine compartment.

The dispensing process includes:

1. Selecting the correct medicine container.
2. Activating the corresponding servo motor.
3. Opening the dispensing gate.
4. Releasing pills into the collection tray.


---

# System Workflow

```
System Start

      ↓

Initialize Arduino Mega

      ↓

Load Medication Schedule

      ↓

Read RTC Time

      ↓

Compare Current Time

      ↓

Medication Time Reached?

      ↓

Activate Servo Motor

      ↓

Dispense Medicine

      ↓

Update LCD Display

      ↓

Activate LED + Buzzer

      ↓

Send ESP8266 Notification

      ↓

Continue Monitoring
```

---

# My Contribution

- Designed the automatic medicine dispensing concept.
- Integrated Arduino Mega control architecture.
- Developed servo motor control logic.
- Integrated RTC scheduling system.
- Implemented keypad and LCD user interface.
- Worked on ESP8266 communication.
- Tested dispensing mechanism.
- Integrated hardware and software components.

---

# Project Output

The developed prototype demonstrates:

- Automated medication dispensing.
- Scheduled medicine management.
- Embedded system control.
- User interaction through keypad and LCD.
- Audio and visual alerts.
- Wireless notification capability.


---

# Advantages

- Reduces missed medication.
- Improves medication scheduling.
- Minimizes manual effort.
- Provides accurate dispensing timing.
- Supports elderly and chronic patients.
- Low-cost healthcare automation solution.


---

# Challenges

- Servo motor calibration.
- Accurate pill dispensing.
- Mechanical alignment.
- Stable power management.
- Reliable wireless communication.
- Integration of multiple modules.


---

# Future Improvements

- Mobile application integration.
- Cloud-based medication monitoring.
- AI-based medication recognition.
- Voice assistant support.
- Camera-based pill verification.
- Patient health record integration.


---

# Repository Structure

```
automatic-medicine-dispenser

│
├── README.md
├── LICENSE
│
├── images
│   ├── banner.png
│   └── system-architecture.png
│
├── Arduino_Code
│   └── Medicine_Dispenser_Code.ino
│
├── Circuit_Diagram
│
├── Documentation
│
└── Results
```

---

# Technologies Used

- Arduino Mega 2560
- RTC DS3231
- ESP8266
- Servo Motors
- LCD Display
- Keypad Interface
- Embedded C/C++
- IoT Communication
- Automation
- Healthcare Technology


---

# Author

**Samthy Shuaib**

Mechatronics Engineering Student

Interested in:

- Robotics
- Embedded Systems
- Automation
- IoT
- Intelligent Systems


GitHub:

https://github.com/Samthy2001
