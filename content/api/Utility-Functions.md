# Utility functions

## `ITER (t)`

Used in a for-loop to iterate all (index, value)-pairs in an array-like table, `t`, in order.

## `PAIRS (t)`

Used in a for-loop to iterate all (key, value)-pairs in a table, `t`, in unspecified order.

## `TYPE (v)`

Returns the type of value `v` as a string. The returned value is one of `"number"`, `"string"`, `"table"`, `"function"`, or `"nil"`.

## `STR (v)`

Tries to convert `v` to a string and return it.

## `NUM (v)`

Tries to convert `v` to a number and return it. If `v` is not a number or a string representation of a number, the special value `nil` is returned instead.
