# Cybersecurity : CSN150

Student: Rahmman Sadman

Project: ESP32-CAM Wi-Fi Scanner

## Purpose
The purpose of this project is to set up the ESP32-CAM using Arduino IDE and learn how to scan nearby Wi-Fi networks. I will also document the steps I followed, including any problems and how I fixed them.

## Equipment
* [ESP32Cam](https://www.amazon.com/Aideepen-ESP32-CAM-Bluetooth-ESP32-CAM-MB-Arduino/dp/B08P2578LV/ref=sr_1_3?crid=4FY0ECFW0ZX7&keywords=ESP32+Cam&qid=1678902050&sprefix=esp32+cam%2Caps%2C240&sr=8-3)

* [USB Micro Data Cable](https://www.amazon.com/AmazonBasics-Male-Micro-Cable-Black/dp/B0711PVX6Z/ref=sr_1_1_sspa?keywords=micro+usb+data+cable&qid=1678902214&sprefix=Micro+USB+data+%2Caps%2C89&sr=8-1-spons&psc=1&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUFaU0NaUVZHU1RFUlAmZW5jcnlwdGVkSWQ9QTA3NTA4MDVFVERCS01HVlgxM1YmZW5jcnlwdGVkQWRJZD1BMDE4NTE1NTIwWUdONkdWSzU1M1Amd2lkZ2V0TmFtZT1zcF9hdGYmYWN0aW9uPWNsaWNrUmVkaXJlY3QmZG9Ob3RMb2dDbGljaz10cnVl)

## Links to documentation and tools

##### Video 1: 

##### Other Links: 
- [Arduino IDE Download](https://www.arduino.cc/en/software/)

##### AI GPTs used
- ChatGPT: I used ChatGPT to help me understand the lab instructions and organize my documentation.

## Steps I followed
1. I opened the GitHub repository provided by my professor.
2. I clicked Fork to create my own copy of the repository.
3. I added my name to the repository name.
4. I opened the README.md file to edit the documentation.
5. I added my name, project title, purpose, and Arduino IDE download link.
6. I downloaded and installed Arduino IDE 2.3.10 on my computer.
7. I opened Arduino Preferences and added the ESP32 board manager URL.
8. I opened Boards Manager and installed ESP32 by Espressif Systems version 3.3.12.
9. I selected AI Thinker ESP32-CAM as my board.
10. I opened the WiFiScan example from the Arduino examples menu.
11. I clicked Verify to check the code, and it compiled without errors.

## Problems and Solutions
1. Problem: At first, I had trouble finding where to create my own GitHub fork.
   Solution: I opened the Fork dropdown menu and selected Create a new fork.

### Example Problems From Professor's Template (Not My Errors)
**Problem:** E (485) camera: Camera probe failed with error 0x105(ESP_ERR_NOT_FOUND)
Camera init failed with error 0x105
**Solution:**

### Example Problem
**Problem:** Arduino code will not load on ESP32 Cam.
**Solution:** Camera drivers were incorrect I needed to install the driver: [https://www.wch-ic.com/downloads/CH341SER_ZIP.html](https://github.com/martin-ger/esp32_nat_router).  I used file, "CH341SER.ZIP" and it worked.

## Final Report

For this lab, I created my own GitHub repository by forking my professor's template. I updated the README file with my project information and documented the steps I followed.

I also installed Arduino IDE 2.3.10 and added the ESP32 board package by Espressif Systems. After selecting the AI Thinker ESP32-CAM board, I opened the WiFiScan example and verified the code. The program compiled successfully without any errors.

I learned how to use GitHub to document my work and how to prepare Arduino IDE for an ESP32 project. I have not tested the Wi-Fi scanner on a physical ESP32-CAM yet.
