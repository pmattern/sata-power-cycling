# SATA power cycling

The SATA port of several embedded devices, e. g. Cubietruck, gets power-cycled during reboot.
The kernel (rightly) doesn't expect this behaviour which hence ends in emergency parking of HDD heads.

This repository provides some patches mitigating the problem by triggering the same HDD shutdown that's normally
performed during system shutdown only when devices get rebooted as well.

Preliminary repo to provide the patches when building binary distro packages, future undecided.
