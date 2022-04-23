# Graphics API

## `PNT (x, y, ...)`
Draws a point/pixel at position (`x`, `y`) on the screen;
additional argument pairs will be used as additional (x,y) positions to draw at.

## `LINE (x1, y1, x2, y2, ...)`
Draws a line from (`x1`,`y1`) to (`x2`,`y2`); 
additional argument pairs will be used to draw additional lines, starting from 
the previous set of coordinates.

## `CIRC (x, y, radius)`
Draws a circular border, with a center at (`x`,`y`), and a radius or `radius`.

## `DISC (x, y, radius)`
Fills a circular area, with a center at (`x`,`y`), and a radius or `radius`.

## `RECT (x, y, width, height)`
Draws a rectangular border starting a (`x`, `y`), with a width of `width` and 
a height of `height`.

## `FILL (x, y, width, height)`
Fills a rectangular area starting a (`x`, `y`), with a width of `width` and a 
height of `height`.

## `CLR ()`
Clears the display.

## `CLR (x, y, width, height)`
Clears a rectangular area of the display, starting at (`x`, `y`),
with a width of `width` and a height of `height`.

## `SPR (id, x, y)`
Draws a $4 \times 8$ sprite with index `id` at position (`x`,`y`).

## `SPR (id, x, y, fx, fy)`
Draws a $4 \times 8$ sprite with index `id` at position (`x`,`y`);
set `fx` to `true` to flip the sprite horizontally, 
set `fy` to `true` to flip the sprite vertically.

## `SPR (id, x, y, fx, fy, clear)`
Draws a $4 \times 8$ sprite with index `id` at position (`x`,`y`);
set `fx` to `true` to flip the sprite horizontally, 
set `fy` to `true` to flip the sprite vertically, 
set `clear` to `true` to clear the area behind the sprite.

## `TILE (id, x, y)`
Draws a $8 \times 8$ tile with index `id` at position (`x`,`y`).

## `TILE (id, x, y, fx, fy)`
Draws a $8 \times 8$ tile with index `id` at position (`x`,`y`);
set `fx` to `true` to flip the tile horizontally, 
set `fy` to `true` to flip the tile vertically.

## `TILE (id, x, y, fx, fy, clear)`
Draws a $8 \times 8$ tile with index `id` at position (`x`,`y`);
set `fx` to `true` to flip the tile horizontally, 
set `fy` to `true` to flip the tile vertically, 
set `clear` to `true` to clear the area behind the tile.

## `SLAB (id, x, y)`
Draws a $16 \times 16$ slab with index `id` at position (`x`,`y`).

## `SLAB (id, x, y, fx, fy)`
Draws a $16 \times 16$ slab with index `id` at position (`x`,`y`);
set `fx` to `true` to flip the slab horizontally, 
set `fy` to `true` to flip the slab vertically.

## `SLAB (id, x, y, fx, fy, clear)`
Draws a $16 \times 16$ slab with index `id` at position (`x`,`y`);
set `fx` to `true` to flip the slab horizontally, 
set `fy` to `true` to flip the slab vertically, 
set `clear` to `true` to clear the area behind the slab.

## `TXT (str, x, y)`
Draws the string `str` at position (`x`, `y`).

## `TXT (str, x, y, clear)`
Draws the string `str` at position (`x`, `y`);
set `clear` to `true` to clear the area behind the text.

## `WB ()`
Changes the rendering mode to white-on-black (default mode is black-on-white), 
i.e. sets the background color to white and the drawing color to black.

## `BW ()`
Changes the rendering mode to black-on-white (the default mode), 
i.e. sets the background color to black and the drawing color to white.

## `IWB ()`
Toggles the rendering mode between black-on-white and white-on-black.

