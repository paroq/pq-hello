include $(PQ_FACTORY)/rules.mk

hello_sources := \
	hello.c

binaries := hello

LDFLAGS += -lhello-lib

hello: $(hello_sources)
	$(call show_vars,CFLAGS CPPFLAGS)
	gcc $(CFLAGS) $(CPPFLAGS) -o $@ $^ $(LDFLAGS)

build-stamp: $(binaries)
	echo "building hello..."
	touch $@

clean-stamp:
	echo "cleaning hello..."
	rm -f *-stamp
	rm -f $(binaries)
