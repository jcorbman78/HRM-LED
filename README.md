# HRM-LED
Heart Rate Monitor LED
1. BLE Heart Rate Data Acquisition:

BLE Library: You'll need a BLE library for the ESP32. The "ESP32 BLE Arduino" library is commonly used.
Heart Rate Service: The heart rate monitor will expose a heart rate service with a heart rate measurement characteristic.
Characteristic Reading: Your ESP32 code will need to scan for BLE devices, connect to your heart rate monitor, discover the heart rate service and characteristic, and read the heart rate value.
2. Heart Rate Zone Mapping:

Create a function that takes the heart rate value as input and returns the corresponding zone.
Use if-else or switch statements to map the heart rate to the correct zone.
3. LED Color Mapping:

Assign a color to each heart rate zone. For example:
Z1: Green
Z2: Blue
Z3: Yellow
Z4: Orange
Z5: Red
Create a function that takes the zone number as input and returns the corresponding RGB color value.
4. LED Control:

Use the Adafruit NeoPixel library to set the color of the WS2812B LED strip based on the heart rate zone.
