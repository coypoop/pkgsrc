# $NetBSD: Makefile,v 1.93 2020/08/17 20:20:21 leot Exp $

PKGNAME=	${DISTNAME:S/links/&-gui/}
PKGREVISION=	5
COMMENT=	Lynx-like text and graphics WWW browser

USE_TOOLS+=		pkg-config
CONFIGURE_ARGS+=	--enable-graphics
CONFIGURE_ARGS+=	--without-sdl

BUILDLINK_DEPMETHOD.libXt?=	build

PKG_SUPPORTED_OPTIONS+=	svg

.include "../../www/links/Makefile.common"

.if !empty(PKG_OPTIONS:Msvg)
.  include "../../graphics/librsvg/buildlink3.mk"
.else
CONFIGURE_ARGS+=	--without-librsvg
.endif

.include "../../fonts/fontconfig/buildlink3.mk"
.include "../../graphics/freetype2/buildlink3.mk"
.include "../../graphics/png/buildlink3.mk"
.include "../../graphics/tiff/buildlink3.mk"
.include "../../x11/libX11/buildlink3.mk"
.include "../../x11/libXt/buildlink3.mk"

.include "../../mk/bsd.pkg.mk"
