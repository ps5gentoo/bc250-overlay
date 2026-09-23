Small Repo Stuff for the BC-250 with Gentoo.


## References & Credits

| Project | Resources | Used by |
|---|---|---|
| BC-250 40 CU Unlock | [Repository](https://github.com/duggasco/bc250-40cu-unlock) | Original Arch implementation for `bc250-40cu.sh` |
| BC-250 CU Live Manager | [Repository](https://github.com/WinnieLV/bc250-cu-live-manager) · [Script](https://github.com/WinnieLV/bc250-cu-live-manager/blob/main/bc250-cu-live-manager.sh) | `bc250-40cu.sh` |
| UMR | [Repository](https://gitlab.freedesktop.org/tomstdenis/umr) | `bc250-40cu.sh`, `bc250-cu-status.sh` |
| BC-250 ACPI Fix | [Original tables](https://github.com/bc250-collective/bc250-acpi-fix) · [8-core update](https://github.com/mendesrr/bc250-acpi-fix-updated-8c) · [guarded universal sources](acpi-tables/) | `bc250-power.sh` |
| Cyan Skillfish Governor | [Repository](https://github.com/filippor/cyan-skillfish-governor/tree/smu) · [Performance-mode script](https://github.com/filippor/cyan-skillfish-governor/blob/smu/scripts/cyan-skillfish-performance-mode) | `bc250-power.sh` |
| BC-250 SMU OC | [Repository](https://github.com/bc250-collective/bc250_smu_oc) | `bc250-power.sh` |
| CachyOS BC250 Toolkit | [Repository](https://github.com/redbeard1083/bc250-toolkit) | Design reference for the independently implemented zswap-backed disk profile; upstream code has no declared license |
| BC-250 CPU Core Unlock | [Linux helper](https://github.com/rw-r-r-0644/bc250-core-unlock) · [EFI source](https://github.com/Hexxeh/bc250-efi-core-unlock) · [EFI headers](https://github.com/yoppeh/efi) | Original SMU method and the optional pre-boot implementation adapted by `bc250-power.sh` |
| BC-250 Memory Config | [Repository](https://github.com/fanoush/bc250_memcfg) · [VRAM guide](https://elektricm.github.io/amd-bc250-docs/bios/vram/) | CMOS UMA utility fetched by `bc250-ram-split.sh` |
| BC-250 GDDR6 Memory Temperature | [Repository](https://github.com/pan-Rijovich/bc250-memory-temperature) · [integrated commit](https://github.com/pan-Rijovich/bc250-memory-temperature/commit/b7e6bffcb5d592fc03edde375b7598ddc79aa846) | Live SMU payload and MR3 temperature method by pan-Rijovich and bc250-collective, guarded by `bc250-memory-temperature.sh` |
| BC-250 GFX1013 Fix | [Repository](https://github.com/DryhoppedIPA/bc250-gfx1013-fix) · [integrated commit](https://github.com/DryhoppedIPA/bc250-gfx1013-fix/commit/d3e6dc062c34d2523db0abe5741d1f5b0dea00d9) | Kernel compute lifecycle repair and pinned alternate RADV build by DryhoppedIPA |
| OptiScaler | [Repository](https://github.com/optiscaler/OptiScaler) · [release](https://github.com/optiscaler/OptiScaler/releases/tag/v0.9.4) | Checksum-pinned per-game installation with collision backups and guarded rollback |
| BC-250 FSR4 RC9 | [Repository](https://github.com/daniel-h-0/bc250-fsr4-fork) · [release](https://github.com/daniel-h-0/bc250-fsr4-fork/releases/tag/v4.0.0-rc9) | Integrity-checked portable FSR 4.1.1 INT8 DLL with per-target rollback |
| CachyOS BC-250 GE-Proton and RADV | [Repository](https://github.com/MastaG/linux-cachyos-bc250) · [release assets](https://github.com/MastaG/linux-cachyos-bc250/releases/tag/repo) | Checksum-pinned GE compatibility tool and FSR4 Mesa patch series adapted for user-local SteamOS installation |
| BC-250 HDMI AC-3 encoding | [Implementation guide and scripts](https://github.com/rpf16rj/bc250-steamos-real-toolkit/tree/main/extras/hdmi-ac3-encoding) | ALSA `a52` routing and WirePlumber profile behavior adapted by `hdmi-ac3/hdmi-ac3.sh` |
| Valve kernel mirror | [Repository](https://github.com/Evlav/linux-integration) | `bc250-audio-fix/fetch-sources.sh` |
| SteamOS package mirror | [Package index](https://steamdeck-packages.steamos.cloud/archlinux-mirror/) | Audio, AIC8800, and NCT6687 build scripts; stable channels are discovered automatically |
| SteamOS atomic-update keep list | [Defaults](https://github.com/evlaV/steamos-customizations/blob/master/atomic-update/rauc/atomic-update-keep.conf.in) · [Drop-in example](https://github.com/evlaV/steamos-customizations/blob/master/atomic-update/rauc/example-additional-keep-list.conf.in) | `bc250-update-persistence.sh` |
| AIC8800 | [Repository](https://github.com/shenmintao/aic8800d80) · [integrated commit](https://github.com/shenmintao/aic8800d80/commit/e93a7d2b6b9634acefc2aae2891e787fb48fdb01) | `aic8800/steamdeck-setup.sh` |
| NCT6687D | [Repository](https://github.com/Fred78290/nct6687d) · [integrated commit](https://github.com/Fred78290/nct6687d/commit/a49a8abdfb6221772ecc836b3109e0cc338203cf) | `nct6687d/steamdeck-setup.sh` |
