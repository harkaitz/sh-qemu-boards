.POSIX:
.SUFFIXES:
.PHONY: all clean install check
all:
PROJECT   =qemu-boards
VERSION   =1.0.0
PREFIX    =/usr/local
BUILDDIR ?=.build

all:
clean:
install:
check:
## -- BLOCK:license --
install: install-license
install-license: README.md COPYING COPYRIGHT
	mkdir -p $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
	cp README.md COPYING COPYRIGHT $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
## -- BLOCK:license --
## -- BLOCK:sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/iso-raspberry $(DESTDIR)$(PREFIX)/bin
	cp bin/qemu-h-rpi3 $(DESTDIR)$(PREFIX)/bin
	cp bin/lomount $(DESTDIR)$(PREFIX)/bin
## -- BLOCK:sh --
