# Overlays by WeoM

<div align="center">

**English | [Русский](README_ru.md)**

</div>

A set of overlays for RivaTuner Statistics Server (RTSS), designed on a 1920x1080 screen resolution.  
Supported platforms: Full versions are for AMD (CPU) only; the others were tested on AMD CPUs and NVIDIA GPUs, but should work on other platforms as well.

## Overlay variations

- **AMD Full v3.0 graph** — full overlay with two variants of CPU core load graphs
- **Regular** — inspired by a third‑party overlay, original author unknown
- **Mini / Micro / Nano / Pico** — compact overlays of different sizes
- **Horizontal** — NVIDIA‑style horizontal overlay
- **I2HARD AMD** — overlay inspired by I2HARD

## Table of contents

- [Requirements](#requirements)
- [Fonts used](#fonts-used)
- [Installation](#installation)
- [Important information](#important-information)
- [Screenshots](#screenshots)

## Requirements

- [RTSS](https://www.guru3d.com/download/rtss-rivatuner-statistics-server-download/)
- [MSI Afterburner](https://www.msi.com/Landing/afterburner/graphics-cards)
- [HWiNFO](https://www.hwinfo.com/) (recommended for proper display of the Full versions)

## Fonts used

- Impact Bold 7
- Roboto Bold 7 — [Download](https://fonts.google.com/specimen/Roboto)
- Unispace Bold 7 (default RTSS font)
- Bahnschrift Bold Condensed 7

## Installation

1. Download and extract the `overlays.zip` archive | **[Download latest version](https://github.com/We0M/Overlays/releases/download/v1.0/Overlays.7z)**
2. Open **RTSS** and go to:
   1. `Setup` → `Plugins`
   2. Make sure the checkbox next to `OverlayEditor.dll` is enabled.
   3. Double‑click `OverlayEditor.dll` to open the editor.
   4. In OverlayEditor, go to the **Overlays** tab → **Import**.
   5. Select the desired overlay from the folder where you extracted the archive.
3. If necessary, adjust data sources for your system.

## Important information

> [!IMPORTANT]
> **User settings in the overlays are locked by default.**
>
> All overlays ignore user OSD settings so that the overlay looks the same for everyone.  
> Because of this, changing font/scale via RTSS user settings does not work.
>
> To unlock this:
> 1. Open the overlay properties.
> 2. Uncheck `Lock user settings`.
> 3. Apply the font, style and size specified in the `Name` field.

> [!IMPORTANT]
> In the `AMD Full v3.0 graph …` overlays, some sensors are duplicated from LibreHardwareMonitor (LHM).
> Before relying on these readings, compare them with sensors from HWiNFO:
>
> 1. Some sensors may be missing in LHM.
> 2. Some sensors may show incorrect values.
> 3. Sensor names may not reflect their actual meaning.
>
> For example, on my system the SoC Voltage in LHM was labeled as `Vcore`,
> and the `Core (S12 TFN)` sensor did not show core voltage at all.

> [!CAUTION]
> **CPU clock from RTSS may cause stutters.**
>
> On a Ryzen 5 5600G system, the `CPU clock` source from RTSS caused micro‑stutters
> (visible on the Frametime graph and confirmed via `%PollingTime0%`, `%PollingTime1%` macros).
>
> It is recommended not to use `CPU clock` from RTSS and to keep the CPU frequency
> source provided by MSI Afterburner / HWiNFO instead.

## Screenshots
<div align="center">

### Impact default 7
![AMD Full v3.0 graph v1 Impact](preview/AMD%20Full%20v3.0%20graph%20v1%20impact.png)
![AMD Full v3.0 graph v2 Impact](preview/AMD%20Full%20v3.0%20graph%20v2%20impact.png)

| ![Regular v1.0 impact](preview/Regular%20v1.0%20impact.png) | ![Mini v1.0 impact](preview/Mini%20v1.0%20impact.png) | ![Micro v1.0 impact](preview/Micro%20v1.0%20impact.png) | ![Nano v1.0 impact](preview/Nano%20v1.0%20impact.png) | ![Pico v1.0 impact](preview/Pico%20v1.0%20impact.png) |
| :---------------------------------------------------------: | :---------------------------------------------------: | :-----------------------------------------------------: | :---------------------------------------------------: | :---------------------------------------------------: |
|                        Regular v1.0                         |                       Mini v1.0                       |                       Micro v1.0                        |                       Nano v1.0                       |                       Pico v1.0                       |

### Font: Roboto Bold 7

![AMD Full v3.0 graph v1 Roboto](preview/AMD%20Full%20v3.0%20graph%20v1%20Roboto.png)
![AMD Full v3.0 graph v2 Roboto](preview/AMD%20Full%20v3.0%20graph%20v2%20Roboto.png)

| ![Horizontal v1.0 static FT](preview/Horizontal%20v1.0%20Roboto%20static%20FT.png) |
| :---------------------------------------------------------: |
|                        Horizontal v1.0 static FT            |

### Font: Unispace Bold 7 (this is the default RTSS font)
![AMD Full v3.0 graph v2 Unispace](preview/AMD%20Full%20v3.0%20graph%20v2%20Unispace.png)

### I2HARD | Font: Bahnschrift Bold Condensed 7

> Thanks to the I2HARD channel for the idea for this overlay — I just recreated it.

![I2HARD AMD v2.0](preview/I2HARD%20AMD%20v2.0.png)

</div>

