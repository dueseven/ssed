## Process this file with automake to produce Makefile.in
noinst_LIBRARIES = libsed.a
noinst_HEADERS = getopt.h utils.h obstack.h strverscmp.h \
	stdbool_.h

libsed_a_SOURCES = getopt1.c getopt.c utils.c
EXTRA_DIST = memmove.c strerror.c

AM_CPPFLAGS = -I$(top_srcdir)/lib -I$(top_srcdir)/intl -I$(top_srcdir)/pcre \
	-I$(top_srcdir)	-I$(top_builddir)/lib -I$(top_builddir)/intl

libsed_a_LIBADD = @LIBOBJS@ @ALLOCA@
libsed_a_DEPENDENCIES = $(libsed_a_LIBADD)

DISTCLEANFILES = stdbool.h
