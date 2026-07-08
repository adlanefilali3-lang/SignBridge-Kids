# System Architecture

## Overview

The SignBridge Kids system consists of a smart glove, a BBC micro:bit, and a mobile application.

## Data Flow

Smart Glove
    │
    ▼
Flex Sensors + MPU6050
    │
    ▼
ADS1115
    │
    ▼
BBC micro:bit
    │
Bluetooth
    │
    ▼
Mobile Application
    │
    ├── Text Translation
    ├── Speech Output
    └── Learning Mode

## Description

- Flex Sensors detect finger bending.
- MPU6050 detects hand orientation.
- ADS1115 converts analog signals to digital values.
- BBC micro:bit processes the data and sends it via Bluetooth.
- The mobile application displays the translated text, plays audio, and provides learning activities.
