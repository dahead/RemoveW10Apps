# Remove Windows 10 built-in applications

This repository contains a powershell script for removing the Windows 10 built-in apps.

List all installed apps for all users:
```powershell
Get-AppxPackage -AllUsers | ft Name, PackageFullName -AutoSize
```

Remove all pre-installed apps:
```powershell
Get-AppxPackage -AllUsers | Remove-AppxPackage
```
