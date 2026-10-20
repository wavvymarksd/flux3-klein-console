---
title: FLUX 3 Klein Console
emoji: 🎮
colorFrom: red
colorTo: gray
sdk: static
app_file: index.html
pinned: false
short_description: Retro 8-bit console demo for FLUX 3 Image Klein
models:
- black-forest-labs/flux-3-image-klein-comfy
- black-forest-labs/flux-3-image-klein
---

# FLUX 3 Klein Console 🎮

A dark, 8-bit home-console front-end for **FLUX 3 Image Klein**, the 5.6B open-weights
text-to-image and image-editing model from Black Forest Labs.

- Type a prompt into the cartridge slot and press **A** (or **START**) to generate.
- Load up to 4 reference images to edit or compose them.
- Pick **TURBO** (distilled, 16 steps) or **CLASSIC** (base, 50 steps).
- **B** inserts a random cartridge (example prompt).

The prompt upsampler always runs first, so short prompts are fine. The expanded caption
that the model actually saw is printed on the screen afterwards.

## How it runs

This is a static Space. Your browser sends each request with
[`@gradio/client`](https://www.npmjs.com/package/@gradio/client) to the official
[black-forest-labs/flux-3-image-klein](https://huggingface.co/spaces/black-forest-labs/flux-3-image-klein)
Space, which runs the weights repackaged in
[flux-3-image-klein-comfy](https://huggingface.co/black-forest-labs/flux-3-image-klein-comfy)
(the same checkpoints, also available for ComfyUI). Generations use the visitor's ZeroGPU quota.

The model is released under the FLUX Kommunity License. FLUX and Black Forest Labs are trademarks
of Black Forest Labs; this fan demo is not affiliated with or endorsed by them.
