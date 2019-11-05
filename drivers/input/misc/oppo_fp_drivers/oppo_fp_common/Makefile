ifeq ($(CONFIG_OPPO_FINGERPRINT_QCOM),y)
PROJECT_NAME = $(subst MSM_,,$(OPPO_TARGET_DEVICE))
else ifeq ($(CONFIG_OPPO_FINGERPRINT_MTK),y)
PROJECT_NAME = $(shell echo $(TARGET_PRODUCT) | sed -e 's/full_oppo.*_//g')
endif

ccflags-y += -DCONFIG_OPPO_FINGERPRINT_PLATFORM=660

obj-y     +=  oppo_fp_common.o

