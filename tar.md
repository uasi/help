# tar

## Order of options in (BSD) tar

If you _compress_ files, put options _right after archive path._

```
tar czf foo.tar.gz --exclude=.svn foo1 foo2 foos/
```

If you _decompress_ a file, put options _at last._

```
tar xzfC foo.tar.gz out-dir --strip-components=1
```

## Excluding files

Use `--exclude=<file or dir>`. The given name is matched against for each entry
of every subdirectory.

## Decompressing into a specific directory

Use `C` with `--strip-components`.

```
tar xzfC foo.tar.gz out-dir --strip-components=1
```
