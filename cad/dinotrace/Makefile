# $NetBSD: Makefile,v 1.52 2020/08/31 18:06:40 wiz Exp $
#

DISTNAME=	dinotrace-9.4c
PKGREVISION=	6
CATEGORIES=	cad
MASTER_SITES=	http://www.veripool.org/ftp/
EXTRACT_SUFX=	.tgz

MAINTAINER=	dmcmahill@NetBSD.org
HOMEPAGE=	http://www.veripool.org/dinotrace/
COMMENT=	Tool for viewing the output of digital simulators

LICENSE=	gnu-gpl-v3

GNU_CONFIGURE=		YES
INFO_FILES=		YES
USE_TOOLS+=		gmake perl

.include "../../mk/motif.buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
