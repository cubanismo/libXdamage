lib_LTLIBRARIES = libXdamage.la

libXdamage_la_SOURCES = \
	xdamageint.h	\
	Xdamage.c

libXdamage_la_LIBADD = $(XDAMAGE_LIBS) $(X_LIBS)
libXdamage_la_CFLAGS = $(XDAMAGE_CFLAGS) $(X_CFLAGS)

INCLUDES = -I$(top_srcdir)/include/X11/extensions

#
# Library version info.  Check the libtool docs for
# instructions on when and how to change this value
#
# bump when the ABI changes
XDAMAGE_CURRENT=1
# bump for non-ABI changes, reset to zero when CURRENT changes
XDAMAGE_REVISION=0
# bump when the ABI changes in backward-compatible fashion
XDAMAGE_AGE=1
libXdamage_la_LDFLAGS = -version-info ${XDAMAGE_CURRENT}:${XDAMAGE_REVISION}:${XDAMAGE_AGE} -no-undefined

libXdamageincludedir = $(includedir)/X11/extensions
libXdamageinclude_HEADERS = $(top_srcdir)/include/X11/extensions/Xdamage.h 
