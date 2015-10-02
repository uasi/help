# Key Bindings

- `Esc-.` or `Esc-_`: insert the last word of the previous command

# Parameter expansion: ${foo HERE}

See `man zshexpn` for "PARAMETER EXPANSION"

# Parameter expansion flags: ${(HERE)foo}

See `man zshexpn` for "Parameter Expansion Flags"

- `${(z)foo}`: split the result of the expansion into words
- `${(q)foo}`: quote metachars by backslash
- `"${(@f)foo}"`: split the value by newline (f) and expand it like `"$@"` (@)

# Parameter expansion using history modifier: ${foo:HERE}

- `${foo:h}`: same as `dirname` (h for Head)
- `${foo:t}`: same as `basename` (t for Tail)
- `${foo:r}`: drop exention (r for Root)

# References

- http://qiita.com/mollifier/items/26a9ddcb7470f539e575
