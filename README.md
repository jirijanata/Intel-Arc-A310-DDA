# Intel Arc A310 Hyper-V Discrete Device Assignment
This repository documents how to configure Hyper-V Discrete Device Assignment (DDA) on Windows Server 2025

Lenovo P360 Ultra
BIOS/UEFI Configuration
- Devices - Video
  - Auto
    - if there is no dedicated graphics card in x16/x4 slot -> everything will show on the IGD output
    - if there is a dedicated graphics card in x16/x4 slot and no display connected to the dedicated graphics card -> BIOS/UEFI/Boot screen will be always shown only on output of the dedicated graphics card, Windows login screen will be shown on IGD output, if there is display connected.
    - if there is a dedicated graphics card in x16/x4 slot and no display connected to the dedicated graphics card -> everything will be shown on output of the dedicated graphics card
  - IGD - if there is a dedicated graphics card in x16/x4 slot, the system won't boot.
  - PEG - only the dedicated graphics card in x16/x4 will be active

Lenovo P3 Ultra
BIOS/UEFI Configuration
- Devices - Video
  - Auto
    - if there is no dedicated graphics card in x16/x4 slot -> everything will show on the IGD output
    - if there is a dedicated graphics card in x16/x4 slot and no display connected to the dedicated graphics card -> BIOS/UEFI/Boot screen will be always shown only on output of the dedicated graphics card, Windows login screen will be shown on IGD output, if there is display connected.
    - if there is a dedicated graphics card in x16/x4 slot and no display connected to the dedicated graphics card -> everything will be shown on output of the dedicated graphics card
  - IGD - only the integraded graphics card will be active. The dedicated graphics card installed in x16/x4 slot will not be visible in Windows.
  - PEG - only the dedicated graphics card in x16/x4 will be active
      
