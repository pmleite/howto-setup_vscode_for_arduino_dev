# How to setup VSCODE for Arduino Develloping.

## Pre-requisites

- [x] Arduino IDE
- [x] Visual Studio Code
- [x] Arduino Extension for VSCODE
- [x] Arduino CLI
  
- [x] Arduino Board
- [x] USB Cable
  
## Steps to follow

1. Install Arduino IDE from [here](https://www.arduino.cc/en/software).
2. Install Visual Studio Code from [here](https://code.visualstudio.com/download).
3. Install Arduino Extension for VSCODE from [here](https://marketplace.visualstudio.com/items?itemName=vsciot-vscode.vscode-arduino).
4. Install Arduino CLI from [here](https://github.com/arduino/arduino-cli)

## c_cpp_properties.json 

Use those rules in the file (Linux Example)
The objective is to add the include PATHs of the default libraries of arduino

```json
{
    "configurations": [
        {
            "name": "Arduino",
            "includePath": [
                "${workspaceFolder}/**",
                "/home/<YOUR HOMEFOLDER>/.arduino15/packages/arduino/hardware/avr/1.8.6/cores/arduino",
                "/home/<YOUR HOMEFOLDER>/.arduino15/packages/arduino/hardware/avr/1.8.6/variants/mega",
                "/home/<YOUR HOMEFOLDER>/.arduino15/packages/arduino/hardware/avr/1.8.6/libraries/EEPROM/src",
                "/home/<YOUR HOMEFOLDER>/.arduino15/packages/arduino/tools/avr-gcc/7.3.0-atmel3.6.1-arduino7/lib/gcc/avr/7.3.0/include",
                "/home/<YOUR HOMEFOLDER>/.arduino15/packages/arduino/tools/avr-gcc/7.3.0-atmel3.6.1-arduino7/lib/gcc/avr/7.3.0/include-fixed",
                "/home/<YOUR HOMEFOLDER>/.arduino15/packages/arduino/tools/avr-gcc/7.3.0-atmel3.6.1-arduino7/avr/include"
            ],
            "compilerPath": "C:/Program Files (x86)/Arduino/hardware/tools/avr/bin/avr-gcc.exe",
            "cStandard": "c11",
            "cppStandard": "c++17",
            "intelliSenseMode": "gcc-x64"
        }
    ],
    "version": 4
}
```

## Rules to create a project

The name of the folder must be the same as the name of the .ino file
