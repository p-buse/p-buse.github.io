---
layout: game
title: Break
date: 2014-04-26
permalink: /games/break/
description: Time-looping rectangle platformer!
image: /images/screenshots/break_128.png
video: https://www.youtube.com/watch?v=dQw4w9WgXcQ
basename: break
game_memory: 268435456
canvas_width: 960px
canvas_height: 600px
controls: >
    <p><kbd>←</kbd> <kbd>→</kbd> or <kbd>A</kbd> <kbd>D</kbd> - Move</p>
    <p><kbd>↑</kbd> or <kbd>W</kbd> - Jump</p>
    <p><kbd>↓</kbd> or <kbd>S</kbd> - Switch Player</p>
    <p><kbd>R</kbd> - Reset Loop</p>
---

I made Break to learn Unity and because I was interested in loop-based music at the time. Break grew out of [#1GAM's][1gam] February 2014 theme, LOOPING. I took on more than I could finish in a month, so I made it a semester-long project. You play as three colored rectangles (no, I had not played [Thomas Was Alone][thomas] at the time) trying to escape an infinite loop. The game is named for the [command in computer programming that exits a loop][break-wiki]. Any action you take is recorded and will loop ad infinitum, or until you overwrite the loop. The toughest part was programming the looping. It works by capturing your input at a fixed update and playing back the captured input for the two players you don't have selected.

The [source is on GitHub][break-source].

[1gam]: http://www.onegameamonth.com/
[thomas]: http://www.mikebithellgames.com/thomaswasalone/
[break-wiki]: http://en.wikipedia.org/wiki/Control_flow#Early_exit_from_loops
[break-source]: https://github.com/p-buse/break
