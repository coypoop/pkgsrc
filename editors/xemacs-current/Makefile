# $NetBSD: Makefile,v 1.106 2020/09/24 17:02:02 hauke Exp $

PKGNAME=	${DISTNAME}
PKGREVISION=	14
COMMENT=	*BETA* XEmacs text editor version ${PKGVERSION_NOREV}

# extra options for x11 support, not for sharing with xemacs-current-nox11
# Version information in ../../editors/xemacs-current/Makefile.common

PKG_SUPPORTED_OPTIONS+=		x11 xft xface
PKG_SUGGESTED_OPTIONS+=		x11

.include "options.mk"

LIBDIR=				${PREFIX}/lib/${DISTNAME}

SUBST_CLASSES+=			desktop-file
SUBST_STAGE.desktop-file=	pre-configure
SUBST_MESSAGE.desktop-file=	Fixing paths in XEmacs desktop file
SUBST_VARS.desktop-file=	PREFIX LIBDIR
SUBST_FILES.desktop-file=	etc/xemacs.desktop

INSTALLATION_DIRS+=		share/applications

.include "Makefile.common"

.include "../../sysutils/desktop-file-utils/desktopdb.mk"
.include "../../mk/bsd.pkg.mk"
