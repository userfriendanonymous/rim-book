# Path

> A path consists of identifiers (module names), separated by `.`.

```
let
    mod this where
        mod is where
            mod a where
                mod path where
                    let value = 5
in
    mod alias = this.is.a.path
```

A path can also have a period (`.`) before it:
```
mod alias = .this.is.a.path
```
This is useful when dealing with some types of identifiers:
```
let
    val 10StartsWithDigit = 100
in
    val used = .10StartsWithDigit + 1 # 101 #
```