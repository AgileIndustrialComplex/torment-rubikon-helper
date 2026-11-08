# Torment Rubikon Helper

A single-file labyrinth scribe for marking out rooms and walking them, dressed in
Planescape: Torment bronze-on-stone.

Open `index.html` — no build step, no dependencies, no server needed.

## What it does

- **Infinite board.** Every square is a room with four sides; nothing is bounded.
- **Build mode.** Walk with WASD / arrows (or click a room). Entering a room reveals
  its walls and they stay revealed; the side you walk through opens as you pass.
  Click a wall — or the arrow pad — to open or close a side by hand.
- **Explore mode.** Walk the ways you opened. Only the passages you cut let you
  through; a blue guide line runs through the middles of the rooms to the Lobby, a
  red one to the Wizard room.
- **Names.** The Lobby is fixed at the origin. One room can be labelled
  *Nordom room* and one *Wizard room* — label a different room to move the name,
  click again to remove it.
- **Undo** (or Ctrl/Cmd+Z) steps back through every change: walls, moves, labels,
  mode switches, clearing.
- **Clear board** wipes the maze; **Seal everything** closes every passage.

Everything is kept in `localStorage`, so the board survives a reload.

## Hosting

Served straight from GitHub Pages: <https://agileindustrialcomplex.github.io/torment-rubikon-helper/>

The file also works from `file://` — just open it.