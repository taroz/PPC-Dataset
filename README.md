# Precise Positioning Challenge (PPC)
The Precise Positioning Challenge (PPC) is a challenge to develop technology to achieve precise position estimation from GNSS and IMU data acquired by vehicles in the urban environment of Japan. This challenge was held between November and December 2024. The dataset from this PPC will be made available as open data.

## Features
- Three-frequency multi-GNSS and high rate (5 Hz) GNSS data for driving in urban environments
- High precision MEMS IMU data (100Hz) synchronized to GPS time
- Provides reference station GNSS data
- Provides reliable positional ground-truth data

# Download
- PPC 2024
  - [Download Link]() (200MB)

# Directory Structure
```
PPC-Dataset
│   README.md : Dataset description
│
└───nagoya : Vehicle driving data set in Nagoya
│   │   README.md : Nagoya dataset description
│   └───run1
│       │   base.nav  : RINEX navigation data of a reference station
│       │   base.obs  : RINEX observation data of a reference station
│       │   rover.obs : RINEX observation data on vehicles
│       │   imu.csv   : IMU data on vehicles
│       │   reference.csv : Ground truth of vehicle position and attitude
│   └───run2
│       │   ...
│   └───run3
│       │   ...
└───tokyo : Vehicle driving data set in Tokyo
│   │   README.md : Tokyo dataset description
│   └───run1
│       │   ...
│   └───run2
│       │   ...
│   └───run3
│       │   ...
```
# Nagoya data

# Tokyo data

# GNSS Data
- Vehicle GNSS data
  - Septentrio mosaic-X5 mounted on a vehicle and data acquisition at 5Hz
  - The format is RINEX Version 3.04
  - Antenna
    - Tokyo data: Trimble AT1675
    - Nagoya data: Trimble Zephyr 3 Rover

- Reference station GNSS data
  - Data acquisition at 1Hz, format RINEX Version 3.04
  - Receiver/antenna/coordinates
    - Tokyo data: Trimble Alloy/Zephyr Geodetic 2
      - Antenna coordinates (phase center): `35.66633426, 139.79220181, 59.82` (deg, deg, m)
    - Nagoya Data: Trimble NetR9/Zephyr 3 Base
      - Antenna coordinates (phase center): `35.13470947, 136.97757427, 104.718` (deg, deg, m)

# IMU data
- IMU: Analog Devices, ADIS16505-2
- CSV file of IMU acceleration and angular velocity acquired at 100Hz
- IMU mounting orientation (IMU coordinate system)
  - X direction: vehicle traveling direction Y direction: vehicle right direction Z direction: vehicle down direction
- GNSS antenna mounting position (lever arm) viewed from IMU
  - Tokyo data: `0.31, 0.0, -0.55` (m)
  - Nagoya data: `0.593, -0.670, -1.216` (m)