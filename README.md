Boot with EFI stub kernel.

Get more information from [EFI stub kernel](https://wiki.gentoo.org/wiki/EFI_stub_kernel).

Generate basic config

    make savedefconfig

Restore from basic config

    cp /path/your-defconfig .config
    make olddefconfig
    make menuconfig
    ......
    make -j$((`nproc`+1)) && make modules_install

More: <https://wiki.gentoo.org/wiki/Kernel/Configuration>
