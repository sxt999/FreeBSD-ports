# Created by: Horance Chou <horance@freedom.ie.cycu.edu.tw>

PORTNAME=	libffi
PORTVERSION=	3.4.2
CATEGORIES=	devel
MASTER_SITES=	https://github.com/${PORTNAME}/${PORTNAME}/releases/download/v${PORTVERSION}/

MAINTAINER=	kbowling@FreeBSD.org
COMMENT=	Foreign Function Interface

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

TEST_DEPENDS=	runtest:misc/dejagnu

USES=		compiler:c11 cpe libtool pathfix
USE_LDCONFIG=	yes
GNU_CONFIGURE=	yes
CPE_VENDOR=	libffi_project

CONFIGURE_ARGS=	--disable-multi-os-directory
INSTALL_TARGET=	install-strip
INFO=		libffi
TEST_TARGET=	check

post-patch:
	@${REINPLACE_CMD} -e 's| -Wno-psabi||g' \
		${WRKSRC}/testsuite/lib/libffi.exp

.include <bsd.port.mk>
