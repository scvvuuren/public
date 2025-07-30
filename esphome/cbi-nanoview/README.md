# CBI Nanoview Energy Meter
Protocol Details : https://www.nanoview.co.za/protocol.html

Inspiration Projects : https://github.com/denvera/esp32-nanoview and http://silico.co.za/blog/2019/04/13/hacking-the-nanoview-with-a-rpi-zero-w/

The objective of this esphome project is to provide a simplified method to make the Nanoview Device Smart.
The protocol data are read and provided back as multiple sensors to Home Assistant.



Wiring

⚠️ WARNING: Electrical Shock Hazard ⚠️
Working with live power in your DB (Distribution Board) can expose you to severe electrical shock, which may result in serious injury or death.
Always switch off the mains power to your DB board before attempting any wiring or modifications. If you are unsure or uncomfortable performing this task, please request assistance from a qualified electrician.

````
NanoHub
├── Black Wire
│   (Cut and Splice Here)
│   └── [SPLICE POINT]
│       ├── To Tablet (Ground)
│       └── To ESP32 (Ground)
│
├── White Wire
│   (Cut and Splice Here)
│   └── [SPLICE POINT]
│       ├── To Tablet (Transmit Data)
│       └── To ESP32 (Receive Data)
│
├── Red Wire
│   └── To Tablet (Power)  <-- UNTOUCHED
│
└── Green Wire
    └── To Tablet (No Connection) <-- UNTOUCHED
````

Simply copy the yaml configuration to your esphome project configuration file and modify the substitutions to match your requirements.

ESPHome Web Interface

<img width="1829" height="575" alt="image" src="https://github.com/user-attachments/assets/97c55362-c7ed-43c4-a75d-1aa26c92dcc7" />

Home Assistant Integration

<img width="297" height="853" alt="image" src="https://github.com/user-attachments/assets/42d90140-9c0e-4993-9858-f6c2d8ca4b84" />

Home Assistant Device History

<img width="1609" height="372" alt="image" src="https://github.com/user-attachments/assets/23f0a777-1956-4100-bba0-c1f77126a09c" />

Energy Dashboard - Individual Device Energy over 1 Month

<img width="1373" height="418" alt="image" src="https://github.com/user-attachments/assets/64b151dc-5d74-4bec-9e8d-5f9b9796f11c" />

