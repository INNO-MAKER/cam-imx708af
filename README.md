# CAM-IMX708AF
## Description
- InnoMaker IMX708 Auto focus Camera Module Compatible with raspberry pi camera V3
 

##  Specification
- Back-illuminated, stacked CMOS 12-megapixel Sony IMX708 image sensor
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
- Dimensions: 25 × 24 × 11.5mm (12.4mm height for Wide variants)
- Ribbon cable length: 200mm
-  Cable connector: 15 × 1mm FPC

##  Quick Start Guide
- Step1, Add dtoverlay=imx708 to last line of config.txt
  - sudo nano /boot/firmware/config.txt
- Step2, Change camera_auto_detect=0
- Step3, reboot and preview
  - libcamera-hello -t 0