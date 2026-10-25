# Mobileconfig Website

<div align="center">

  <img src="https://img.shields.io/badge/iOS%2FmacOS-Web%20Clip-007AFF?style=for-the-badge&logo=apple" alt="iOS/macOS web clip" />
  <img src="https://img.shields.io/badge/Type-Configuration%20Profile-4B8BBE?style=for-the-badge" alt="Configuration profile" />
  <img src="https://img.shields.io/badge/Status-Example%20Only-FF6B6B?style=for-the-badge" alt="Example only" />

</div>

A simple iOS/macOS web clip profile generator and example project for creating Home Screen bookmarks.

## Overview

This repository shows how to create a `.mobileconfig` file that adds a website shortcut to the Home Screen as a web clip. It is useful for turning a website into an app-like icon on iPhone or iPad.

## Features

- Home Screen web clip example
- Easy to customize for your own site
- Works as a simple iOS/macOS configuration profile
- Clean, minimal template for deployment testing

## Quick Start

1. Open `Example1.mobileconfig` or `Example2.mobileconfig`.
2. Change the label to your preferred app name.
3. Change the URL to your target website.
4. Save the file with a `.mobileconfig` extension.
5. Open the file on your device and install it.

## Example Profile

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
    <key>PayloadContent</key>
    <array>
        <dict>
            <key>FullScreen</key>
            <true/>
            <key>IgnoreManifestScope</key>
            <false/>
            <key>IsRemovable</key>
            <true/>
            <key>Label</key>
            <string>Example App</string>
            <key>Precomposed</key>
            <false/>
            <key>URL</key>
            <string>https://example.com</string>
            <key>PayloadIdentifier</key>
            <string>com.example.mywebclippayload</string>
            <key>PayloadType</key>
            <string>com.apple.webClip.managed</string>
            <key>PayloadUUID</key>
            <string>1d6d6912-708e-441a-9272-526ef05bbe3c</string>
            <key>PayloadVersion</key>
            <integer>1</integer>
        </dict>
    </array>
    <key>PayloadDisplayName</key>
    <string>Web Clip</string>
    <key>PayloadIdentifier</key>
    <string>com.example.myprofile</string>
    <key>PayloadType</key>
    <string>Configuration</string>
    <key>PayloadUUID</key>
    <string>289fc7fc-2870-479d-b30f-8d0592b7ef04</string>
    <key>PayloadVersion</key>
    <integer>1</integer>
</dict>
</plist>
```

## How to customize

### Change the app name

Update this value:

```xml
<key>Label</key>
<string>minecraft</string>
```

Replace it with the name you want shown on the Home Screen.

### Change the website

Update this value:

```xml
<key>URL</key>
<string>Minecraft.net</string>
```

Use a valid URL such as:

```text
https://example.com
https://yourdomain.com
```

## Installation Guide

1. Download the `.mobileconfig` file.
2. Open the file on your iPhone or iPad.
3. Go to Settings.
4. Scroll down to VPN & Device Management.
5. Open the profile.
6. Enter your passcode if prompted.
7. If you see a warning saying the profile is unsigned, review it carefully and continue if you understand the risk.
8. Once installed, look for the app icon on your Home Screen.

## Warning

This repository is for example and testing use. If a profile is unsigned or not trusted, you should review it before installing. Some profiles may require a valid certificate or trusted configuration before they work properly.

## Related Projects

- Mobileconfig Example: https://github.com/huynhw19/MOBILECONFIG-EXAMPLE
- Windows 11 EXE File: https://github.com/huynhw19/Windows-11-EXE-file

## Notes

- Replace example values before using in production.
- These profiles are meant as starting points, not as signed production deployments.
- Apple may require valid signing or a trusted profile for some enterprise scenarios.

---

Made for simple, clean website-to-app shortcuts on iOS and macOS.
