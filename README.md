> 🎮 [Play Live Demo](https://skadnrwhd-web.github.io/tower-of-hanoi-3d-2/) · 🪵 [Part 1 (3 pegs)](https://skadnrwhd-web.github.io/tower-of-hanoi-3d/) · ☕️ [Buy Me a Coffee](https://buymeacoffee.com/ujnam80)

# Tower of Hanoi 3D II · 4 Pegs

Part 2 of the wooden 3D Tower of Hanoi. This time there are **four pegs**, and the
shortest solution is no longer obvious. Part of my "algorithm toys" series.

## Features
- 4 pegs, 4 to 8 disks
- Shows the optimal move count (Frame-Stewart) and tells you when you hit it
- **Auto-solve**: watch the Frame-Stewart algorithm solve it move by move
- Classic / Random Shuffle / Chaos Mode
- Drag & drop with shadows and procedural wood texture
- Code panel lights up as you pick, check and drop a disk
- Best score saved on your device (localStorage)
- Mobile friendly (screen split into 4 touch zones)

## The algorithm
With 4 pegs the minimum number of moves is

`T(n) = min over k of ( 2·T(k) + 2^(n-k) - 1 )`

Move the top `k` disks to a spare peg using all 4 pegs, move the remaining `n-k`
disks with only 3 pegs, then bring the `k` disks back on top.
Optimal moves: 4 disks = 9, 5 = 13, 6 = 17, 7 = 25, 8 = 33.

## Support
☕️ [buymeacoffee.com/ujnam80](https://buymeacoffee.com/ujnam80)

## Tech
- Single `index.html`, no build tools, no server
- [Three.js](https://threejs.org/) via import map (unpkg CDN)
