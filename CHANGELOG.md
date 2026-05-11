# Changelog

This file tracks released versions of the C# CaptureSDK.

## Version 2.0.33.469

### New

  * Added IsNFCReader and IsBarcodeReader methods in CaptureHelperDevice to distinguish device scan type



### Improvements

  * N/A


### Bug fixes

  * Fixed Net9 restriction on iOS. Now supports Net9 and above



## Version 2.0.26.184

### New

  * N/A


### Improvements

  * Updated native Android CaptureSDK to version 2.0.22

  * Updated minimum .NET target to version 9

  * Updated native iOS CaptureSDK to version 2.0.73. ARM64 simulator is added for build only purpose

  * Updated SetTrigger[...]Async into one method, SetTriggerAsync(). See ICaptureProperty.Values.Trigger values for arguments



### Bug fixes

  * N/A


## Version 2.0.19.509

### New

  * Added [Add/Remove]DeviceAsync methods to discover or remove a connectalbe Bluetooth LE device

  * Added Bluetooth LE devices connect operation: ConnectDiscoveredDeviceAsync method

  * Added a Windows Bluetooth Picker to pair to Classic Bluetooth devices



### Improvements

  * Deprecated old Bluetooth LE connection management: StartDeviceDiscoveryAsync and [Get/Set]FavoritesAsync methods

  * Removed the need to use the Device Manager

  * Updated AddBluetoothDeviceAsync with Classic Discovery mode to display the Bluetooth Picker on Windows



### Bug fixes

  * N/A


## Version 1.8.13.170
- Updated NuGet package released on [nuget.org](https://www.nuget.org/packages/SocketMobile.Capture)
- Added helper methods in CaptureHelper targeting Bluetooth LE devices
  - Added `[Get/Set]Property` to ease the creation of properties not listed in the Helper
  - Added `SetShutdownDevice` method to power off the device
  - Added `SetResetDevice` method to reset the device
  - Added `[Get/Set]LocalAcknowledgmentAsync` to manage scanning delays
  - Added `[Get/Set]DecodeActionAsync` to manage the scanner's behavior when reading a barcode (beep, LED, rumble)

## Version 1.8.1.594

- Updated NuGet package released on [nuget.org](https://www.nuget.org/packages/SocketMobile.Capture)
- Added support for SocketScan S721 scanner on Windows

## Version 1.7.112.395

- Updated NuGet package released on [nuget.org](https://www.nuget.org/packages/SocketMobile.Capture)
- Added SocketCam C820 support to MAUI
- Fixed symbology availability across different camera usages. Symbologies are now consistent across all devices

## Version 1.7.83.246

- Updated NuGet package released on [nuget.org](https://www.nuget.org/packages/SocketMobile.Capture)
- Fixed `SetTimersTimeoutAsync()` method by adding the auto lock parameter
  - Added Timer documentation [here](https://docs.socketmobile.dev/capture/csharp/en/latest/topicsTimers.html)
- Fixed SocketCam's stability on Windows (UWP)
  - Camera switch
  - No Camera detected
  - USB Camera support, check [documentation](https://docs.socketmobile.dev/capture/csharp/en/latest/topicsSocketCam.html) under SocketCam->Setup->Windows (UWP)->Note
- Added the NFC Tag ID, `TagIdData`, in the `CaptureDecodedData` received from the `DecodedData` event

## Version 1.7.68.40

- Updated NuGet package released on [nuget.org](https://www.nuget.org/packages/SocketMobile.Capture)
- Removed Xamarin support
- Added device properties in CaptureHelper
  - [Get/Set]ThemeSelectionAsync() method. Retrieve or Set the UI theme for devices like S550 or S370
  - SetFactoryResetAsync() method. Factory resets a Bluetooth Low Energy device like S320, S370, S550
  - [Get/Set]TimersTimeoutAsync() method. Retrieve or Set the auto lock and power off timers

## Version 1.7.54.884

- Last version to support Xamarin
- Updated NuGet package released on [nuget.org](https://www.nuget.org/packages/SocketMobile.Capture)
- Added support for M963 device 
- Fixed connection dropping after 30 seconds for projects targeting .NET 6 and above
- Updated documentation on S370 device about getting a double device arrival event

## Version 1.7.34.67

- Updated documentation on scanner configuration and pairing per platform
- Updated documentation on unsupported D600 and S370 devices on Windows
- Fixed Bluetooth Low Energy Manager device removal event when the Bluetooth is switched off
