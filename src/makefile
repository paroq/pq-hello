include $(PQ_FACTORY)/rules.mk

hello_sources := \
	hello.c

binaries := hello

CFLAGS +=
LDFLAGS += 
CPPFLAGS += 

hello: $(hello_sources)
	gcc $(CFLAGS) $(CPPFLAGS) -o $@ $^ $(LDFLAGS)

build-stamp: $(binaries)
	echo "building hello..."
	touch $@

clean-stamp:
	echo "cleaning hello..."
	rm -f *-stamp
	rm -f $(binaries)
