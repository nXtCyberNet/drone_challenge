
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
```

Provided parameters:

- Object ID
- Distance from radar
- Direction angle
- Altitude
- Speed
- Heading
- Detection confidence
- Movement history
- Estimated trajectory

---

# 2. GPS Tracking Data

The system provides estimated UAV position information.

Example:

```json
{
    "latitude": 28.613,
    "longitude": 77.209,
    "altitude": 80,
    "accuracy": 5
}
```

Provided parameters:

- Current position
- Altitude
- Position accuracy
- Movement direction
- Previous positions
- Location updates

GPS data may contain simulated errors and noise.

---

# 3. RF Spectrum Scanner

The RF monitoring system detects multiple wireless signals in the area.

Example:

```json
[
    {
        "frequency": "2.4GHz",
        "signal_strength": -42,
        "direction": 120,
        "stability": 0.85
    },
    {
        "frequency": "5.8GHz",
        "signal_strength": -67,
        "direction": 80,
        "stability": 0.45
    }
]
```

Provided parameters:

- Frequency
- Signal strength
- Direction
- Signal stability
- Signal activity
- Multiple simultaneous RF sources

The environment may contain:

- UAV-related signals
- Random RF transmissions
- Background noise
- Interference signals

---

# 4. Vision Detection System

A simulated camera system provides object detection information.

Example:

```json
{
    "object_type": "unknown_air_object",
    "confidence": 0.91,
    "position": {
        "x": 240,
        "y": 180
    }
}
```

Provided parameters:

- Object classification
- Detection confidence
- Position
- Tracking information

---

# 5. Environmental Sensor Data

The control panel provides surrounding environmental conditions.

Example:

```json
{
    "wind_speed": 12,
    "wind_direction": 240,
    "visibility": 70,
    "temperature": 31,
    "humidity": 60
}
```

Provided parameters:

- Wind speed
- Wind direction
- Visibility
- Temperature
- Humidity
- Environmental changes

---

# 6. UAV Telemetry Data

Additional simulated telemetry information:

Example:

```json
{
    "battery": 78,
    "velocity": 14,
    "vertical_speed": 2,
    "flight_time": 320
}
```

Provided parameters:

- Battery level
- Velocity
- Vertical movement
- Flight duration
- Motion status

---

# Control Panel Interface

The simulated ground control station contains:

- 2D radar display
- UAV tracking information
- GPS location view
- RF spectrum monitor
- Camera detection panel
- Weather/environment panel
- UAV telemetry panel
- Real-time data stream

---

# Objective

Using the available sensor information, teams must create an intelligent system capable of analyzing the UAV environment and making autonomous decisions.

Teams can use any approach:

- Machine Learning models
- Prediction algorithms
- Statistical analysis
- Sensor fusion techniques
- Custom algorithms

The challenge is to extract meaningful information from multiple imperfect sensor sources and build an intelligent UAV monitoring system.
```
