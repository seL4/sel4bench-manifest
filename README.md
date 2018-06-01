<!--
     Copyright 2017, Data61
     Commonwealth Scientific and Industrial Research Organisation (CSIRO)
     ABN 41 687 119 230.

     This software may be distributed and modified according to the terms of
     the BSD 2-Clause license. Note that NO WARRANTY is provided.
     See "LICENSE_BSD2.txt" for details.

     @TAG(DATA61_BSD)
-->
# sel4bench-manifest

Manifest of the seL4bench project, which contains a set of microbenchmarks for seL4.

# Getting the project

Use the repo tool as described on [the wiki](https://docs.sel4.systems/GettingStarted#get-googles-repo-tool)

    mkdir sel4bench
    cd sel4bench
    repo init -u https://github.com/seL4/sel4bench-manifest.git
    repo sync
    mkdir build
    cd build
    ../init-build.sh -DPLATFORM=sabre -DHARDWARE=TRUE -DAARCH32=TRUE -DRELEASE=TRUE -DFAULT=TRUE -DFASTPATH=TRUE
    ninja
