# $NetBSD: Makefile,v 1.5 2020/09/03 07:29:40 bsiegert Exp $

DISTNAME=	go-cmp-0.4.0
MASTER_SITES=	${MASTER_SITE_GITHUB:=google/}
PKGREVISION=	4
CATEGORIES=	devel
GITHUB_PROJECT=	go-cmp
GITHUB_TAG=	v${PKGVERSION_NOREV}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://github.com/google/go-cmp
COMMENT=	Package for comparing Go values in tests
LICENSE=	modified-bsd

GO_DIST_BASE=	${DISTNAME}
GO_SRCPATH=	github.com/google/go-cmp

.include "../../devel/go-xerrors/buildlink3.mk"
.include "../../lang/go/go-package.mk"
.include "../../mk/bsd.pkg.mk"
