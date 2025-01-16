# Tokyo Dataset
- **run1**: 2024/07/23 04:04:30 (GPST) - 2024/07/23 04:44:20 (GPST)

<img src="https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/tokyo1.jpg?raw=true" height=400px > <img src="https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/fisheye_satellite_short_tokyo1.gif?raw=true" height=400px >

- **run2**: 2024/07/23 01:10:00 (GPST) - 2024/07/23 01:40:30 (GPST)

<img src="https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/tokyo2.jpg?raw=true" height=400px > <img src="https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/fisheye_satellite_short_tokyo2.gif?raw=true" height=400px >

- **run3**: 2024/07/23 01:51:00 (GPST) - 2024/07/23 02:42:00 (GPST)

<img src="https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/tokyo3.jpg?raw=true" height=400px > <img src="https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/fisheye_satellite_short_tokyo3.gif?raw=true" height=400px >

## Ground truth
- Reference position and attitude was acquired using the Applanix POS LVX-120

![](https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/tumsat_poslv.jpg?raw=true)

## GNSS Data
### Vehicle GNSS data
- Receiver: Septentrio mosaic-X5
- Antenna: Trimble AT1675
- Data acquisition: 5 Hz
- Format: RINEX Version 3.04

### Reference station GNSS data
- Receiver: Trimble Alloy
- Antenna: Trimble Zephyr Geodetic 2
- Data acquisition: 1 Hz
- Format: RINEX Version 3.04
- Coordinate (phase center): `35.66633426, 139.79220181, 59.82` (deg, deg, m) 

## IMU data
- IMU: Analog Devices, ADIS16505-2
- Data acquisition: 100 Hz with GPS time stamp
- IMU mounting orientation (IMU coordinate system)
  - X direction: vehicle traveling direction, Y direction: vehicle right direction, Z direction: vehicle down direction
- GNSS antenna mounting position (lever arm) viewed from IMU
  - `0.593, -0.670, -1.216` (m)