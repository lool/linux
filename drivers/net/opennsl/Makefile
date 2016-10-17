#
# Makefile for OpenNSL drivers
#

ccflags-y += \
	-Idrivers/net/opennsl/include \
	-Idrivers/net/opennsl/systems/bde/linux/include \
	-Idrivers/net/opennsl/systems/bde/shared/include \
	-Idrivers/net/opennsl/systems/linux/kernel/modules/include

obj-$(CONFIG_OPENNSL_BCM_KNET) += linux-bcm-knet.o

linux-bcm-knet-objs := \
	systems/linux/kernel/modules/bcm-knet/bcm-knet.o \
	systems/linux/kernel/modules/shared/gmodule.o \

obj-$(CONFIG_OPENNSL_KERNEL_BDE) += linux-kernel-bde.o

linux-kernel-bde-objs := \
	systems/bde/linux/kernel/linux-kernel-bde.o \
	systems/bde/linux/kernel/linux_shbde.o \
	systems/bde/linux/shared/mpool.o \
	systems/bde/shared/shbde_iproc.o \
	systems/bde/shared/shbde_mdio.o \
	systems/bde/shared/shbde_pci.o \

obj-$(CONFIG_OPENNSL_USER_BDE) += linux-user-bde.o

linux-user-bde-objs := \
	systems/bde/linux/user/kernel/linux-user-bde.o \
	systems/linux/kernel/modules/shared/ksal.o \
	systems/linux/kernel/modules/shared/gmodule.o \

