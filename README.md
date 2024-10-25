# USB_to_TTL_Converter
USB Serial Port to CMOS Logic-Level Serial Port converter.

# Custom USB to TTL Converter (CP2102)

This project involves building a custom USB to TTL converter using the CP2102 chipset. The converter allows communication between a USB port and TTL-level serial devices, ideal for embedded systems, microcontrollers, or other electronics projects.

## Features

- **Chipset:** CP2102 USB-to-UART Bridge
- **Supported Baud Rates:** 300bps to 1Mbps
- **Operating Voltage:** 3.3V or 5V (adjustable)
- **USB Interface:** Standard USB Type-A/B
- **TTL Levels:** Supports both 3.3V and 5V devices
- **Compact Design:** Small footprint for easy integration
- **Plug & Play:** No external power supply needed

## Requirements

- **CP2102 Drivers:**
  - Windows: [Download from Silicon Labs](https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers)
  - Linux: Typically pre-installed, or install via package manager.
  - macOS: [Download from Silicon Labs](https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers)
  
- **Hardware:**
  - CP2102 chip
  - USB connector (Type-A/B)
  - Capacitors and resistors (refer to datasheet)
  - Header pins for TTL connection

## Pinout

| Pin  | Description     |
|------|-----------------|
| TXD  | Transmit Data    |
| RXD  | Receive Data     |
| GND  | Ground           |
| VCC  | Power Supply (3.3V or 5V) |
| DTR  | Data Terminal Ready |
| RTS  | Ready to Send    |

## Setup & Usage

### 1. Install CP2102 Driver
- Follow the instructions for your operating system to install the CP2102 driver (links provided above).

### 2. Connect the Converter
- Connect the USB side of the converter to your computer.
- Connect the **TXD**, **RXD**, and **GND** pins to the corresponding pins of your TTL device. Ensure the **VCC** level is correct for your target device (3.3V or 5V).

### 3. Configure Serial Communication
- Use a serial communication software (e.g., [PuTTY](https://www.putty.org/) or [Tera Term](https://ttssh2.osdn.jp/index.html.en)) to interact with your device.
- Select the correct COM port (visible in Device Manager or equivalent tool).
- Configure baud rate and other serial settings to match your device requirements.

### 4. Testing
- Send and receive data to/from your TTL device using the serial monitor software.
- If using a microcontroller, ensure your serial code matches the configuration.

## Schematics

Below is the basic schematic for the USB to TTL converter:




![2](https://github.com/user-attachments/assets/a5468c34-2413-47e3-8633-976caf87c56d)
![3](https://github.com/user-attachments/assets/00a9abe1-3383-47c1-a605-71058c218d13)
![Schematic](https://github.com/user-attachments/assets/4d903c8b-ef05-4ec5-a92b-33deb477d3d5)
