# chroot-rpi-image
Chroot to a raspberry pi image from your x86 PC using QEMU

* Compile a new static linked version of qemu:
`./configure --target-list=aarch64-linux-user,arm-linux-user --enable-avx2 --disable-bsd-user --disable-guest-agent --disable-strip --disable-werror --disable-gcrypt --disable-debug-info --disable-debug-tcg --enable-docs --disable-tcg-interpreter --enable-attr --disable-brlapi --disable-linux-aio --disable-bzip2 --disable-bluez --disable-cap-ng --disable-curl --disable-fdt --disable-glusterfs --disable-gnutls --disable-nettle --disable-gtk --disable-rdma --disable-libiscsi --disable-vnc-jpeg --disable-kvm --disable-lzo --disable-curses --disable-libnfs --disable-numa --disable-opengl --disable-vnc-png --disable-rbd --disable-vnc-sasl --disable-sdl --disable-seccomp --disable-smartcard --disable-snappy --disable-spice --disable-libssh2 --disable-libusb --disable-usb-redir --disable-vde --disable-vhost-net --disable-virglrenderer --disable-virtfs --disable-vnc --disable-vte --disable-xen --disable-xen-pci-passthrough --disable-xfsctl --enable-linux-user --disable-system --disable-blobs --disable-tools --static --disable-pie --prefix=~/bin/qemu-user-static`

In the bin folder of your home dir inside the qemu-user-static directory there will be 2 executables one for aarch64 and one for arm (aarch32)
