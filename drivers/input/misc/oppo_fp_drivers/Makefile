ifeq ($(CONFIG_OPPO_FINGERPRINT),y)
obj-y        += oppo_fp_common/
obj-y        += fpc/
endif
ifneq ($(filter MSM_17011, $(OPPO_TARGET_DEVICE)),)
obj-y        += goodix_fp/
endif