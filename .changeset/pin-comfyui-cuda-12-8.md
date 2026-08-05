---
"worker-comfyui": minor
---

Pin ComfyUI to 0.29.0, build on CUDA 12.8, and pin the runtime PyTorch to 2.11.0+cu128 so the image runs on every host allowed by the Hub config. `allowedCudaVersions` in `.runpod/hub.json` moves from 12.6/12.7 to 12.8–13.0 (driver >= 570). Existing Hub endpoints keep the old release and its near-exhausted 12.6/12.7 host pool — update your endpoint to this release to pick up the new host range.
