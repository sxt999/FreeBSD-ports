PORTNAME=	cassandra
DISTVERSION=	1.3.2.a.20200527
PORTEPOCH=	1
CATEGORIES=	databases
PKGNAMEPREFIX=	${PHP_PKGNAMEPREFIX}

MAINTAINER=	daniel@blodan.se
COMMENT=	Extension to access Cassandra

LICENSE=	APACHE20
LICENSE_FILE=	${WRKSRC}/LICENSE

DEPRECATED=	Requires php 7.4 which is set to expire on 2022-11-29
EXPIRATION_DATE=2022-11-28

LIB_DEPENDS=	libcassandra.so:databases/cassandra-cpp-driver \
		libgmp.so:math/gmp \
		libuv.so:devel/libuv

USES=		localbase php:ext

USE_GITHUB=	yes
GH_ACCOUNT=	datastax
GH_PROJECT=	php-driver
GH_TAGNAME=	61faee0

IGNORE_WITH_PHP=	80 81 82
PHP_MODNAME=	cassandra

WRKSRC_SUBDIR=	ext

.include <bsd.port.mk>
