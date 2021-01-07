# Memory management

> Commands for managing memory.

- Clear swap:

`sudo swapoff -a && sudo swapon -a`

- Clear caches:

`echo 3 | sudo tee /proc/sys/vm/drop_caches`
