
FILECMD:=file

MAGICDIRS:=../misc_magic ../com_magic ../exe_magic
MAGICFILES:=$(wildcard ../misc_magic/*.magic ../com_magic/*.magic ../exe_magic/*.magic)

mfcm.mgc: $(MAGICDIRS) $(MAGICFILES)
	rm -rf mfcm
	mkdir -p mfcm
	cp $(MAGICFILES) mfcm/
	$(FILECMD) -C -m mfcm
	rm -rf mfcm

.PHONY: clean
clean:
	rm -f mfcm.mgc
