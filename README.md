# Cyber Wrapper for Intel&reg; RealSense&trade; Devices
These are packages for using Intel RealSense cameras (D400 series SR300 camera and T265 Tracking Module) with Cyber.

## Installation Instructions

The following instructions support Cyber , on **Ubuntu 18.04**.

### Step 1: Install the latest Intel&reg; RealSense&trade; SDK 2.0
- #### Install from [Debian Package](https://github.com/IntelRealSense/librealsense/blob/master/doc/distribution_linux.md#installing-the-packages) - In that case treat yourself as a developer. Make sure you follow the instructions to also install librealsense2-dev and librealsense-dkms packages.

#### OR
- #### Build from sources by downloading the latest [Intel&reg; RealSense&trade; SDK 2.0](https://github.com/IntelRealSense/librealsense/releases/tag/v2.24.0) and follow the instructions under [Linux Installation](https://github.com/IntelRealSense/librealsense/blob/master/doc/installation.md)

### Step 2: Install Cyber RT
Install by readme by https://github.com/mickeyouyou/apollo_lite

## Published Channels

```bash
/realsense/pose
/realsense/left_image
/realsense/right_image 
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
bash realsense.sh stop
```

## T265 API
https://github.com/IntelRealSense/librealsense/blob/master/doc/t265.md

- Frame Management : https://github.com/IntelRealSense/librealsense/blob/master/doc/frame_lifetime.md
- librealsense Error Handling Scheme : https://github.com/IntelRealSense/librealsense/blob/master/doc/error_handling.md
