# BugFix-QBluetooth-pairing-pin

Created by E-Protocol
https://github.com/e-protocol

Bug fix: QBluetooth pairing pin failure with user input

Platform: Android

IDE: Qt Creator version 5.3.12
Build under OS Linux

Description: 
Includes QtBluetoothBroadcastReceiver (java) file - required for fixing bug 
with pairing devices with 4-digit pin (i.e. 0000/1234). Just follow the 
instructions below.

Instructions:
1) Download QtBluetoothBroadcastReceiver.java from GitHub
https://github.com/e-protocol/BugFix-QBluetooth-pairing-pin
2) Replace original file. In my Linux OS location:
/opt/Qt5.12.3/5.12.3/Src/qtconnectivity/src/android/bluetooth/src/org/qtproject/qt5/android/bluetooth
3) Open bluetooth.pro as a project in Qt. In my Linux OS location:
/opt/Qt5.12.3/5.12.3/Src/qtconnectivity/src/android/bluetooth
4) Choose required build for your current Android version. 
5) Take file from your release in the same directory as bluetooth.pro QtAndroidBluetooth.jar and replace it in your templates. In my OS Linux location: /opt/Qt5.12.3/5.12.3/android_armv7/jar where android_armv7 is a build version for your current Android version
6) Build release and be happy! Now you can use QBluetooth lib and pair with any bluetooth device
