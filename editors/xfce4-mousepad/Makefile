# $NetBSD: Makefile,v 1.51 2020/08/31 18:09:26 wiz Exp $

PKGREVISION= 5
.include "../../meta-pkgs/xfce4/Makefile.common"

VERSION=	0.4.2
DISTNAME=	mousepad-${VERSION}
PKGNAME=	xfce4-mousepad-${VERSION}
CATEGORIES=	editors
MASTER_SITES=	http://archive.xfce.org/src/apps/mousepad/0.4/

HOMEPAGE=	http://users.xfce.org/~benny/xfce/apps.html
COMMENT=	Xfce text editor

.include "../../devel/glib2/schemas.mk"
.include "../../devel/xfce4-conf/buildlink3.mk"
.include "../../sysutils/desktop-file-utils/desktopdb.mk"
.include "../../x11/gtksourceview3/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
