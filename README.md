# Sodor Steam Racers

A 3D kart-style racing game in the browser, where the racers are steam engines. The whole game lives in a single file, `index.html`; the only other file is the 3D library it uses, `vendor/three.min.js`.

## Play

Open `index.html` in a recent browser. The 3D library (three.js r128) is included in the `vendor` folder, so the game also works offline; if that folder is missing, the library is loaded from a CDN instead. The game can be played with a keyboard, a game controller or a touch screen; the in-game **How to play** screen lists every control.

| Keyboard | Controller | Action |
|---|---|---|
| Arrows / WASD | Stick / D-pad, RT or A, LT or B | Drive, accelerate, brake |
| Shift | RB or LB | Drift (a long drift gives a mini-turbo) |
| Space | X | Use item |
| C | Y | Look back |
| R | Back | Back on the track |
| Esc or P | Start | Pause (resume, restart or quit) |
| M | | Music on / off |

On a touch screen, on-screen buttons appear: ◀ ▶ to steer (the engine accelerates by itself), and DRIFT, ITEM and BRAKE on the right. For a rocket start, hold BRAKE during the countdown and let go just before GO. In the menu, the arrow keys or the D-pad choose the engine (← →) and the track (↑ ↓).

## Features

- **Eleven engines**, modelled by type (tank engines, tender engines, a tram, a diesel shunter, an electric), each with its own speed, acceleration and handling. Heavier engines push lighter ones aside.
- **Six tracks**: Sodor Meadows, Seaside Line, Quarry Run, Autumn Woods, Snowy Pass and Moonlight Yard (a night race), each with three boost pads.
- **Three game modes**:
  - *Single Race* against seven other engines.
  - *Season*, a championship over all six tracks, saved automatically after every race so it can be continued later.
  - *Time Trial*, alone against the clock and against the ghost of your best run.
- **Three difficulty levels**: Easy, Normal, Hard. Computer engines pick their moment to use items and steer around oil slicks.
- **Driving skills**: rocket start on the signal lights, three-stage drift mini-turbos, slipstream behind other engines, boost pads.
- **Seven items**: Coal Boost, Triple Coal, Oil Slick, Runaway Truck, Whistle Blast, Buffer Shield and Red Signal.
- **Race screen**: signal-light countdown, speedometer, lap splits, wrong-way warning, minimap, and race statistics at the finish.
- **Hall of Fame** per track, with the five best race times and the five best lap times, ranked separately for races (Single Race and Season) and for Time Trial.
- **Options**: Realistic or Cartoon graphics, three quality levels for slower computers, camera distance, music and sound-effect volumes.
- **Original synthesized music**: a gentle menu theme, a race theme arranged in a different style on each track (bouncy, calypso, rock, folk, sleigh bells, night swing) that speeds up on the final lap, and finish-line fanfares.
- **Synthesized sound effects**: a whistle of its own for every engine (a bell for Toby, horns for Diesel and Kana), steam chuffs paced by the wheels, rail-joint clatter, flange squeal when drifting, nearby rivals heard in stereo, and an ambience for each track (birds, waves and gulls, wind, crickets and owls).

Season saves, Hall of Fame times, ghosts, the driver name and all options are stored in the browser (`localStorage`), so they stay on the browser and computer where they were made.

## Disclaimer

This is an unofficial, non-commercial fan project. It is not affiliated with, endorsed by or connected to the owners of *Thomas & Friends*; character names belong to their respective owners.

## License

The code is released under the [MIT License](LICENSE). `vendor/three.min.js` is [three.js](https://threejs.org) r128, © three.js authors, also under the MIT License.
