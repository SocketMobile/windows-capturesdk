# Changelog

This file tracks released versions of the C# CaptureSDK.

## Version 1.7.34.67

- Updated documentation on scanner configuration and pairing per platform
- Updated documentation on unsupported D600 and S370 devices on Windows
- Fixed Bluetooth Low Energy Manager device removal event when the Bluetooth is switched off

## Version 1.7.54.884

- Last version to support Xamarin
- Updated NuGet package released on [nuget.org](https://www.nuget.org/packages/SocketMobile.Capture)
- Added support for M963 device 
- Fixed connection dropping after 30 seconds for projects targeting .NET 6 and above
- Updated documentation on S370 device about getting a double device arrival event

## Version 1.7.68.40

- Updated NuGet package released on [nuget.org](https://www.nuget.org/packages/SocketMobile.Capture)
- Removed Xamarin support
- Added device properties in CaptureHelper
  - [Get/Set]ThemeSelectionAsync() method. Retrieve or Set the UI theme for devices like S550 or S370
  - SetFactoryResetAsync() method. Factory resets a Bluetooth Low Energy device like S320, S370, S550
  - [Get/Set]TimersTimeoutAsync() method. Retrieve or Set the auto lock and power off timers
