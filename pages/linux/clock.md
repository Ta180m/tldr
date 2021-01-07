# Clocking

> Change clock of various components

- Set CPU governor to performance:

`sudo cpupower frequency-set -g performance`

- Set CPU governor to powersave:

`sudo cpupower frequency-set -g powersave`

- Print dedicated GPU clocks

`sudo cpupower frequency-set -g performance`

- Reclock the dedicated GPU

`echo {{pstate}} | sudo tee /sys/kernel/debug/dri/1/pstate`
