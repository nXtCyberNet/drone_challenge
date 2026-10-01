# AEROSHIELD: Counter-UAV Intelligence Challenge

## Overview

A ground control station is monitoring an unknown UAV entering a controlled airspace.

Teams are provided with a simulated control panel containing multiple sensor feeds. Using the available information, teams must design their own algorithm/system to analyze the UAV behavior and make decisions.

The challenge environment simulates a real-time UAV monitoring system.

---

# Control Panel Sensors

## 1. Radar System

The radar provides real-time tracking information of detected aerial objects.

Data provided:

```json
{
    "track_id": 7,
    "distance": 420,
    "angle": 36,
    "altitude": 80,
    "speed": 14,
    "heading": 120,
    "confidence": 0.87
}
