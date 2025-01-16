# Precise Positioning Challenge (PPC)
The Precise Positioning Challenge (PPC) is a challenge to develop technology to achieve precise position estimation from GNSS and IMU data acquired by vehicles in the urban environment of Japan. This challenge was held between November and December 2024. The dataset from this PPC will be made available as open data.

## Features
- Triple frequency multi-GNSS and high rate (5 Hz) GNSS data for driving in urban environments
- High-precision MEMS IMU data (100Hz) synchronized to GPS time
- Provides reference station GNSS data
- Provides reliable ground truth data

# Download
- [Download Link](https://drive.google.com/file/d/19bOSJpqblSTm6iSW5aaRekcSC2hUae9V/view?usp=drive_link) (Google Drive, 155MB)

# Directory Structure
```
PPC-Dataset
│   README.md : Dataset description
│
└───nagoya : Vehicle driving data in Nagoya
│   │   README.md : Nagoya dataset description
│   └───run1
│       │   base.nav  : RINEX navigation data of a reference station
│       │   base.obs  : RINEX observation data of a reference station
│       │   rover.obs : RINEX observation data on vehicles
│       │   imu.csv   : IMU data on vehicles
│       │   reference.csv : Ground truth of vehicle position and attitude
│       │   trajectory.kml : Trajectory of the vehicle 
│   └───run2
│       │   ...
│   └───run3
│       │   ...
└───tokyo : Vehicle driving data in Tokyo
│   │   README.md : Tokyo dataset description
│   └───run1
│       │   ...
│   └───run2
│       │   ...
│   └───run3
│       │   ...
```
# Nagoya dataset
Click [here](./nagoya) for more information
![](https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/nagoya_trajectory.jpg?raw=true)

# Tokyo dataset
Click [here](./tokyo) for more information
![](https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/tokyo_trajectory.jpg?raw=true)

# GNSS Data
- Vehicle GNSS data
  - Septentrio mosaic-X5 mounted on a vehicle and data acquisition at 5 Hz
  - Format: RINEX Version 3.04
  - Antenna
    - Tokyo data: Trimble AT1675
    - Nagoya data: Trimble Zephyr 3 Rover

- Reference station GNSS data
  - Data acquisition at 1 Hz, format: RINEX Version 3.04
  - Receiver/antenna/coordinates
    - Tokyo data: Trimble Alloy/Zephyr Geodetic 2
      - Antenna coordinates (phase center): `35.66633426, 139.79220181, 59.82` (deg, deg, m)
    - Nagoya data: Trimble NetR9/Zephyr 3 Base
      - Antenna coordinates (phase center): `35.13470947, 136.97757427, 104.718` (deg, deg, m)

# IMU data
- IMU: Analog Devices, ADIS16505-2
- CSV file of IMU acceleration and angular velocity acquired at 100 Hz
- IMU mounting orientation (IMU coordinate system)
  - X direction: vehicle traveling direction, Y direction: vehicle right direction, Z direction: vehicle down direction
- GNSS antenna mounting position (lever arm) viewed from IMU
  - Tokyo data: `0.31, 0.0, -0.55` (m)
  - Nagoya data: `0.593, -0.670, -1.216` (m)

# Additional Information
- [PPC2024 overview](http://taroz.net/data/PPC2024.pdf) (in Japanese)
- [PPC2024 results](http://taroz.net/data/PPC2024_results.pdf) (in Japanese)