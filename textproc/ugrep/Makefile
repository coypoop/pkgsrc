# $NetBSD: Makefile,v 1.5 2020/09/12 15:17:04 wiz Exp $

DISTNAME=	ugrep-2.5.5
CATEGORIES=	textproc
MASTER_SITES=	${MASTER_SITE_GITHUB:=Genivia/}
GITHUB_TAG=	v${PKGVERSION_NOREV}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://github.com/Genivia/ugrep
COMMENT=	Fast grep with many enhancements including Unicode support
LICENSE=	modified-bsd

.include "options.mk"

GNU_CONFIGURE=		yes
USE_LANGUAGES=		c c++
USE_TOOLS+=		gmake pkg-config

CONFIGURE_ARGS+=	--with-bzlib
CONFIGURE_ARGS+=	--with-lz4
CONFIGURE_ARGS+=	--with-lzma	# lzma & xz files
CONFIGURE_ARGS+=	--with-zlib

.include "../../archivers/bzip2/buildlink3.mk"
.include "../../archivers/lz4/buildlink3.mk"
.include "../../archivers/xz/buildlink3.mk"
.include "../../devel/zlib/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
