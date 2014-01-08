# Rsync

    # Archive mode, verbose[, dry-run]
    rsync -av[n] srcdir dstdir
    
    rsync -a srcdir  dstdir # Copy srcdir in dstdir
    rsync -a srcrir/ dstdir # Copy contents of srcdir in dstdir
    
    rsync user@host:srcdir dstdir
    rsync srcdir user@host:srcdir
    
    # Copy nothing but subtree rooted to foodir
    # `dir_name/***` means "directory itself and all of its contents"
    rsync -a --exclude='*' --include='/foodir/***' srcdir dstdir

