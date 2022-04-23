# Input API

In the following functions, `key` must be one of the strings:

* `"L"` : indicates the left-arrow/A key, 
* `"R"` : indicates the right-arrow/D key,
* `"U"` : indicates the up-arrow/W key,
* `"D"` : indicates the down-arrow/S key,
* `"1"` : indicates the Z/C/space key, and
* `"2"` : indicates the X/return key.

## `KEY (key)`
Returns whether the key `key` is currently being held down.

## `KEYN (key)`
Returns whether the key `key` was pressed since the last frame.

## `IKEY (key)`
Integer version of `KEY`; returns 1 if the key is held, 0 otherwise.

## `IKEYN (key)`
Integer version of `KEYN`; returns 1 if the key was pressed since last frame, 
0 otherwise.

