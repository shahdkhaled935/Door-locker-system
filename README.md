# 🔐 Door Locker Security System (Embedded Systems Project)

## 📌 Overview
The Door Locker Security System is a secure embedded system implemented using two ATmega32 microcontrollers.  
The system provides password-based authentication to control a door lock mechanism with safety and alarm features.

---

## 🧠 System Architecture
The system follows a layered architecture and is divided into two ECUs:

### 🟦 HMI_ECU (Human Machine Interface)
- ATmega32 Microcontroller (8MHz)
- 2x16 LCD Display
- 4x4 Keypad
- Responsible for user interaction
- Sends and receives data via UART

### 🟥 CONTROL_ECU (System Controller)
- ATmega32 Microcontroller (8MHz)
- EEPROM (I2C Communication)
- DC Motor (Door control using PWM)
- Buzzer (Alarm system)
- Responsible for system logic, authentication, and control actions

---

## ⚙️ System Features
- Password creation and confirmation system
- Secure password storage using external EEPROM
- UART communication between two microcontrollers
- Door unlocking and locking using DC motor
- Password change functionality
- 3-attempt security system with alarm activation
- System lock with buzzer for 1 minute after failed attempts

---

## 🔌 Drivers Implemented
- GPIO Driver  
- LCD Driver  
- Keypad Driver  
- UART Driver  
- I2C Driver  
- EEPROM Driver  
- DC Motor Driver (PWM using Timer0)  
- Buzzer Driver  
- Timer1 Driver (interrupt-based timing)

---

## 🧩 Technical Highlights
- Multi-MCU communication using UART
- Interrupt-based timer implementation
- Modular driver-based architecture
- EEPROM non-volatile memory handling
- PWM motor control for door mechanism

---

## 📷 Hardware Design
The system was designed using Proteus schematic.

![System Design](schematic.png)

---

## 👩‍💻 My Contribution
- Designed and implemented system drivers
- Developed communication protocol between MCUs
- Implemented security logic and password handling
- Integrated hardware components (LCD, Keypad, Motor, EEPROM)

---

## 📌 Notes
This project was developed as part of an Embedded Systems final project focusing on real-world security system design and microcontroller communication.
