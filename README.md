# Z370F-Hackintosh
EFI Partition and Guidelines for my Hackintosh

## Config
- iGPU Enabled Headless (Some DRM content like Apple TV driven by dGPU with `Shiki`)
- Verbose Off
- Scaled for 4K
- Boot picker is disabled by default (use `Option` key to show it)
- `agdpmod=pikera` is enabled because i'm using a Navi GPU.

## ACPI

1. DSDT.aml (disabled by default)
2. SSDT-PLUG.aml
3. SSDT-EC.aml
4. SSDT-HPET.aml
5. SSDT-USBX.aml
6. SSDT-UIAC.aml

## Kexts
1. Lilu
2. VirtualSMC
3. WhateverGreen
4. AppleALC
5. IntelMausi
6. SMCProcessor

## Bios
Disabled:
- Fast Boot
- VT-d
- CSM

Enabled:
- VT-x
- Above 4G decoding
- Hyper-Threading
- OS type: Windows 8.1/10 UEFI Mode
