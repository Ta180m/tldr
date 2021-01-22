# Clocking

> Change clock of various components

- List available CPU governors:

`cat /sys/devices/system/cpu/cpufreq/policy?/energy_performance_available_preferences`

- Print current CPU governor:

`cat /sys/devices/system/cpu/cpu*/cpufreq/scaling_governor`

- Set CPU governor to performance:

`sudo cpupower frequency-set -g performance`

- Set CPU governor to powersave:

`sudo cpupower frequency-set -g powersave`

- Print dedicated GPU clocks:

`sudo cat /sys/kernel/debug/dri/1/pstate`

- Reclock the dedicated GPU:

`echo {{pstate}} | sudo tee /sys/kernel/debug/dri/1/pstate`
