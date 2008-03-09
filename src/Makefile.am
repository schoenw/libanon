#
# src/Makefile.am --
#
# Copyright (c) 2008 Juergen Schoenwaelder, Jacobs University Bremen.
#
# See the file "COPYING" for information on usage and redistribution
# of this file, and for a DISCLAIMER OF ALL WARRANTIES.
#
# @(#) $Id: Makefile.am 1921 2006-05-08 15:14:36Z schoenw $
#

INCLUDES                = $(OPENSSL_CFLAGS)

bin_PROGRAMS		= anon
anon_SOURCES		= anon.c anon.1 \
			  xmalloc.c system.h \
			  getopt.c getopt1.c getopt.h
anon_LDADD		= libanon.la $(OPENSSL_LIBS) -lpcap

include_HEADERS         = libanon.h
lib_LTLIBRARIES         = libanon.la
libanon_la_SOURCES      = anon-ip.c anon-ipv6.c anon-mac.c anon-int64.c \
			  anon-uint64.c anon-octs.c anon-key.c
libanon_la_LDFLAGS      = -version-info @VERSION_LIBTOOL@ $(OPENSSL_LIBS)

man_MANS		= anon.1 anon-ip.3 anon-mac.3

EXTRA_DIST		= $(man_MANS)
