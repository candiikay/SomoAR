# Pocket Garden – WebXR (No Unity)

A minimal, install‑free AR garden built with **WebXR + Three.js**. Tap to place stylized plants on detected surfaces. Uses WebXR hit‑test and optional anchors (if supported) with simple localStorage save/restore.

## Run
- Serve over **HTTPS** or `http://localhost` (Chrome treats localhost as secure).
- Use **Chrome on Android** for the widest WebXR AR support. iOS Safari AR support is limited.
- Host the folder or run a local server (e.g., `python3 -m http.server`), then open `index.html`.

## Features
- WebXR immersive‑AR session via Three.js `ARButton`.
- Surface **hit‑test** and reticle placement.
- Tap to plant (3 plant types).
- **Anchors** if the device supports them; otherwise places relative to the current session origin.
- **Save** layout to localStorage; **Restore** relative to the current origin; **Clear** saved.
- Simple growth animation over time.

## Notes on Persistence
Without VPS/Geo, exact real‑world re‑localization across *separate* sessions is not guaranteed.
This starter:
- Saves transforms; restores **relative** to the new session origin.
- If anchors are available, items follow anchors during the session for better stability.
- For “same spot next day” behavior on the **web**, you would need a VPS provider (e.g., 8th Wall/Niantic).

## Customize
- Replace the `makePlant()` factory with your own GLTF models (use `GLTFLoader`).
- Add watering/harvesting UI and growth state to the save blob.
- Swap localStorage for IndexedDB for richer save data.

## Credits
- Three.js & WebXR.
