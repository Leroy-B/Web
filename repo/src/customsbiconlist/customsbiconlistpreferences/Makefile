ARCHS = arm64

include $(THEOS)/makefiles/common.mk

BUNDLE_NAME = CustomSBIconListPreferences
CustomSBIconListPreferences_FILES = CustomSBIconListPreferences.mm
CustomSBIconListPreferences_INSTALL_PATH = /Library/PreferenceBundles
CustomSBIconListPreferences_FRAMEWORKS = UIKit
CustomSBIconListPreferences_PRIVATE_FRAMEWORKS = Preferences

include $(THEOS_MAKE_PATH)/bundle.mk

internal-stage::
	$(ECHO_NOTHING)mkdir -p $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences$(ECHO_END)
	$(ECHO_NOTHING)cp entry.plist $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences/CustomSBIconListPreferences.plist$(ECHO_END)