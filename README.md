# PocketBridge

PocketBridge is a C#/.NET 10 Windows app for sending files between PCs and phones on the same Wi-Fi network.

## Download

Open **Releases** and download `PocketBridge.exe`. It is a self-contained Windows x64 app; no separate .NET installation is required. Windows Firewall may ask to allow private-network connections the first time you run it.

## Use PocketBridge

- **PC to PC:** Open the app on both PCs, select a device, choose a file or folder, and send. The receiving PC asks before saving.
- **Phone or tablet:** Choose **Quick connect QR…** on the PC and scan the code. Keep the page open on the same Wi-Fi to send files in either direction.
- Folders are sent as ZIP files. Files received by the PC are saved in `Downloads\PocketBridge`.

Pairing codes expire after 10 minutes and work once. Transfers require approval on the receiving device. Transfers stay on the local network and are unencrypted, so use a trusted Wi-Fi network.

## Build

Install the .NET 10 SDK and run `dotnet publish .\PocketBridge.csproj -c Release -r win-x64 --self-contained true -p:PublishSingleFile=true -p:IncludeNativeLibrariesForSelfExtract=true -p:EnableCompressionInSingleFile=true`.

## License

No open-source license has been assigned. You may download and run the published application; source reuse and redistribution are not granted.
