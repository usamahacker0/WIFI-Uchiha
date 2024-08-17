# WiFi-Uchiha

WiFi-Uchiha is a project based on the ESP32 NodeMCU that allows you to create a WiFi deauther, jam WiFi stations and access points, and create fake WiFi access points. The project also includes a 1.3-inch OLED I2C display for real-time status updates and a local website for control and monitoring.

## Features
- **WiFi Deauther:** Jam specific WiFi stations and access points.
- **Fake WiFi Access Point:** Create and broadcast fake WiFi networks.
- **OLED Display:** 1.3-inch I2C OLED display for real-time status updates.
- **Local Website:** Control and monitor the device via a local web interface.

## Device Overview
![Device](device_image.jpg)
![IMG-20240817-WA0014](https://github.com/user-attachments/assets/9e7fd3d4-2eda-450d-a33e-0b7a60c556cf)

## Schematic
![Schematic](schematic_image.jpg)

![WIFI-Uchiha_Wiring](https://github.com/user-attachments/assets/c99e608f-44dd-4089-b9a2-d2ee95f97d2f)

## Local Web Control Page
![Web Control Page](web_control_page_image.jpg)

![Screenshot 2024-08-17 133918](https://github.com/user-attachments/assets/f28a2d9f-10b0-43f5-ba08-3ee8b1aa4758)
## Hardware Requirements
- ESP32 NodeMCU
- 1.3-inch OLED Display (I2C)
- Additional components as per your requirements

## Flashing the Firmware using ESPHome-Flasher

1. **Download the Firmware:**
   - Download the pre-compiled firmware file (`wifi-uchiha.bin`) from the [Releases]([https://github.com/usamahacker0/WIFI-Uchiha/blob/main/WIFI-Uchiha_2.0.bin]) section.

2. **Download ESPHome-Flasher:**
   - Download the ESPHome-Flasher tool from [ESPHome-Flasher Releases](https://github.com/esphome/esphome-flasher/releases).

3. **Flash the Firmware:**
   - Open ESPHome-Flasher.
   - Connect your ESP32 NodeMCU to your computer via USB.
   - Select the appropriate COM port.
   - Click on "Browse" and select the `wifi-uchiha.bin` file.
   - Click "Flash ESP" to upload the firmware to your ESP32.

4. **Connecting the OLED Display:**
   - Connect the OLED display to the ESP32 using I2C (SDA and SCL) as shown in the schematic.

5. **Accessing the Local Web Interface:**
   - Connect to the WiFi network created by the ESP32.
   - Open a web browser and go to `http://192.168.4.1` to access the control page.

## Usage
- **Deauth Mode:** Select a WiFi station or access point to jam.
- **Fake AP Mode:** Create a new fake WiFi access point with a custom SSID.
- **OLED Display:** View the status of the device and current operations.
## Disclaimer

This project is for **educational purposes only**. The use of WiFi deauthers and fake access points can be illegal and unethical in many regions. **Do not use this project to disrupt, interfere, or harm any legitimate WiFi networks.** The authors are not responsible for any misuse or damages caused by using this project.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
