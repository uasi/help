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

## See unpushed commits

If you want to see all commits on all branches that aren't pushed yet, you might be looking for something like this:

    git log --branches --not --remotes

And if you only want to see the most recent commit on each branch, and the branch names, this:

    git log --branches --not --remotes --simplify-by-decoration --decorate --oneline

via http://stackoverflow.com/a/3338774/454997
