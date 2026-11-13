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


---

# Lab: ESP32 Camera

**Student:** Rahmman Sadman  
**Class:** CSN 150 D03  
**Project:** ESP32-CAM Camera Firmware


## Purpose

The purpose of this lab was to install the camera firmware on my ESP32-CAM using Arduino IDE. I also learned how to connect the camera to my Wi-Fi network and view live video through a web browser.


## Equipment

- ESP32-CAM (AI Thinker)
- USB data cable
- Computer running Windows 11
- Arduino IDE 2.3.10
- Google Chrome
- 2.4 GHz Wi-Fi network


## Steps I Followed

1. I connected my ESP32-CAM to my computer using a USB cable.
2. I opened Arduino IDE 2.3.10.
3. I opened the CameraWebServer example from the ESP32 camera examples.
4. I selected AI Thinker ESP32-CAM as my board and COM3 as my port.
5. I opened board_config.h and selected CAMERA_MODEL_AI_THINKER.
6. I entered my Wi-Fi information in the CameraWebServer code.
7. I checked the board settings and uploaded the camera firmware.
8. I opened Serial Monitor and set the baud rate to 115200.
9. I pressed the reset button on my ESP32-CAM.
10. The Serial Monitor showed that the camera connected to Wi-Fi successfully.
11. I opened the camera's IP address in Google Chrome.
12. I clicked Start Stream and was able to see live video from my ESP32-CAM.
13. I took a screenshot of the camera software with the camera pointed at myself.


## Problems and Solutions

1. Problem: The CameraWebServer example had the wrong camera model selected.
   Solution: I opened board_config.h and changed the camera model to AI Thinker ESP32-CAM.

2. Problem: At first, the Serial Monitor showed a Wi-Fi connection warning.
   Solution: After restarting the ESP32-CAM, it successfully connected to my Wi-Fi network and displayed the camera IP address.


## Final Report

In this lab, I was able to get my ESP32-CAM working using Arduino IDE. I uploaded the camera firmware and connected the camera to my Wi-Fi network. After opening the IP address in Google Chrome, I was able to see live video from the camera.

I learned how to set up the camera, use Serial Monitor to find its IP address, and access the camera through a web browser. Overall, the lab was successful because the camera worked and I was able to take a screenshot of the live video.
