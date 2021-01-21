# PRIME

> Manage hybrid graphics.
> More information: <https://wiki.archlinux.org/index.php/PRIME>.
> Also see `clock`.

- Run application on dedicated GPU:

`DRI_PRIME=1 {{application_name}}`

- Check status of dedicated GPU:

`sudo cat /sys/kernel/debug/vgaswitcheroo/switch`
