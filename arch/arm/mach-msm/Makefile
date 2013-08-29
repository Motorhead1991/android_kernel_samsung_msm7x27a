obj-y += io.o dma.o memory.o timer.o
obj-y += clock.o clock-voter.o clock-dummy.o
obj-y += modem_notifier.o subsystem_map.o
obj-$(CONFIG_CPU_FREQ_MSM) += cpufreq.o
ifndef CONFIG_ARCH_MSM8X60
obj-y += acpuclock-arm11.o
endif

ifdef CONFIG_MSM_VIC
obj-y += irq-vic.o
else
ifndef CONFIG_ARCH_MSM8X60
obj-y += irq.o
endif
endif

obj-$(CONFIG_ARCH_MSM8X60) += clock-dummy.o iommu.o iommu_dev.o devices-msm8x60-iommu.o
obj-$(CONFIG_MSM_PROC_COMM) += proc_comm.o clock-pcom.o vreg.o
obj-$(CONFIG_MSM_PROC_COMM) += clock.o 
obj-$(CONFIG_MSM_SMD) += smd.o smd_debug.o
obj-$(CONFIG_MSM_SMD) += last_radio_log.o
obj-$(CONFIG_MSM_SCM) += scm.o scm-boot.o
obj-$(CONFIG_HOTPLUG_CPU) += hotplug.o
obj-$(CONFIG_SMP) += headsmp.o platsmp.o

# Arch calls
obj-$(CONFIG_ARCH_MSM_ARM11) += acpuclock-7201.o
obj-$(CONFIG_ARCH_MSM_SCORPION) += pmu.o
obj-$(CONFIG_ARCH_MSM_CORTEX_A5) += acpuclock-7201.o
obj-$(CONFIG_ARCH_MSM_KRAIT) += msm-krait-l2-accessors.o pmu.o
obj-$(CONFIG_ARCH_MSM7X27) += gpiomux-7x27.o gpiomux-v1.o gpiomux.o
obj-$(CONFIG_ARCH_MSM7X30) += board-msm7x30.o devices-msm7x30.o
obj-$(CONFIG_ARCH_QSD8X50) += board-qsd8x50.o devices-qsd8x50.o
obj-$(CONFIG_ARCH_MSM8X60) += board-msm8x60.o
obj-$(CONFIG_ARCH_MSM7X30) += gpiomux-7x30.o gpiomux-v1.o gpiomux.o
obj-$(CONFIG_ARCH_QSD8X50) += gpiomux-8x50.o gpiomux-v1.o gpiomux.o
obj-$(CONFIG_ARCH_MSM8X60) += gpiomux-8x60.o gpiomux-v2.o gpiomux.o

# Board calls
obj-$(CONFIG_MACH_MSM7X25_SURF) += board-msm7x27.o devices-msm7x25.o
obj-$(CONFIG_MACH_MSM7X25_FFA) += board-msm7x27.o devices-msm7x25.o
obj-$(CONFIG_ARCH_QSD8X50) += sirc.o
obj-$(CONFIG_ARCH_MSM7X27A) += dal_axi.o msm_vibrator.o clock-pcom-lookup.o
obj-$(CONFIG_MACH_HALIBUT) += board-halibut.o devices-msm7x00.o
obj-$(CONFIG_MACH_TROUT) += board-trout.o board-trout-gpio.o board-trout-mmc.o devices-msm7x00.o board-trout-panel.o
obj-$(CONFIG_MACH_MSM7X27A_RUMI3) += board-msm7x27a.o devices-msm7x27a.o
obj-$(CONFIG_MACH_MSM7X27A_SURF) += board-msm7x27a.o devices-msm7x27a.o
obj-$(CONFIG_MACH_MSM7X27A_FFA) += devices-msm7x27a.o

ifdef CONFIG_MSM_V2_TLMM
obj-y	+= gpio-v2.o
else
obj-y	+= gpio.o
endif
obj-$(CONFIG_MSM_PROC_COMM_REGULATOR) += proccomm-regulator.o
