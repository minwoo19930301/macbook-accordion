<p align="center">
  <a href="https://github.com/minwoo19930301/macbook-accordion/releases/latest/download/MacBookAccordion-0.1.3.dmg"><img src="https://img.shields.io/badge/DOWNLOAD%20DMG-0.1.3-FFCC00?style=for-the-badge&labelColor=111111" alt="Download DMG"></a>
</p>

# MacBook Accordion

A tiny accordion you play with your MacBook's lid angle sensor.

<table>
  <tr>
    <td width="70%"><img src="assets/macbook-accordion-usage.png" alt="Holding a MacBook like an accordion"></td>
    <td width="30%" align="center"><img src="assets/app-icon.png" alt="App icon" width="180"></td>
  </tr>
</table>

## Install

1. Click **DOWNLOAD DMG** above.
2. Open the DMG and drag `MacBook Accordion.app` into `Applications`.
3. Launch it from `Applications`, and keep that copy in the Dock.

It's an unsigned personal build. If macOS blocks the first launch, Control-click the app and choose `Open` once.

## How to play

1. Cover the ambient light sensor next to the camera with a finger.
2. While covered, open and close the lid. A note plays each time the angle crosses into the next note.
3. Uncover it to move the lid silently.

It reads only the light sensor's lux value, not camera video, so no camera permission is needed. Works on MacBooks from the 2019 16-inch MacBook Pro onward; some M1/M2 models have sensor issues.

## Build

```shell
./scripts/package_dmg.sh 0.1.3   # dist/MacBookAccordion-0.1.3.dmg
```

Based on [samhenrigold/LidAngleSensor](https://github.com/samhenrigold/LidAngleSensor).
