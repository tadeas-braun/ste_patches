**STE patches for CM-11.0**

Patch android source code :

    patch -p1 < ste_patches/framework_av.patch
    patch -p1 < ste_patches/framework_native.patch
    patch -p1 < ste_patches/framework_base.patch
    patch -p1 < ste_patches/hardware_libhardware.patch
    patch -p1 < ste_patches/hardware_libhardware_legacy.patch
    patch -p1 < ste_patches/system_core.patch
    patch -p1 < ste_patches/bionic.patch
    patch -p1 < ste_patches/bootable_recovery.patch
    patch -p1 < ste_patches/external_bluetooth_bluedroid.patch

Revert each patch before syncing the source :

    patch -p1 -R < ste_patches/framework_av.patch
    patch -p1 -R < ste_patches/framework_native.patch
    patch -p1 -R < ste_patches/framework_base.patch
    patch -p1 -R < ste_patches/hardware_libhardware.patch
    patch -p1 -R < ste_patches/hardware_libhardware_legacy.patch
    patch -p1 -R < ste_patches/system_core.patch
    patch -p1 -R < ste_patches/bionic.patch
    patch -p1 -R < ste_patches/bootable_recovery.patch
    patch -p1 -R < ste_patches/external_bluetooth_bluedroid.patch
    repo sync
    patch -p1 < ste_patches/framework_av.patch
    patch -p1 < ste_patches/framework_native.patch
    patch -p1 < ste_patches/framework_base.patch
    patch -p1 < ste_patches/hardware_libhardware.patch
    patch -p1 < ste_patches/hardware_libhardware_legacy.patch
    patch -p1 < ste_patches/system_core.patch
    patch -p1 < ste_patches/bionic.patch
    patch -p1 < ste_patches/bootable_recovery.patch
    patch -p1 < ste_patches/external_bluetooth_bluedroid.patch

