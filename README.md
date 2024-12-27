# CAM-IMX708AF
## Description
- InnoMaker IMX708 Auto focus Camera Module Compatible with raspberry pi camera V3
 

##  Specification
- Back-illuminated, stacked CMOS 12-megapixel IMX708 image sensor
- High signal-to-noise ratio (SNR)
- Built-in 2D Dynamic Defect Pixel Correction (DPC)
- Phase Detection Autofocus (PDAF) for rapid autofocus
- QBC Re-mosaic function
- HDR mode (up to 3 megapixel output)
- CSI-2 serial data output
  - 2-wire serial communication (supports I2C fast mode and fast mode plus)
  - 2-wire serial control of focus mechanism
- Resolution: 11.9 megapixels
- Sensor size: 7.4mm sensor diagonal
- Pixel size: 1.4μm × 1.4μm
- Horizontal/vertical: 4608 × 2592 pixels
- Diagonal field of view: 75 degrees 
- Common video modes: 1080p50, 720p100, 480p120
- Output: RAW10
- IR cut filter: Integrated in standard variants; not present in NoIR variants
- Dimensions: 32 × 32 × 11.5mm (12.4mm height for Wide variants)
- Ribbon cable length: 150mm
  
-  Cable connector: 15 × 1mm FPC,22 x 0.5mm FPC
  

##  Quick Start Guide
- Step1, Add dtoverlay=imx708 to last line of config.txt
  - sudo nano /boot/firmware/config.txt
- Step2, Change camera_auto_detect=0
- Step3, reboot and preview
  - libcamera-hello -t 0

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
  - dtoverlay=imx708
  - Change camera_auto_detect=1 to camera_auto_detect=0

- Step3, Reboot and use below command to preview
  - libcamera-hello -t 0