# $NetBSD: Makefile,v 1.48 2020/09/14 20:08:27 adam Exp $

DISTNAME=	qtlocation-everywhere-src-${QTVERSION}
PKGNAME=	qt5-qtlocation-${QTVERSION}
COMMENT=	Qt5 module for qtlocation

BUILD_TARGET=		sub-src
MAKE_ENV+=		QTDIR=${QTDIR}
INSTALL_ENV+=		INSTALL_ROOT=${DESTDIR}
INSTALLATION_DIRS+=	lib/pkgconfig

.include "../../x11/qt5-qtbase/Makefile.common"

post-install:
.for i in Qt5Location.pc Qt5Positioning.pc
	cd ${DESTDIR}${PREFIX}/lib/pkgconfig && \
	${LN} -f -s ${QTPREFIX}/lib/pkgconfig/${i} ${i}
.endfor

.include "../../x11/qt5-qtdeclarative/buildlink3.mk"
.include "../../x11/qt5-qtserialport/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
