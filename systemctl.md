# Systemctl

```
$ systemctl restart <unit> # restart <unit>
$ systemctl reload <unit>  # make <unit> reloads its own config file
```

Enable your unit file:

```
ln -s myunit /etc/systemd/system/$target.wants
```
