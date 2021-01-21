# yay

> Yet Another Yogurt: A utility for Arch Linux to build and install packages from the Arch User Repository.
> A frontend to `pacman`.

- Synchronize and update all packages from the repos and AUR:

`yay`

- Interactively search and install packages from the repos and AUR:

`yay {{package_name|search_term}}`

- Install a new package from the repos and AUR:

`yay -S {{package_name}}`

- Search the package database for a keyword from the repos and AUR:

`yay -Ss {{keyword}}`

- Get information about a package:

`yay -Si {{package_name}}`

- Clean the package cache:

`yay -Sc`

- Completely wipe the package cache:

`yay -Scc`

- Uninstall a package and delete config files:

`yay -Rns {{package_name}}`

- Install a local package (useful for rolling back updates):

`yay -U /var/cache/pacman/pkg/{{package_name}}`

- Find out which package owns a file:

`yay -Qo {{file_name}}`

- List files contained in a package:

`yay -Ql {{package_name}

- List all explicitly installed packages (includes AUR packages):

`yay -Qe`

- Save all explicitily installed packages to a file:

`yay -Qe | awk '{print $1}' > packages.txt`

- Remove unneeded dependencies:

`yay -Yc`

- Show statistics for installed packages and system health:

`yay -Ps`
