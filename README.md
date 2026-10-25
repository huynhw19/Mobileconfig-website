# Mobileconfig-website
Mobileconfig website is a iOS and macOS that puts the bookmark
in your apps.

Start with this






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
            <string>minecraft</string>
            <key>Precomposed</key>
            <false/>
            <key>URL</key>
            <string>Minecraft.net</string>
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








Edit these:
Change the label into a name. This label will be added to Home Screen.


Change the URL into a valid website. This bookmark will be added to Home Screen.


Once you complete that, Save that to file, Go to the 3 dots, and open options. You will see something bottom of the screen. Turn on and hold the .txt file and select rename. Remove txt and add mobileconfig.

Installer guide.
1. Launch the mobileconfig file
2. Open settings and scroll down to VPN
3. Open the profile
4. Enter your passcode
5. If it say, This profile is not sign, Ignore this and install
6. Once it install, search in apps and start website.

If you got an error, that means you done something wrong. Try use an example and change the mobileconfig into a txt.
You might want to update to fix some errors.


See other projects
Mobileconfig example: https://github.com/huynhw19/MOBILECONFIG-EXAMPLE

Windows 11 Exe file: https://github.com/huynhw19/Windows-11-EXE-file
