# Moon Patrol

DCPU game developed to honor the Moon Patrol for Atari 2600.

This game is proving grounds for DCPU usage in arcade games. Current version utilizes:

* double buffering
* parallax scrolling
  * pixel perfect
  * two layers
* dynamic font modification sprite
  * bullet
* static sprite animations
  * rover
  * enemy
* collision detection
  * rover - pit
  * bullet - enemy
* title screen with 64x48 lores-mode

Game loop uses about 1300-1600 cycles per frame. That leaves 4000+ (about 70%) of cpu capacity idle.
We could easily add more content (e.g. enemies, bullets) to the game without hittin cpu constraints,
and the routines are not even fully optimized yet.

 * 16 frames / second
 * 1300-1600 cycles per frame are used
 * 4000-5000 cycles per frame are free
 * 66 of 128 fonts are free

Key|Functionality
---|--------------
Left|Stop
Right|Move double speed
Up|Jump
Space|Fire

My personal High Score: 1450 :D
