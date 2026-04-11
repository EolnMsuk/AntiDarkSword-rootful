TARGET := iphone:clang:16.5:14.0
include $(THEOS)/makefiles/common.mk

TWEAK_NAME = AntiDarkSwordDaemon
AntiDarkSwordDaemon_FILES = Tweak.x
AntiDarkSwordDaemon_CFLAGS = -fobjc-arc
AntiDarkSwordDaemon_FRAMEWORKS = Foundation CoreFoundation

include $(THEOS_MAKE_PATH)/tweak.mk
