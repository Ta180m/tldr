# Clocking

> Change clock of various components

- Print dedicated CPU clocks:

`cat /sys/devices/system/cpu/cpu*/cpufreq/scaling_governor`

- Set CPU governor to performance:

`sudo cpupower frequency-set -g performance`

- Set CPU governor to powersave:

`sudo cpupower frequency-set -g powersave`

- Print dedicated GPU clocks (first card):

`sudo cat /sys/kernel/debug/dri/0/pstate`

- Reclock the dedicated GPU:

`echo {{pstate}} | sudo tee /sys/kernel/debug/dri/0/pstate`
