NULL=
SUBDIRS = \
	config                      \
	petardfs.test               \
	sampledata expected_output  

EXTRA_DIST = 

noinst_PROGRAMS = \
	ut_simpleread                 

AM_CPPFLAGS =                                           \
	@FUSE_CFLAGS@                                   \
	-I. 						\
	-I$(srcdir) -I$(top_srcdir) -I$(top_srcdir)/src	\
	-I$(top_builddir)				\
        -I$(includedir)                                 \
	@LIBPOPT_CFLAGS@                                \
	@CFLAGS@

ut_simpleread_SOURCES = ut_simpleread.cpp ut_common.hh
ut_simpleread_LDADD   = @LIBPOPT_LIBS@ -lpopt
ut_simpleread_LDFLAGS = $(GLIB_LIBS) @FUSE_LIBS@

