---
Name: DeviceCredentialDeployment.exe
Description: Device Credential Deployment
Author: 'Elliot Killick'
Created: '2021-08-16'
Commands:
  - Command: DeviceCredentialDeployment
    Description: Grab the console window handle and set it to hidden
    Usecase: Can be used to stealthily run a console application (e.g. cmd.exe) in the background
    Category: Conceal
    Privileges: User
    MitreID: T1564
    OperatingSystem: Windows 10
Full_Path:
  - Path: C:\Windows\System32\DeviceCredentialDeployment.exe
Detection:
  - IOC: DeviceCredentialDeployment.exe should not be run on a normal workstation
Acknowledgement:
  - Person: Elliot Killick
    Handle: '@elliotkillick'
---