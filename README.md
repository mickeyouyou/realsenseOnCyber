# Cyber Wrapper for Intel&reg; RealSense&trade; Devices
These are packages for using Intel RealSense cameras (D400 series SR300 camera and T265 Tracking Module) with Cyber.

## Installation Instructions

The following instructions support Cyber , on **Ubuntu 18.04**.


## Channels

```bash
/realsense/pose
/realsense/raw_image 
/realsense/acc
/realsense/gyro
```

## Start

> 1. Please ensure installed Cyber envonroment, you can echo cyber ip like:`echo ${CYBER_IP}` to check.
> 2. use `rs-enumerate-devices` debug tool ensure the mounted device.


Start driver by:
```bash 
bash realsense.sh
```

Check published data by `cyber_monitor`.

Stop:
```bash
bashh realsense.sh
```

## T265 API
https://github.com/IntelRealSense/librealsense/blob/master/doc/t265.md

- Frame Management : https://github.com/IntelRealSense/librealsense/blob/master/doc/frame_lifetime.md
- librealsense Error Handling Scheme : https://github.com/IntelRealSense/librealsense/blob/master/doc/error_handling.md
