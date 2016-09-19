# sel4bench-manifest

Manifest of the seL4bench project, which contains a set of microbenchmarks for seL4.

# Getting the project

Use the repo tool as described on [the wiki](https://wiki.sel4.systems/Getting%20started#Get_Google.27s_.22Repo.22_tool)

    mkdir sel4bench
    cd sel4bench
    repo init -u https://github.com/seL4/sel4bench-manifest.git
    repo sync
    make sabre_release_O2_defconfig # replace with platform of your choice
    make oldconfig
    make
