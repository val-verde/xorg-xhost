# $XdotOrg: $

AC_PREREQ([2.57])
AC_INIT(xhost,[7.0], [xorg@freedestkop.org],xhost)
AM_INIT_AUTOMAKE([dist-bzip2])
AM_MAINTAINER_MODE

AM_CONFIG_HEADER(config.h)

AC_PROG_CC
AC_PROG_INSTALL

AC_TYPE_SIGNAL

# Checks for pkg-config packages
PKG_CHECK_MODULES(XHOST, x11 xmu)
AC_SUBST(XHOST_CFLAGS)
AC_SUBST(XHOST_LIBS)

# Transport selection macro from xtrans.m4
XTRANS_CONNECTION_FLAGS

# Secure RPC detection macro from xtrans.m4
XTRANS_SECURE_RPC_FLAGS

AC_OUTPUT([Makefile])