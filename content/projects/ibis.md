---
title: 'UTS Rocketry - Ibis Flight Computer'
date: 2024-06-18
draft: false
cover:
    image : "projects/ibis/cover.png"
    width : 100
---

Ibis is a full system flight computer that was designed for UTS Rocketry's 2024 rocket - Goana.

I was responsible for all the software and RF communications involved with the flight computer.

## Features

- 2 dual core esp32 MCUs
  - ESP32s3
  - i2c inter-chip communication

- Redundant GPS modules

- RFM95W LoRa RF module
  - 3km of downlink range

- exFat compatible SD data logging

- Dual recovery deployment
  - Drogue + Main parachute deployment
  - Customisable deployment delays and altitudes

- RTOS task management
  - Necessary for utilising all 4 cores effectively

- 11 DoF sensor measurements
  - 9 DoF IMU
    - xyz Acceleration
      - ±16 g
    - xyz Gyroscope
    - xyz Magnetometer
  - Barometer (BMP280)
    - Temperature
    - Pressure
  - High-g Accelerometer
    - ±120 g
