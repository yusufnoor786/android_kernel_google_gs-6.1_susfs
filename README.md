# SUSFS guard LKM (from KernelSU-Next v3.4.2) for the Pixel 6a gs-6.1 kernel tree

`susfs_guard_lkm.ko` sources from KernelSU-Next v3.4.2 `kernel/susfs`, packaged as a Kleaf
`kernel_module`. Place at `private/google-modules/susfs` and build:

    tools/bazel build --config=bluejay //private/google-modules/susfs:susfs

Built with `KBUILD_MODPOST_WARN=1`; load with `ksud susfs load` (note: `ksud` loads its own embedded
module, not this one). Not tested as a standalone load on the phone.
Licence: GPL-2.0. Upstream: https://github.com/KernelSU-Next/KernelSU-Next
