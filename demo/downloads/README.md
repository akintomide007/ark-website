# Mobile App Downloads

This directory hosts the mobile app files for direct download via QR code.

## Files

- `ark-home.apk` - Android APK file (auto-generated during build)
- `ark-home.ipa` - iOS IPA file (manual upload required)

## Setup

1. Build the mobile app using `./build-mobile.sh`
2. Copy the generated APK from `android/app/build/outputs/apk/release/` to this directory
3. The QR code on the dashboard will automatically point to the APK download

## Dynamic URLs

The download URLs are automatically generated based on the current Orange Pi IP:
- APK: `http://[ORANGE_PI_IP]:3006/downloads/ark-home.apk`
- QR Code: Generated dynamically pointing to the APK URL

## Features

- ✅ Dynamic IP discovery - no hardcoded addresses
- ✅ QR code generation for easy mobile downloads
- ✅ Works alongside App Store/Play Store distribution
- ✅ Hosted directly on Orange Pi device
