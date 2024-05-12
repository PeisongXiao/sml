# SML - Script Markup Language
SML is a markup language specifically designed for network narrative scripting. The project aims to reduce duplicated workloads, provide intuitive control over the flow of the story, and be able to integrate into other programming languages.

## Basic syntax
### Identifiers
Identifiers can only contain alphanumeric characters and `_` and `-`.
### Names
Defined and/or used by `[name]` in front of a line.
### Line
A single line of text that starts with a `name` or nothing, representing a single line of dialoge.
### Jump tags
Defined by `|tag|`, and jumped to by `>tag`.
### Flags
Defined by an identifier, defaults to `off` when first accessed.

To turn a flag on, use `+flag`; to turn it off, use `-flag`; to toggle it, use `^flag`.

### Values
Defined by an identifier, stores an integer value. Denoted by `:value`.

### Signals
Signals that can be sent to the user. A list of signals with their associated values will be generated during preprocessing of the script.

Signals are sent by `!signal`.

### Blocks
Enclosed by `{}`, things within will be treated as a single line.

### Conditions
Conditions are used in the form of `?expression: TODO`.

### Imports
Modules can be imported by `~PATH_TO_FILE`.
