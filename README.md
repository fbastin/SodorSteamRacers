# Sodor Steam Racers

A 3D kart-style racing game in the browser, where the racers are steam engines. Everything lives in a single file, `index.html`.

## Play

Open `index.html` in a recent desktop browser. An internet connection is needed on load, because the 3D library (three.js r128) comes from a CDN. The game is played with the keyboard.

| Key | Action |
|---|---|
| Arrows / WASD | Drive |
| Shift | Drift (a long drift gives a mini-turbo) |
| Space | Use item |
| P | Pause |
| Esc | Back to menu |

## Features

- **Ten engines**, modelled by type (tank engines, tender engines, a tram, a diesel shunter, an electric), each with its own speed, acceleration and handling.
- **Six tracks**: Sodor Meadows, Seaside Line, Quarry Run, Autumn Woods, Snowy Pass and Moonlight Yard (a night race).
- **Three game modes**:
  - *Single Race* against seven other engines.
  - *Season*, a championship over all six tracks, saved automatically after every race so it can be continued later.
  - *Time Trial*, alone against the clock.
- **Three difficulty levels**: Easy, Normal, Hard.
- **Items**: Coal Boost, Oil Slick, Runaway Truck and Whistle Blast.
- **Hall of Fame** per track, with the five best race times and the five best lap times.
- **Two graphics styles**, Realistic and Cartoon, selectable in the menu.

Season saves, Hall of Fame times, the driver name and the graphics setting are stored in the browser (`localStorage`), so they stay on the browser and computer where they were made.

## Disclaimer

This is an unofficial, non-commercial fan project. It is not affiliated with, endorsed by or connected to the owners of *Thomas & Friends*; character names belong to their respective owners.
