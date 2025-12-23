# Pump Volume Test (ESP32-S3)

A small test program to control a pump via a MOSFET using an ESP32-S3 DevKit.

## Hardware
*   **Board**: ESP32-S3 DevKitC-1 (N16R8)
*   **Pump**: Connected to MOSFET module
*   **MOSFET Pin**: GPIO 4
*   **External Button**: GPIO 5 (to GND)
*   **Status LED**: Onboard WS2812 (GPIO 48)

## Functionality
1.  **Ready (Green)**: Waiting for input.
2.  **Active (Yellow)**: Pump pulses continuously (150ms ON / 850ms OFF).
3.  **Stopped (Red)**: Pump stopped. Waiting for restart.

## Controls
*   **External Button (GPIO 5)**: Toggles continuous pumping ON/OFF.
*   **Boot Button (GPIO 0)**: Triggers a single pump stroke (useful for precise volume measurement).

## Pinout Reference
*   [OceanLabz ESP32-S3 Pinout](https://www.oceanlabz.in/esp32-s3-devkit-pinout-reference/)
