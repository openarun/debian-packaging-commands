## This repository contains frequently used commands for packaging of debian sources.

### How to create .deb file with dependency of a debian source.
`$ cd mypackage`

The following command will generate a .deb file which will contain all the depedencies as in the control file of that specific package.

`$ mk-build-deps`

### Build package with GBP + sbuild.

Without signing your package with GPG key:

`$ gbp buildpackage --git-builder=sbuild -v -d experimental`

To sign your package with your GPG key :

`$ gbp buildpackage --git-builder=sbuild -v -d experimental -k [GPG-Key]`
