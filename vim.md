# Vim

## :vimdiff

To compare two buffers, use `:diffthis` for both buffers.

## External commands

- `:{range}!{cmd} [arg]` Filter `{range}` lines through `{cmd}`

## Jump list

- `:ju[mp]` Print the jump list
- `CTRL-O   Go to `[count]` older cursor position
- `CTRL-I`  Go to `[count]` newer cursor position
- `CTRL-^`  Edit the previously edited file

## Deprecated commands, good for custom mappings

- `[f`, `]f`  Same as `gf` (edit the file whose name is under the cursor)

## Wrap existing text

```
:set textwidth=80
```
