ARCHS = armv7 armv7s arm64 arm64e

include $(THEOS)/makefiles/common.mk

BUNDLE_NAME = NoAnnoyancePrefs
NoAnnoyancePrefs_FILES = NoAnnoyancePrefs.mm NoAnnoyanceSettings.mm NoAnnoyanceHeader.mm
NoAnnoyancePrefs_INSTALL_PATH = /Library/PreferenceBundles
NoAnnoyancePrefs_FRAMEWORKS = UIKit
NoAnnoyancePrefs_PRIVATE_FRAMEWORKS = Preferences

include $(THEOS_MAKE_PATH)/bundle.mk

internal-stage::
	$(ECHO_NOTHING)mkdir -p $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences/NoAnnoyance$(ECHO_END)
	$(ECHO_NOTHING)cp entry.plist $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences/NoAnnoyance/NoAnnoyance.plist$(ECHO_END)
