# General Math Functions

## `FLR (n)`
Returns the number `n` rounded down to the nearest integer.

## `CEIL (n)`
Returns the number `n` rounded up to the nearest integer.

## `RUND (n)`
Returns the number `n` rounded up/down to the nearest integer.

## `SIGN (n)`
Returns the sign of the number `n`, i.e. returns 1 if `n` is positive, 0 
if `n` is zero, or -1 if `n` is negative.

## `ABS (n)`
Returns the absolute, or non-negative value, of the number `n`.

## `CLMP (n, min, max)`
Clamps the number `n` to a value between `min` and `max`, both inclusive.
Same as `MIN (MAX (min, n), max)` (see below).

## `OVFW (n, min, max)`
Warps `n` to a value between `min` and `max`, both inclusive.
Same as `((n - min) % (1 + max - min)) + min`.

## `MIN (a,...)`
Takes a sequence of numbers and returns the smallest value.

## `MAX (a,...)`
Takes a sequence of numbers and returns the largest value.

## `AVG (a,...)`
Takes a sequence of numbers and returns their average.

## `DIV (a,b)`
Integer division; returns the integer component of dividing `a` with `b`.

## `DST2 (x1, y1, x2, y2)`
Returns the squared euclidean distance between (`x1`,`y1`) and (`x2`,`y2`).

## `DIST (x1, y1, x2, y2)`
Returns the euclidean distance between (`x1`,`y1`) and (`x2`,`y2`).

## `DEG (rad)`
Converts from radians to degrees.

## `RAD (deg)`
Converts from degrees to radians.

## `EXP (n)`
Returns the exponential function applied to the number `n`.

## `LN (n)`
Returns the natural logarithm applied to the number `n`.

## `LG (n)`
Returns the base 2 logarithm applied to the number `n`.

## `LOG (n)`
Returns the base 10 logarithm applied to the number `n`.

## `SQRT(n)`
Returns the square root of the number `n`.

