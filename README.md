# ARCH - Unreal Engine starter (AngelSkies TV)

The ARCH node as its own world, built from one Unreal project for **Meta Quest (VR)** and **Google Play (Android)**.
Part of AngelSkies TV (see angelskies-tv-roku) until ARCH becomes its own AR/VR + Google Play app.

## Open it
1. Install Unreal Engine 5.4 (Epic Games Launcher) and Git LFS (`git lfs install`)
2. `git clone https://github.com/AngelSkiesTV/arch-unreal`
3. Double-click ARCH.uproject
4. Create the level Content/ARCH/Maps/ARCH_Station and save (it's already set as the default map)

## Quest build
- Install Android Studio + NDK per Epic's Android setup docs; enable Developer Mode on the Quest
- Optional: enable the Meta XR plugin (MetaXR) for Quest-specific features; OpenXR is on by default
- Platforms > Android > Package (ASTC). Sideload with `adb install`

## Google Play build
Same Android package; for phone (non-VR) set a separate flat-screen pawn/map, then upload the AAB in Play Console.

## Content
- DAZ characters: see DAZ_Exports/README.md
- Videos: the Media folder will stream the ARCH feed from the AngelSkies Cloudflare backend once it's live
- Steam (PC VR): Windows target is included; Steam upload script can be added later
