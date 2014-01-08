# Perl

## Frequently-used switches

- `-a`: with `-n` or `-p`, turns on autosplit mode
- `-F`: specify an alternate delimiter for `-a`
- `-l`: auto-chomp each line when used with `-n` or `-p`
- `-n`: `while (<>) { Your program here... }`
- `-p`: like `-n` but print each line

## Idiomatic switch usages

To modify a file in-place, use this:

    perl -lni -e 's///' file

Use Perl like an alternative to Awk:

    perl -lna -e '...' file
