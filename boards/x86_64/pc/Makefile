_BASE    = 1
ARCH     = x86
XARCH    = x86_64
# qemu-system-x86_64 -M pc -cpu ?
CPU     ?= qemu64
MEM     ?= 1024M
QEMU    ?= v0.10.6
SMP     ?= 4
LINUX   ?= v5.1
BUILDROOT?= 2019.02.2

# Check qemu support:
# $ qemu-system-i386 -net nic,model=?
#   qemu: Supported NIC models: ne2k_pci,i82551,i82557b,i82559er,rtl8139,e1000,pcnet,virtio
#
# Kernel enabled: ne2k_pci, e1000, rtl8139, pcnet
NETDEV  ?= ne2k_pci
SERIAL  ?= ttyS0
ORIIMG  ?= arch/$(ARCH)/boot/bzImage

# Verified ROOTDEV: /dev/ram0, /dev/nfs, /dev/hda
ROOTDEV ?= /dev/ram0

KIMAGE  ?= $(PREBUILT_KERNEL)/$(XARCH)/$(MACH)/$(LINUX)/bzImage
ROOTFS  ?= $(PREBUILT_ROOT)/$(XARCH)/$(CPU)/rootfs.cpio.gz
HROOTFS ?= $(PREBUILT_ROOT)/$(XARCH)/$(CPU)/rootfs.ext2
