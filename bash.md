# Bash

## Style

https://github.com/progrium/bashstyle

http://mywiki.wooledge.org/Quotes

## Extended globbing

See http://www.linuxjournal.com/content/bash-extended-globbing

To enable extended glob, `shopt -s extglob` or exec bash with `-O extglob`.

    ?(pattern-list)   Matches zero or one occurrence of the given patterns
    *(pattern-list)   Matches zero or more occurrences of the given patterns
    +(pattern-list)   Matches one or more occurrences of the given patterns
    @(pattern-list)   Matches one of the given patterns
    !(pattern-list)   Matches anything except one of the given patterns

`dir/!(*.gz)` matches everything but .gz files _in the dir directory_.

## Pitfalls

Don't do `*!(.jpg|gif)`, do `!(*.jpg|*.gif)`.

## Get dirname

`$(cd "$(dirname "$BASH_SOURCE")"; pwd)`
