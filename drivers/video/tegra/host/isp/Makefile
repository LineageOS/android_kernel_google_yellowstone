GCOV_PROFILE := y
ccflags-y += -Idrivers/video/tegra/host
ccflags-y += -Idrivers/video/tegra/camera
ccflags-y += -Werror

ifeq ($(CONFIG_ARCH_TEGRA_18x_SOC),y)
ccflags-y += -I../kernel-t18x/drivers/video/tegra/host/
endif

nvhost-isp-objs  = \
		isp_isr_v1.o \
		isp.o

obj-$(CONFIG_TEGRA_GRHOST_ISP) += nvhost-isp.o
