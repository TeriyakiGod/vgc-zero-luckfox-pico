# app/Makefile - Mock app for Luckfox Pico SDK

# Output binary (dummy)
TARGET := dummy_app

# Build directory (align with SDK)
BUILD_DIR ?= $(CURDIR)/../build/app

.PHONY: all clean install

all: $(BUILD_DIR)/$(TARGET)

# Create empty binary (no compilation needed)
$(BUILD_DIR)/$(TARGET):
	@echo "  MOCK    $(TARGET)"
	@mkdir -p $(BUILD_DIR)
	@touch $@

clean:
	@echo "  CLEAN   $(TARGET)"
	@rm -f $(BUILD_DIR)/$(TARGET)

install: $(BUILD_DIR)/$(TARGET)
	@echo "  INSTALL $(TARGET)"
	@mkdir -p $(TARGET_DIR)/usr/bin/
	@cp $(BUILD_DIR)/$(TARGET) $(TARGET_DIR)/usr/bin/