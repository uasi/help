# SSH

## Print SSH key fingerprint

    ssh-keygen -l -f /path/to/key

## Generate public key from private key

    ssh-keygen -y -f /path/to/key

## Escape secuences

Press Enter, then `~`, then `?`. This shows the list of escape secuences supported by your local SSH client.
