PORTNAME=	libnpupnp
DISTVERSION=	4.2.3
CATEGORIES=	net
MASTER_SITES=	https://www.lesbonscomptes.com/upmpdcli/downloads/

MAINTAINER=	diizzy@FreeBSD.org
COMMENT=	C++ base UPnP library, derived from Portable UPnP, a.k.a libupnp

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/COPYING

LIB_DEPENDS=	libcurl.so:ftp/curl \
		libexpat.so:textproc/expat2 \
		libmicrohttpd.so:www/libmicrohttpd

USES=		compiler:c++14-lang libtool localbase pkgconfig
GNU_CONFIGURE=	yes
USE_LDCONFIG=	yes

INSTALL_TARGET=	install-strip

.include <bsd.port.mk>
