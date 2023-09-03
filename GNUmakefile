lib.name = hid
hid.class.sources = \
	hid.c \
	input_arrays.c \
	$(empty)

define forLinux
hid.class.sources += \
	hid_linux.c \
	$(empty)
endef
define forDarwin
hid.class.sources += \
	hid_darwin.c \
	$(empty)
endef

datafiles = \
	$(wildcard *.pd) \
	$(wildcard *.txt) \
	$(wildcard *.md) \
	$(empty)

datadirs = \
	examples \
	$(empty)

PDLIBBUILDER_DIR=pd-lib-builder
include $(PDLIBBUILDER_DIR)/Makefile.pdlibbuilder
