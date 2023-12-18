# Identifier

Identifiers are in **camelCase** style, no matter whether it's a module name or a value name.

> Unlike most of other programming languages, identifiers here can start on a digit, or even be a number.

## Allowed characters
- English alphabet letters from `a` to `z`, uppercase or lowercase.
- Digits from `0` to `9`.

> An identifier can also be the same as any of language special keywords, such as `mod` or `let`.

## Examples
```
val thisIsValueName = 100
```
If an identifier is a special keyword or starts with a digit, its usage must contain `.` at the beginning (in most of the places, but not everywhere).
```
let
    val val = 5
in
    val hello = .val + 5 # 10 #

# a module called `mod` (special keyword) #
let mod mod where
    # module contents #
in
    # no need to put a period here #
    mod alias = mod

let val 3d = 1 + 1
in val bar = .3d * 10 # 20 #
```
Do not put a period `.` if an identifier is not at the beginning of a path:
```
let bar = this.is.path.3d
# NOT: this.is.path..3d #
```