# Long Range Lights Control Project

This project aims to control long-range lights on a vehicle. Four lights are connected to a relay board controlled by an ESP8266 microcontroller: [Relay Board](https://fr.aliexpress.com/item/1005002928488099.html).

A second board, "ESP3-CYD" [ESP3-CYD Board](https://fr.aliexpress.com/item/1005004971720824.html), allows controlling the lights through a touchscreen graphical interface:

- Activate/Deactivate lights individually
- Activate a preconfiguration of the lights
- Control lighting effects

## Future Development

- Activation of a preconfiguration via GPIO (using optocouplers to control the input with 12V/24V)
- Information feedback from a Victron solar controller via the VE.Direct interface


## LightsControl-CYD

### Overview

`LightsControl-CYD` is a project designed for the ESP32 microcontroller. It includes functionalities for controlling lights through a touchscreen interface and MQTT communication.

### Building and Uploading

To build and upload the project to the ESP32, use the following command:

```sh
pio run --target upload
```
### Dependencies
The project depends on several libraries, which are specified in the platformio.ini file:

- XPT2046_Touchscreen
- lvgl
- TFT_eSPI
- ESPAsyncWebServer
- AsyncTCP
- ElegantOTA
- AsyncMqttClient-esphome

## RelaysBoard

### Overview
RelaysBoard is a project designed for the ESP8266 microcontroller. It includes functionalities for controlling relays through MQTT communication.

### Building and Uploading
To build and upload the project to the ESP8266, use the following command:

```sh
pio run --target upload
```

### Dependencies
The project depends on several libraries, which are specified in the platformio.ini file:

- ElegantOTA
- WebSerial
- AsyncMqttClient-esphome

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.