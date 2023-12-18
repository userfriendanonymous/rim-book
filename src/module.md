# Module
`mod` keyword defines a new module.
```
mod bar where
    # contents #
```

Modules can be defined in three ways:

## Where
```
mod <name> where
    # contents #
```
Defines an new module with given items.

## File
```
mod <name> file <file_name>
```
Defines a module in another file.

#### Example
File `main.rim`
```
mod bar file bar
```
File `main/bar.rim`:
```
val foo = 1 + 2
```

## Alias
```
mod <name> = <path>
```
#### Example
```
mod alias = path.to.another.module
```