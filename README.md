# EventBoard – RTC-Driven Message Display System  

## 📌 Objective  
The **EventBoard** project is an embedded system built using the **LPC2148 ARM7 microcontroller**. Its main goal is to **automatically display predefined messages** on an LCD at scheduled times using the **RTC (Real-Time Clock)**.  

The system also provides:  
- A secure **Admin Mode** with keypad + password protection  
- Ability to edit RTC time and enable/disable messages  
- Temperature monitoring using **LM35 sensor**  

---

## 🖼️ Block Diagram  
*(See project PDF in Docs/ for full diagram)*  

---

## ⚙️ Hardware Requirements  
- LPC2148 Microcontroller  
- 16x2 LCD  
- Keypad  
- LEDs (Status Indication)  
- LM35 Temperature Sensor  
- Buzzer  

## 💻 Software Requirements  
- Embedded C  
- Keil µVision (C Compiler)  
- Flash Magic (for programming LPC2148)  

---

## 🔄 Project Workflow  
1. **Normal Mode**  
   - RTC time is continuously displayed.  
   - If the current time matches a scheduled message → message scrolls on LCD & Green LED turns ON.  
   - If no message → system displays RTC + Room Temperature & Red LED turns ON.  

2. **Admin Mode**  
   - Enter via **external switch interrupt**.  
   - Secure access via **password-protected keypad**.  
   - Allows user to **edit RTC time** and **select active messages**.

---

## 🚀 Features
- ✅ Real-Time Clock driven scheduling  
- ✅ Scrolling message display on LCD  
- ✅ Secure Admin Mode (password protected)  
- ✅ Temperature monitoring with LM35 sensor  
- ✅ LED status indication (Green = Active, Red = Idle)  

---

## 🎯 Applications
- 📌 College/School notice boards  
- 📌 Office event reminders  
- 📌 Automated lab schedules  
- 📌 Smart home display systems  
