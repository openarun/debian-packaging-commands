## This repository contains frequently used commands for packaging debian packages.

### How to create .deb file with dependency of a debian package.
`$ cd mypackage`

The following command will generate a .deb file which will contain all the depedencies as in the control file of that specific package.
`$ mk-build-deps`
