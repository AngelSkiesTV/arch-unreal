# ARCH - Meta Quest VR Preview

## Live preview while you build (PC + Quest Link)
1. Install the **Meta Quest Link** app on your Windows PC and sign in.
2. Connect the Quest with a USB-C cable (Link) or enable **Air Link** (same 5 GHz Wi-Fi).
3. In the Link app: Settings > General > set **Meta Quest Link as active OpenXR runtime**, and enable **Unknown sources**.
4. Put on the headset and start Quest Link.
5. `git pull` this repo, open `ARCH.uproject` in Unreal Engine 5.4.
6. Click the arrow next to Play > **VR Preview**. The level runs in your headset while the editor stays open.
7. Optional: Editor toolbar > **VR Mode** to edit the level from inside the headset.

## Standalone build on the Quest (no PC)
1. Enable Developer Mode on the Quest (Meta Horizon phone app > Devices > Developer Mode).
2. Install Android Studio + the SDK/NDK versions Unreal 5.4 asks for (Project Settings > Platforms > Android SDK).
3. Platforms > Android > **Package Project** (ASTC). Install the APK with `adb install` or Meta Quest Developer Hub.

## Notes
- OpenXR is enabled; the Meta XR (OculusXR) plugin is optional - install it from the Meta link in ARCH.uproject for passthrough/hand tracking.
- Project targets Quest 2, Quest Pro and Quest 3 with forward shading, multiview and 4x MSAA for performance.
