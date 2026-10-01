# AEROSHIELD: Counter-UAV Intelligence Challenge

## Overview

A ground control station is monitoring an unknown UAV operating inside a controlled airspace.

Teams are provided with a simulated control panel containing multiple sensor feeds and telemetry sources. Using the available information, teams must develop their own algorithm/system to analyze UAV behavior and make intelligent decisions.

The environment provides simulated real-time data similar to what a UAV monitoring system may receive.

---

# Control Panel Sensors & Data Sources

## 1. Radar Tracking System

The radar provides real-time information about detected aerial objects.

Example data:

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
