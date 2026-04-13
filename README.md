# CAM-IMX708AF

## Description
- InnoMaker IMX708 Auto focus Camera Module Compatible with raspberry pi camera V
  
![alt text](https://github.com/INNO-MAKER/cam-imx708af/blob/main/images/7.jpg)

# Description
- Camera Module 3 can be used to take full HD video as well as stills photographs, and features an HDR mode up to 3 megapixels. It carries IR cut filter. Its operation is fully supported by the libcamera library, including Camera Module 3’s rapid autofocus feature: this makes it easy for beginners to use, while offering plenty for advanced users. Camera Module 3 is compatible with all Raspberry Pi computers.
- Camera Module Third Generation: Back-illuminated and stacked CMOS 12-megapixel image sensor (IMX708) with HDR for up to 3 megapixel output
- High-quality Image Output: 4608 × 2592 pixels, carrying IR cut filter, along with built-in 2D DPC and QBC Re-mosaic function, offering high SNR
- Autofocus System: Phase detection autofocus
- CSI-2 serial Data Output: 2-wire serial communication, supporting I2C fast mode and fast-mode plus

# Quick Start For Raspberry PI Series

- Step1, Modify config.txt
  - sudo nano /boot/config.txt
  - For the latest version raspberry Pi OS, it should be 
    - sudo nano /boot/firmware/config.txt

- Step2, Add below content to the last line
  - dtoverlay=imx708  #for pi5+latest os, should add csi channel. Like dtoverlay=imx708,cam0 or dtoverlay=imx708,cam1
  - Change camera_auto_detect=1 to camera_auto_detect=0

- Step3, Reboot and use below command to preview
  - libcamera-hello -t 0
