#
# Makefile for sensor chip drivers.
#

obj-$(CONFIG_THERMAL)		+= thermal_sys.o
obj-$(CONFIG_THERMAL_MSM_POPMEM)	+= msm_popmem-tm.o
obj-$(CONFIG_THERMAL_TSENS)	+= msm_tsens.o
obj-$(CONFIG_THERMAL_TSENS8960) += msm8960_tsens.o
obj-$(CONFIG_THERMAL_PM8XXX)	+= pm8xxx-tm.o
ifdef CONFIG_INTELLI_THERMAL
obj-$(CONFIG_INTELLI_THERMAL)	+= intelli/
else
ifdef CONFIG_INTELLI_THERMAL_V2
obj-$(CONFIG_INTELLI_THERMAL_V2)+= intelli/
else
obj-$(CONFIG_THERMAL_MONITOR)	+= msm_thermal.o msm_thermal-dev.o
endif
endif
obj-$(CONFIG_SPEAR_THERMAL)		+= spear_thermal.o
obj-$(CONFIG_THERMAL_TSENS8974)	+= msm8974-tsens.o
obj-$(CONFIG_THERMAL_QPNP)	+= qpnp-temp-alarm.o
obj-$(CONFIG_THERMAL_QPNP_ADC_TM)	+= qpnp-adc-tm.o
obj-$(CONFIG_THERMAL_DELTA)	+= htc_thermal.o

KBUILD_CFLAGS	+=-Wno-unused-const-variable
KBUILD_CFLAGS	+=-Wno-strict-aliasing
