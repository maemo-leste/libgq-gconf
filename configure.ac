AC_INIT([libgq],
        [0.3],
        [merlijn@wizzup.org],
        [libgq])

AM_INIT_AUTOMAKE
AC_CONFIG_FILES([Makefile
                 gconf/Makefile
                 gconf/gq-gconf.pc])


AC_PROG_CC
AC_PROG_INSTALL
AC_PROG_CXX
AC_PROG_LIBTOOL

PKG_CHECK_MODULES([QT],    [Qt5Core])
PKG_CHECK_MODULES([QTEST], [Qt5Test])
PKG_CHECK_MODULES([GLIB],  [glib-2.0])
PKG_CHECK_MODULES([GCONF], [gconf-2.0])

MOC=`pkg-config Qt5Core --variable=moc_location`
RCC=`pkg-config Qt5Core --variable=exec_prefix`/bin/rcc

AC_SUBST([MOC])
AC_SUBST([RCC])

AC_OUTPUT
