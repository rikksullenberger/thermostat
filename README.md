ESPHome Thermostat HVAC Controller (ESP32-S3-Relay-6CH)
This project configures an ESPHome-based thermostat and HVAC controller using the Waveshare ESP32-S3-Relay-6CH board. It provides dual-point climate control, system runtime protections, Home Assistant integration, and visual relay feedback using an onboard WS2812 RGB LED.

Note: This configuration requires ESPHome version 2025.4.0 or newer. It may work on earlier versions, but it is untested.

The information on the Waveshare ESP32-S3-Relay-6CH board can be found at : https://www.waveshare.com/wiki/ESP32-S3-Relay-6CH
It can be found on Amazon for a decent price, Or Waveshare directly.

🚀 Features
🌡️ Dual-point thermostat with heat/cool mode

📉 Runtime protection (minimum on/off times)

🧠 Preset modes (Home, Comfort, Sleep, Away, OverCool, Warm Up)

📲 Integration with Home Assistant

🌐 Web UI and OTA updates

💡 RGB LED status indicator

📡 Remote temperature & humidity sensors from Home Assistant

🔧 Hardware
🧩 Board: ESP32-S3-Relay-6CH
Processor: ESP32-S3

Relays: 6 isolated relays (10A 250V AC / 10A 30V DC)

LED Indicator: WS2812 RGB LED on GPIO38

Connectivity: Wi-Fi + USB-C

Power: 7–36V DC (via terminal) or 5V via USB-C

Enclosure: DIN rail mountable ABS case

⚙️ GPIO Pin Mapping
Relay Function	Channel	GPIO Pin
Fan	CH1	GPIO1
Low Heat (W1)	CH2	GPIO2
High Heat (W2)	CH3	GPIO41
Cool (Y1)	CH4	GPIO42
Unused	CH5	GPIO45
Unused	CH6	GPIO46
RGB Status LED	-	GPIO38
📐 Diagrams & Resources
🖼️ Wiring Diagram & Dimensions

📑 Schematic PDF

🔌 ESPHome Devices Page

⚙️ YAML Features Overview
📡 Wi-Fi & API
Static IP support

OTA updates

Improv Serial and AP fallback

🌡️ Climate Control
Dual-point thermostat (heat/cool)

Configurable temperature step size

Minimum run/off times for safety

Preset modes with default temps

Fan-only, heat, cool, idle actions mapped to relays

RGB LED feedback for each HVAC mode

📈 Diagnostics
Wi-Fi signal strength (dBm and %)

Connected SSID, IP, MAC address

Firmware version

🔄 Relay Control
Individual GPIO-based relay controls

Status binary sensor

Restart, Safe Mode, and (disabled) Factory Reset buttons

📥 Installation
Flash the device using ESPHome or ESPHome Web.

Add Wi-Fi credentials using Improv or YAML.

Integrate into Home Assistant via the ESPHome integration.

Adjust the climate entity settings in Home Assistant as needed.

📚 Credits
YAML maintained and tested by [Your Name or Handle]

Hardware by Waveshare

Built using ESPHome

📜 License
MIT License

For contributions or issues, please open a GitHub Issue or submit a pull request.

Happy automating! 🏡
