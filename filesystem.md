# Filesystem commands

    # df - show mounted volumes
    # df stands for display free disk space
    # -h option prints size etc. in human-readable format
    $ df -h
    Filesystem                          Size   Used  Avail Capacity  iused    ifree %iused  Mounted on
    /dev/disk0s2                       315Gi  280Gi   34Gi    90% 73465562  8984122   89%   /
    devfs                              201Ki  201Ki    0Bi   100%      696        0  100%   /dev
    map -hosts                           0Bi    0Bi    0Bi   100%        0        0  100%   /net
    map auto_home                        0Bi    0Bi    0Bi   100%        0        0  100%   /home
    /dev/disk0s4                       150Gi   65Gi   85Gi    44%   238821 89246895    0%   /Volumes/BOOTCAMP
    localhost:/_Vp8qCKaG0rtL9mnwtvEnl  315Gi  315Gi    0Bi   100%        0        0  100%   /Volumes/MobileBackups

    # lsblk
    # -f option prints filesystem format
    $ lsblk -f
    ...
