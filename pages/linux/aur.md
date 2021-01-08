# Maintaining AUR packages

> Maintaining packages on the Arch User Repository
> More information: <https://wiki.archlinux.org/index.php/AUR_submission_guidelines>

- Clone the PKGBUILD to a local repository:

`git clone ssh://aur@aur.archlinux.org/{{package_name}}.git`

- Build the package:

`makepkg -s`

- Update .SRCINFO:

`makepkg --printsrcinfo > .SRCINFO`

- Commit and push changes:

`git add PKGBUILD .SRCINFO; git commit; git push`
 
