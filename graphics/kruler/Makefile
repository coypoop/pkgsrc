# $NetBSD: Makefile,v 1.50 2020/08/18 17:58:02 leot Exp $

DISTNAME=	kruler-${KAPPSVER}
PKGREVISION=	2
CATEGORIES=	graphics

HOMEPAGE=	https://kde.org/applications/graphics/kruler/
COMMENT=	KDE screen ruler
LICENSE=	gnu-gpl-v2 AND gnu-fdl-v1.2 AND gnu-lgpl-v2

.include "../../meta-pkgs/kde/applications.mk"

BUILD_DEPENDS+=	kdoctools>=5.19.0:../../devel/kdoctools

USE_TOOLS+=	msgmerge pkg-config

.include "../../devel/knotifications/buildlink3.mk"
.include "../../graphics/hicolor-icon-theme/buildlink3.mk"
.include "../../sysutils/desktop-file-utils/desktopdb.mk"
.include "../../x11/kxmlgui/buildlink3.mk"
.include "../../x11/qt5-qtbase/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
