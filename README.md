# Default waw Unity Project

## Overview
This project is a **cross-platform Unity template** designed to support multiple platforms, including **VR, Mobile, Desktop, and Web**. Created and supported by **Web Art Work team**, this project ensures a flexible and scalable development environment. It is also **managed by waw CLI** for automation and build processes.

## CLI Tool
For automation, use **waw unity CLI** to build and manage the project efficiently.

## Supported Platforms
The project supports the following platforms:

| Name               | Platform Type | OS / Device                          | Output  |
|-------------------|--------------|----------------------------------|---------|
| **vr-android**      | VR           | Quest, Pico (Standalone VR)       | `.apk`  |
| **vr-windows**      | VR           | Valve Index, HTC Vive, Windows MR | `.exe`  |
| **vr-macos**        | VR           | Mac-compatible VR (limited)       | `.app`  |
| **mobile-android**  | Mobile       | Android phones & tablets         | `.apk`  |
| **mobile-ios**      | Mobile       | iPhones & iPads                  | `.ipa`  |
| **desktop-windows** | Desktop      | Windows PC                       | `.exe`  |
| **desktop-linux**   | Desktop      | Linux PC                         | `.x86_64` |
| **desktop-macos**   | Desktop      | Mac                               | `.app`  |
| **web**            | Web          | WebGL & WebXR (Browsers)         | Web files |

## Project Structure
```
/default-unity-project
 ├── /core          → Shared logic (gameplay, UI, networking)
 ├── /platforms
 │    ├── /vr-android      → Quest, Pico VR setup
 │    ├── /vr-windows      → SteamVR, OpenXR setup
 │    ├── /vr-macos        → macOS VR support (limited)
 │    ├── /mobile-android  → Android-specific configurations
 │    ├── /mobile-ios      → iOS-specific configurations
 │    ├── /desktop-windows → Windows-specific configurations
 │    ├── /desktop-linux   → Linux-specific configurations
 │    ├── /desktop-macos   → macOS-specific configurations
 │    ├── /web             → WebGL & WebXR configurations
 ├── /assets        → Common assets (textures, models, UI)
 ├── /scripts       → Shared C# scripts for game logic
 ├── /builds        → Output builds per platform
```

## Development Plan
### **1️⃣ Initialize Project**
1. Create a **new Unity project**.
2. Install **XR Plugin Management** (for OpenXR support).
3. Configure **Cross-Platform Input System**.
4. Create a **basic scene with UI** for testing.

### **2️⃣ Initialize Each Platform**
1. **VR Android (Quest, Pico)** → Configure OpenXR, add Oculus/Pico SDK if needed.
2. **VR Windows (Valve, Vive, Windows MR)** → Enable OpenXR, setup SteamVR.
3. **VR macOS** → Implement limited VR support.
4. **Mobile (Android, iOS)** → Implement touch UI & accelerometer support.
5. **Desktop (Windows, macOS, Linux)** → Set up keyboard/mouse & controller input.
6. **Web (WebGL, WebXR)** → Adjust UI for browser compatibility.

### **3️⃣ Build Each Platform**
1. Automate builds per platform using **waw unity CLI**.
2. Ensure platform-specific optimizations.
3. Test on real devices for performance tuning.

## Next Steps
- Finalize base template setup.
- Implement automated build scripts using **waw unity CLI**.
- Create a GitHub repository for version control and contributions.

---
🚀 **This project serves as the foundation for developing cross-platform applications in Unity. Developers can extend and customize platform-specific implementations while keeping a unified core.**

