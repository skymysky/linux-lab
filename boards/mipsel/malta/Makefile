_BASE    = 1
ARCH     = mips
XARCH    = mipsel
CPU     ?= mips32r2
#LINUX   ?= v4.6.7
LINUX   ?= v5.1
BUILDROOT?= 2016.05
MEM     ?= 128M
NETDEV  ?= pcnet
SERIAL  ?= ttyS0
FSTYPE  ?= ext2
ORIIMG  ?= vmlinuz
ROOTDEV ?= /dev/ram0
CCPRE   ?= mipsel-linux-gnu-
KIMAGE  ?= $(PREBUILT_KERNEL)/$(XARCH)/$(MACH)/$(LINUX)/vmlinuz
ROOTFS  ?= $(PREBUILT_ROOT)/$(XARCH)/$(CPU)/rootfs.cpio.gz
HROOTFS ?= $(PREBUILT_ROOT)/$(XARCH)/$(CPU)/rootfs.$(FSTYPE)
