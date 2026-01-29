# 🐾 Happy Paws: Automatic Pet Feeder
👥 Contributors
      Betül ATALAY
      Ömer YANMAZ

Happy Paws is an advanced embedded system project designed to automate pet feeding routines, addressing the challenges of busy lifestyles and pet health concerns like obesity or anxiety.Developed as part of the ELE 417 - Embedded System Design Project at Hacettepe University.
![IMG-20251222-WA0004 (1)](https://github.com/user-attachments/assets/e2eec2fa-3b9e-4132-aa39-1e0e9ebbbf12)

🏗 System Architecture
The project utilizes a dual-MCU architecture to separate the high-level user interface from the low-level actuation logic.
Master MCU (STM32F746): Handles the LVGL-based graphical user interface and overall system logic.
Slave MCU (STM32F407): Manages the motor control and actuation logic.
Timekeeping: DS3231 RTC module connected via I2C for precise real-time scheduling.
Inter-board Communication: Data transfer between MCUs via UART.
DM-S0306D 360° Continuous Digital Servo: Used to drive the feeding mechanism. Unlike standard servos, it allows for infinite rotation in both directions, which is essential for the screw-driven dispensing system.

💻 Software Implementation
🎨 User Interface (LVGL)
The interface is built using the LVGL library, featuring a modern and responsive design:
Main Dashboard: The home screen provides at-a-glance information including current time, the next scheduled feeding, and dynamic status messages like "Almost time!".
Interactive Controls: A prominent "Instant Treat" button, designed as a clickable paw-print image, allows for manual dispensing outside of the schedule.
![WhatsApp Image 2025-11-29 at 22 45 52 (1)](https://github.com/user-attachments/assets/a1a01964-2ad4-4e1c-aa1d-02f2be48ffa3)

Settings Screen

Scheduling System: A dedicated menu where users can set specific feeding times using roller widgets for hours and minutes.
![WhatsApp Image 2025-12-08 at 21 04 28](https://github.com/user-attachments/assets/42e28655-272a-4973-90f9-ece7faa425b2)

Portion Management: Users can customize the amount of food for each scheduled slot, with options ranging from 10g to 50g via dropdown menus.
![WhatsApp Image 2025-12-08 at 21 05 46](https://github.com/user-attachments/assets/ad997afe-6a9c-4705-8ac9-23573e86f83e)

Manual Synchronization: Through a dedicated "Time" settings screen, users can set the current hour and minute using intuitive roller widgets.
![WhatsApp Image 2025-12-08 at 21 06 16 (1)](https://github.com/user-attachments/assets/63e853cc-c6b1-425d-a7d7-9ea5905b8e25)

📺 Demo
Watch the Happy Paws in action on YouTube:

▶️ Happy Paws - Presentation & Demo 



