# Nagoya Dataset
- **run1**: 2024/08/03 08:53:00 (GPST) - 2024/08/03 09:18:30 (GPST)

<img src="https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/nagoya1.jpg?raw=true" height=400px > <img src="https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/fisheye_satellite_short_nagoya1.gif?raw=true" height=400px >

- **run2**: 2024/07/20 10:22:00 (GPST) - 2024/07/20 10:53:30 (GPST)

<img src="https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/nagoya2.jpg?raw=true" height=400px > <img src="https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/fisheye_satellite_short_nagoya2.gif?raw=true" height=400px >

- **run3**: 2024/08/03 09:50:00 (GPST) - 2024/08/03 10:07:20 (GPST)

<img src="https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/nagoya3.jpg?raw=true" height=400px > <img src="https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/fisheye_satellite_short_nagoya3.gif?raw=true" height=400px >


## Ground truth
- Reference position and attitude was acquired using the Applanix POS LV 220

![](https://github.com/taroz/Misc/blob/master/data/PPC-Dataset/meijo_poslv.jpg?raw=true)

## GNSS Data
### Vehicle GNSS data
- Receiver: Septentrio mosaic-X5
- Antenna: Trimble Zephyr 3 Rover
- Data acquisition: 5 Hz
- Format: RINEX Version 3.04

### Reference station GNSS data
- Receiver: Trimble NetR9
- Antenna: Trimble Zephyr Geodetic 2
- Data acquisition: 1 Hz
- Format: RINEX Version 3.04
- Coordinate (phase center): `35.13470947, 136.97757427, 104.718` (deg, deg, m) 

## IMU data
- IMU: Analog Devices, ADIS16505-2
- Data acquisition: 100 Hz with GPS time stamp
- IMU mounting orientation (IMU coordinate system)
  - X direction: vehicle traveling direction, Y direction: vehicle right direction, Z direction: vehicle down direction
- GNSS antenna mounting position (lever arm) viewed from IMU
  - `0.593, -0.670, -1.216` (m)