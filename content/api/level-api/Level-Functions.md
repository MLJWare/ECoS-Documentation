# Level Functions

## `NEW ()`
Adds a new entity to the level and returns it.

## `NEW (template)`
Adds a new entity to the level, with a copy of the components specified in the 
table `template` and returns the entity.

## `KILL (entity)`
Removes the entity `entity` from the level.

## `MAP (x, y)`
Returns the tile at tile position (`x`,`y`) in the level.

## `MAP (x, y, id)`
Sets the tile at tile position (`x`,`y`) in the level to index `id`, 
and returns the previous index of the tile.

## `LVL (x, y)`
Returns the tile at pixel position (`x`,`y`) in the level.

## `LVL (x, y, id)`
Sets the tile at pixel position (`x`,`y`) in the level to index `id`, 
and returns the previous index of the tile.

## `PIX (x, y)`
Returns the pixel at pixel position (`x`,`y`) in the level.

## `PIX (x, y, id)`
Returns the pixel at pixel position (x,y) in the sprite `id`.

## `FLG (id)`
Returns the bit flags of sprite `id` as a byte.

## `FLG (id, mask)`
Checks whether the bits in `mask` are also set in the bit flags of sprite `id`.

## `ALL (class, ...)`

Used in a for-loop to iterate over all entities with "non-false"-components 
associated with _ALL_ of the classes specified.
For each matching entity, the entity followed by each of the components for 
the specified classes will be returned.

Example:

```lua
for ent, pos, vel in ALL ("pos", "vel") do
  pos.x = pos.x + vel.x
  pos.y = pos.y + vel.y
end
```

## `ALL (t)`
Same as above, except using the elements in the array-like table `t` instead.

## `ANY (class, ...)`
Used in a for-loop to iterate over all entities with "non-false"-components 
associated with _ANY_ of the classes specified.
For each matching entity, the entity followed by the matched component and
its class will be returned.

Example:

```lua
for ent, timer, id in ANY ("delay", "count", "invincible") do
  timer.sec = timer.sec - DT
  if timer.sec <= 0 then
    ent[id] = nil -- removes the component from the entity
  end
end
```

## `ANY (t)`
Same as above, except using the elements in the array-like table `t` instead.

## `SETUP (fn1, ...)`
Adds the specified functions (`fn1`, ...) as setup-systems to the level.

## `SETUP (t)`
Same as above, except using the elements in the array-like table `t` instead.

## `UPDATE (fn1, ...)`
Adds the specified functions (`fn1`, ...) as update-systems to the level.

## `UPDATE (t)`
Same as above, except using the elements in the array-like table `t` instead.

## `DRAW (fn1, ...)`
Adds the specified functions (`fn1`, ...) as draw-systems to the level.

## `DRAW (t)`
Same as above, except using the elements in the array-like table `t` instead.

## `META (t)`
Returns the metatable of `t`.

## `META (t, meta)`
Sets the metatable of `t` to `meta` and returns the table `t`.

## `USE (filename)`
Loads the specified file, `filename`, and returns its content.
The value returned by `filename` is a function or table, the same function/table 
will be obtained from any subsequent call to `USE` by the same filename, 
even if used in different files (uses `/` as separator).

**NOTE**: _This function can only be called before the game runs, i.e. in the top scope. Calling it outside this scope results in an error message._
