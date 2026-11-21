# Sodor Steam Racers

A 3D kart-style racing game in the browser, where the racers are steam engines. The whole game lives in a single file, `index.html`; the 3D library it uses is in `vendor/three.min.js` and the recorded menu theme in `music/menu.js` (synthesized whistle exports are saved in `whistles/`).

## Play

Open `index.html` in a recent browser. The 3D library (three.js r128) is included in the `vendor` folder, so the game also works offline; if that folder is missing, the library is loaded from a CDN instead. The game can be played with a keyboard, a game controller or a touch screen; the in-game **How to play** screen lists every control.

| Keyboard | Controller | Action |
|---|---|---|
| Arrows / WASD | Stick / D-pad, RT or A, LT or B | Drive, accelerate, brake |
| Shift | RB or LB | Drift (a long drift gives a mini-turbo) |
| Space | X | Use item |
| H | Stick click / D-pad ↑ | Blow whistle |
| C | Y | Look back |
| R | Back | Back on the track |
| Esc or P | Start | Pause (resume, restart or quit) |
| M | | Music on / off |

On a touch screen, on-screen buttons appear: ◀ ▶ to steer (the engine accelerates by itself), and DRIFT, ITEM, WHISTLE and BRAKE on the right. For a rocket start, hold BRAKE during the countdown and let go just before GO. The menu has three screens: the game mode (with the saved season or cup to continue), then the engine, then the track or the cup and the difficulty. The arrow keys or the D-pad choose, Enter or A goes to the next screen (or starts the race), Esc or B goes back.

## Features

- **Fourteen engines**, modelled by type (tank engines, tender engines, a streamlined Pacific in an air-smoothed casing, the gold-lined Lady from the magic railroad, a tram, a diesel shunter, an electric), each with its own speed, acceleration and handling. Heavier engines push lighter ones aside.
- **Sixteen tracks**, each with three boost pads:
  - Sodor Meadows, Seaside Line, Quarry Run, Autumn Woods, Snowy Pass and Moonlight Yard (a night race);
  - Harbour Lights (at dusk, out along a pier to a lighthouse), Blossom Valley (cherry blossom and falling petals), Red Rock Canyon (switchbacks between mesas and cacti), Misty Moor (fast sweeping bends in the fog, round a stone circle), Lakeside Loop (round a lake with sailing boats), Timber Line (pine forest and log piles), Rainy Glen (a technical track in the rain), Harvest Fields (square farm roads, hay bales and windmills), Ironworks (smoking chimneys at dusk) and Starlight Summit (snow under the northern lights).
- **Four game modes**:
  - *Single Race* against seven other engines.
  - *Cup*, four races in a row for points on the four tracks of a cup: the Meadow Cup, Sea Breeze Cup, Wild Country Cup and Lamplight Cup, each mixing original and newer tracks. Finishing in the top three wins a gold, silver or bronze trophy, kept for each cup and each difficulty. A cup in progress is saved after every race, separately from the season.
  - *Season*, a championship over all sixteen tracks, saved automatically after every race so it can be continued later.
  - *Time Trial*, alone against the clock and against the ghost of your best run.
- **Three difficulty levels**: Easy, Normal, Hard. Computer engines pick their moment to use items and steer around oil slicks.
- **Driving skills**: rocket start on the signal lights, three-stage drift mini-turbos, slipstream behind other engines, boost pads.
- **Seven items**: Coal Boost, Triple Coal, Oil Slick, Runaway Truck, Whistle Blast, Buffer Shield and Red Signal.
- **Race screen**: signal-light countdown, speedometer, lap splits, wrong-way warning, minimap, and race statistics at the finish.
- **Engine Gallery**: browse all fourteen engines with 3D previews, characteristics (speed, acceleration, handling, weight), and interactive whistle playback.
- **Hall of Fame** per track, with the five best race times and the five best lap times, ranked separately for races (Single Race and Season) and for Time Trial.
- **Options**: Realistic or Cartoon graphics, three quality levels for slower computers, camera distance, music and sound-effect volumes.
- **Music**: a cheerful folk menu theme (accordion, tin whistle, guitar), recorded and looped (if `music/menu.js` is missing, a gentle synthesized theme plays instead), and original synthesized music in the races: a race theme arranged in a different style on each track (bouncy, calypso, rock, folk, sleigh bells, night swing, brass band, harp, western, pipes, reggae, bluegrass, organ jazz, barn dance, machine beat, music box) that speeds up on the final lap, and finish-line fanfares.
- **Synthesized sound effects**: a whistle of its own for every engine (a bell for Toby, horns for Diesel and Kana), steam chuffs paced by the wheels, rail-joint clatter, flange squeal when drifting, nearby rivals heard in stereo, and an ambience for each track (birds, waves and gulls, a foghorn, wind, crickets and owls, a cuckoo, a hawk, curlews, frogs, a woodpecker, rain and thunder, steam hissing in the works).

Season and cup saves, cup trophies, Hall of Fame times, ghosts, the driver name and all options are stored in the browser (`localStorage`), so they stay on the browser and computer where they were made.

## Disclaimer

This is an unofficial, non-commercial fan project. It is not affiliated with, endorsed by or connected to the owners of *Thomas & Friends*; character names belong to their respective owners.

## License

The code is released under the [MIT License](LICENSE). `vendor/three.min.js` is [three.js](https://threejs.org) r128, © three.js authors, also under the MIT License.

The menu theme in `music/menu.js` is AI-generated music: it was made with [ACE-Step 1.5](https://github.com/ace-step/ACE-Step-1.5) (MIT License) through Composer, from a text description of the style (no lyrics, no reference recording), then cut into a seamless loop.
