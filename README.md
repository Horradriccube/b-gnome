# B-Gnome — Lawn Battle

A breakdancing garden gnome rhythm game in a single HTML file. No libraries, no image, model or sound files: the gnome is sculpted in code when the page loads, and the graphics and music are generated live in the browser (WebGL2 + Web Audio).

**Play:** open `index.html` in a browser, or visit the GitHub Pages link for this repo.

## How to play

The garden calls a move. Hit it on the beat to keep the crowd hyped. Survive the 2-minute track to become a Lawn Legend.

| Move | Keys | What he does |
|---|---|---|
| Six-Step | ← or 1 | Low footwork circling around his hands |
| Hat Spin | ↑ or 2 | Takes his hat off and spins on his bald head |
| Windmill | → or 3 | Rolls across his back, legs in a V |
| Flare | ↓ or 4 | Swings his legs in circles on his hands |

- Drag to orbit the camera, scroll or pinch to zoom.
- **Free dance** mode: no scoring, just moves.
- M mutes, P pauses. On phones, use the four on-screen buttons.

## Quality settings

Add to the address:

- `?q=low` / `?q=med` / `?q=high`: detail level (phones default to low)
- `?post=0`: turn off post-processing (bloom, ambient occlusion, depth of field)

The game also lowers its resolution automatically if the frame rate drops.

## How it's made

- **Gnome:** sculpted from signed-distance shapes, turned into a mesh at load time, skinned to a 19-bone rig, with baked crease shading and a weathered-ceramic material.
- **Rendering:** physically based lighting, soft shadow maps, HDR with ambient occlusion, bloom, sun rays, depth of field and filmic grading.
- **Garden:** about 40k grass blades and tens of thousands of instanced leaves, all drawn on the GPU.

Made with Claude.
