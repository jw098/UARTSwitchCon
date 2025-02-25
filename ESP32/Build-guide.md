# How to Build for Windows


## Install ESP-IDF
https://docs.espressif.com/projects/esp-idf/en/stable/esp32/get-started/windows-setup.html

On Windows, you can use the installer. I recommend ensuring that the Command Prompt Desktop shortcut is checked during installation.

## Build
1. Clone this repo.
2. Open ESP-IDF terminal (you may use the Desktop shortcut created during installation)
3. In the terminal, change the directory to to the folder:

`cd [path to UARTSwitchCon]\UARTSwitchCon\ESP32\source\firmware`

4. Run in ESP-IDF terminal: `idf.py build`

## Flash onto device
5. Run in ESP-IDF terminal: `idf.py -p [PORT] flash`
    - Replace `[PORT]` with your ESP32 board's USB port name. e.g. COM5. You can find this using the Device Manager.
    - Sometimes the flash can fail without reason. If it fails, try running the flash command again.

## Connecting the ESP device to the Switch
Click the `BOOT` button on the ESP board. The controller should now show up in the `Change Grip/Order` menu.