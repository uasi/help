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

## Find merge commit which include a specific commit

With git-when-merged:

    # Prereq: brew install git-when-merged
    # For available options, try `git-when-merged --help`, not `git when-merged --help`

    git when-merged [-l] <commit>

Or without it:

    git log <specific-commit>..master --ancestry-path --merges --reverse

via http://stackoverflow.com/questions/8475448/find-merge-commit-which-include-a-specific-commit

On --ancestry-path, it is that:

> When given a range of commits to display (e.g.  commit1..commit2 or commit2 ^commit1), only display commits that exist directly on the ancestry chain
> between the commit1 and commit2, i.e. commits that are both descendants of commit1, and ancestors of commit2.

## Caveats on log -G

It seems it cannot find changes introduced in a merge commit.

    Running `git log -G RAW_BODY_MAXIMUM_LENGTH` in increments/Qiita prints two commits,
    but another commit 14ffb4bea180fdce77762ac6b52230a2ac7796c0 does contain a change on
    RAW_BODY_MAXIMUM_LENGTH.
