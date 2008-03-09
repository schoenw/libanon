#
# Makefile.am --
#
#      Template to generate the toplevel Makefile.in using automake.
#
# Copyright (c) 2008 Juergen Schoenwaelder, Jacobs University Bremen.
#
# See the file "COPYING" for information on usage and redistribution
# of this file, and for a DISCLAIMER OF ALL WARRANTIES.
#
# @(#) $Id: Makefile.am 1921 2006-05-08 15:14:36Z schoenw $
#

AUTOMAKE_OPTIONS        = no-dependencies foreign

EXTRA_DIST		= libanon.lsm.in libanon.spec.in libanon.pc

SUBDIRS			= src test

pkgconfigdir		= $(libdir)/pkgconfig
pkgconfig_DATA		= libanon.pc
$(pkgconfig_DATA):	config.status
