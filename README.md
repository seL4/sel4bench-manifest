<!--
     Copyright 2017, Data61, CSIRO

     SPDX-License-Identifier: CC-BY-SA-4.0
-->

# sel4bench-manifest

Manifest of the `seL4bench` project, which contains a set of microbenchmarks for seL4.

# Getting the project

Use the `repo` tool as described on [the seL4 docsite][repo].

    mkdir sel4bench
    cd sel4bench
    repo init -u https://github.com/seL4/sel4bench-manifest.git
    repo sync
    mkdir build
    cd build
    ../init-build.sh -DPLATFORM=sabre -DHARDWARE=TRUE -DAARCH32=TRUE -DRELEASE=TRUE -DFAULT=TRUE -DFASTPATH=TRUE
    ninja


[repo]: https://docs.sel4.systems/projects/buildsystem/host-dependencies.html#get-googles-repo-tool