# Shipped 3D models

Runtime models live here and are loaded by URL. The folder is intentionally
empty in the current build: the game uses the procedural athlete and needs no
model file to run.

```
public/models/
  volt-athlete.glb   rig plus the 16 gameplay clips
```

Models are tracked in Git LFS (see `.gitattributes`). When a model is added:

1. Record it in `ASSET_CREDITS.md`.
2. Keep it under 2 MB — the initial download budget is 20 MB.
3. Confirm the procedural fallback still works with the model absent.
4. Enable the `useSkinnedModels` preference and check every clip in game.
