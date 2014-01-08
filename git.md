# Git

## Make an existing branch point to HEAD [or another branch]

    git branch -f branch [commit]

This is exactly the same as:

    git checkout branch
    git reset --hard [commit]

without switching between branches.


## How to use git rebase --onto

    rebase --onto base parent-of-first-commit last-commit

Cut a series of commits and join it on "base", then check out "last-commit".
In other words, `git rebase --onto` rewrites the first commit
to make its parent to be "base".
