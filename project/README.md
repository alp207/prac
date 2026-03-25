# Dragon Duel Arena

This project now includes a fresh static front end that uses `dragon.png` as the in-game dragon image.

## Files

- `index.html`: page shell and UI
- `styles.css`: layout and visual styling
- `game.js`: dragon-only 1v1 arena logic
- `dragon.png`: dragon sprite used in the arena
- `render.yaml`: Render static site blueprint

## Gameplay

- Click `Play` to spawn directly as a dragon.
- Move by aiming with the mouse.
- Hold left click or press `Space` to boost.
- On mobile, drag inside the arena to steer and use the on-screen `Boost` button.

## Render

This build is set up as a static site, so deploy it to Render as a `Static Site` or by using the included `render.yaml`.

If you create it manually in Render:

- Service Type: `Static Site`
- Build Command: `echo "Static dragon arena ready"` (or leave it blank)
- Publish Directory: `.`
- Environment Variable: `SKIP_INSTALL_DEPS=true`

If Render says it can't find `package.json`, it is usually doing dependency auto-detection or the service was created as a regular Web Service. Recreate it as a Static Site, or keep the included `render.yaml` and let Render create the service from that blueprint.
