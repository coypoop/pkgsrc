# $NetBSD: Makefile,v 1.11 2020/08/17 20:17:57 leot Exp $

PKGREVISION= 1
.include "../../x11/qt5-qscintilla/Makefile.common"

PKGNAME=	qt5-${DISTNAME:tl}
COMMENT=	Scintilla C++ editor class for Qt5

BUILD_DIRS=	Qt4Qt5

USE_TOOLS+=	gmake

MAKE_ENV+=	QTPREFIX=${QTDIR}
INSTALL_ENV+=	INSTALL_ROOT=${DESTDIR}

do-configure:
	cd ${WRKSRC}/Qt4Qt5 && ${QTDIR}/bin/qmake -o Makefile qscintilla.pro

.include "../../mk/bsd.pkg.mk"
