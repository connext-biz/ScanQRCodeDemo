# QR code Scanner - Connext

A simple tool/demo for scanning QR code via WebRTC. Especially, using for VN citizen identification (VNCI).

## Description

Scanning QR code in a web enviroment is hard for the small and complex one, e.g., QRCode in VNCI.

Demo tools from html5-qrcode, zxing, or qr-scanner can't detect QRCode in VNCI.

Scanning QR code has 3 steps:
1. Capture image from camera via WebRTC.
2. Do some image processing.
3. Decode QR code from processed images.

### To improve the scanning quality for VNCI, we do:
1. Capture image from camera via WebRTC. Users can zoom the camera, and use Flash for trying.
2. Image processing: grayscale and blackwhite.
3. QR code decoding: using qr-scanner. [UMD build](https://github.com/nimiq/qr-scanner?tab=readme-ov-file#single-image-scanning)

**The image processing parameters aren't optimized yet.**

## Usage
Just run the index.html

## Personal testing results 
We do some manual testing on our own devices:
- Work well on iOS >= 17.0
- Work well on Android 
- Work on iOS < 17.0

Note: The scanning speed is related to the auto-focus function of the device.

## License
@2024 Connext