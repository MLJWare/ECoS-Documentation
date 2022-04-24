# Terminal Commands

## `HELP [cmd]`
Shows help info for `[cmd]` if specified; otherwise, prints list of commands.

## `EXIT`
Terminates ECoS.

## `BUILD <code> [cart]`
Creates a cartridge, `[cart]`, (defaults to same as `<code>`)
by bundling existing sprites, sounds, etc. with the given code file, `<code>`.

## `MOUNT <cart> [code]`
Mounts a cartridge, `<cart>`, by loading it into RAM.
The cartridge code will be stored in the folder `[code]` (defaults to 'CART').

## `CLEAR`
Clears the Terminal.

## `SYNTH`
Opens the Synthesizer/Waveform Editor.

## `LEVEL`
Opens the Level/Map Editor.

## `IMAGE`
Opens the Image/Sprite Editor.

## `RUN <file> ...`
Runs the code in `<file>`, passing any additional arguments to the code.

## `EDIT <filename>`
Opens the Code Editor with the file `<file>`.

## `CP <file1> <file2>`
Copies the content of `<file1>` into `<file2>`.

## `MKDIR <foldername>`
Creates a new code folder named `<foldername>`.

## `RM <name>`
Removes the file `<name>`. Can also be used to remove empty folders.

## `LS [start] [folder]`
Lists all elements in `[folder]` (defaults to code root), starting with `[start]`.

## `CARTS [start]`
Lists all cartridges starting with `[start]`.

## `CARTSDIR`
Opens the cartridges folder in the native system file explorer.

## `MEMCLR [start] [size]`
Clears the memory.  
If `[start]` is specified, memory will be cleared starting at this address.  
If `[size]` is specified, at most this many bytes will be cleared in memory.

## `MEMCPY <start> <size> <index>`
Copies a chunk of memory, of at most `<size>` bytes from address `<start>` to
address `<index>`.

**NOTE**: 
The arguments to `MEMCLR` and `MEMCPY` both accept basic arithmetic
expressions consisting of `+ - * /` operations, parentheses, as well as the following symbolic addresses:

* `FONT`  : Memory address of the first character of the text font.
* `#FONT` : Size of a single font character, in bytes.
* `GFX`   : Memory address of the internal graphics sprites.
* `#GFX`  : Size of a single internal graphics sprite.
* `SPR`   : Memory address of the first user editable sprite.
* `#SPR`  : Size of a single user editable sprite, in bytes (including the bit flags).
* `LVL`   : Memory address of the first tile in the level.
* `#LVL`  : Size of the entire level, in bytes.
* `SFX`   : Memory address of the first user definable sound effect/melody.
* `#SFX`  : Size of a single user definable sound effect/melody, in bytes.
