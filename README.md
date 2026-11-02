# Simple Waypoints — Beam Only (Minecraft 26.3)

A client-side Fabric waypoint mod. In the world, waypoints are shown only by a 3D beacon-style beam. There are no logo markers, ground rings, floating labels, or distance labels. The beam keeps a bright core and a narrow, faint but visible outer shell.

## Target
- Minecraft Java 26.3
- Fabric Loader 0.19.5 or newer
- Java 25
- Fabric API for Minecraft 26.3 (the build currently uses 0.163.0+26.3)

## Build with GitHub Actions
1. Upload the contents of this folder to the root of your GitHub repository. Include the hidden `.github` folder.
2. Push to the `main` branch (or use Actions → Build Simple Waypoints → Run workflow).
3. Wait for the workflow to finish successfully.
4. Open the successful run, scroll to **Artifacts**, and download `simple-waypoints-mc-26.3-beam-only`.
5. Extract that artifact ZIP. The `.jar` inside is the file to place in `.minecraft/mods`.

## Build locally
With JDK 25 and Gradle 9.8 installed, run:

```bash
gradle clean build --no-daemon -PwithBeam=true
```

The mod JAR is written to `build/libs/`. Do not put this source project ZIP in the Minecraft `mods` folder.

## Note
The source package is prepared for the 26.3 toolchain, but it has not been compiled or launched in this environment. The GitHub Actions run is the verification step; use its compiler output if any source API needs adjustment.
