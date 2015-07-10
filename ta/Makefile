CROSS_COMPILE := $(CROSS_COMPILE_TA)
BINARY = 614789f2-39c0-4ebf-b23592b32ac107ed
DEBUG = 0
include $(TA_DEV_KIT_DIR)/mk/ta_dev_kit.mk

.PHONY: all
all: $(O)/$(BINARY).ta

$(O)/$(BINARY).ta: $(O)/$(BINARY).bin
	@$(cmd-echo-silent) '  GEN    $@'
	@rm -f $@
	@cat faked_armv7_uta_signed_header.bin $< > $@

