# $NetBSD: Makefile,v 1.3 2020/05/16 17:13:41 adam Exp $

DISTNAME=	flake8-polyfill-1.0.2
PKGNAME=	${PYPKGPREFIX}-${DISTNAME}
CATEGORIES=	devel python
MASTER_SITES=	${MASTER_SITE_PYPI:=f/flake8-polyfill/}

MAINTAINER=	kamelderouiche@yahoo.com
HOMEPAGE=	https://gitlab.com/pycqa/flake8
COMMENT=	Polyfill package for Flake8 plugins
LICENSE=	mit

DEPENDS+=	${PYPKGPREFIX}-flake8-[0-9]*:../../devel/py-flake8
TEST_DEPENDS+=	${PYPKGPREFIX}-pep8-[0-9]*:../../devel/py-pep8

PYTHON_VERSIONED_DEPENDENCIES=	test:test

USE_LANGUAGES=	# none

# needs to be installed
do-test:
	cd ${WRKSRC} && pytest-${PYVERSSUFFIX}

.include "../../lang/python/egg.mk"
.include "../../lang/python/versioned_dependencies.mk"
.include "../../mk/bsd.pkg.mk"
