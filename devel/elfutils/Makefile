# Created by: Conrad Meyer <cem@FreeBSD.org>

PORTNAME=	elfutils
DISTVERSION=	0.187
CATEGORIES=	devel
MASTER_SITES=	https://sourceware.org/elfutils/ftp/${PORTVERSION}/

MAINTAINER=	cem@FreeBSD.org
COMMENT=	Library for manipulating ELF files and partial implementation of binutils

LICENSE=	LGPL3 GPLv2+ GPLv3+
LICENSE_COMB=	multi
LICENSE_FILE_GPLv3+ =	${WRKSRC}/COPYING
LICENSE_FILE_GPLv2+ =	${WRKSRC}/COPYING-GPLV2
LICENSE_FILE_LGPL3=	${WRKSRC}/COPYING-LGPLV3

BROKEN_armv6=		fails to build: fails to compile i386_disasm.c
BROKEN_sparc64=		sparc patch does not apply cleanly to 0.172

LIB_DEPENDS=	libargp.so:devel/argp-standalone \
		libcurl.so:ftp/curl
BUILD_DEPENDS=	gnulib>=0:devel/gnulib

PLIST_SUB=	VERSION=${PORTVERSION}

CFLAGS+=	-I${LOCALBASE}/share/gnulib/lib
LDFLAGS+=	${LOCALBASE}/lib/libargp.so \
		${LOCALBASE}/lib/libintl.so

OPTIONS_DEFINE=	MANPAGES NLS
OPTIONS_DEFAULT=	MANPAGES
OPTIONS_SUB=	yes

NLS_USES=	gettext
NLS_USES_OFF=	gettext  # used anyway
NLS_CONFIGURE_ENABLE=	nls

USES=		autoreconf cpe gmake libtool pkgconfig tar:bzip2
CPE_VENDOR=	${PORTNAME}_project
GNU_CONFIGURE=	yes
USE_LDCONFIG=	yes

CFLAGS+=	-Wno-error -Wno-format-nonliteral
CFLAGS+=	-Wno-null-dereference -Wno-unused-value

# Avoid conflict with binutils / elftoolchain programs with the same names:
CONFIGURE_ARGS+=	--program-prefix=eu-
# Disable debuginfod until option support can be added:
CONFIGURE_ARGS+=	--disable-debuginfod

.include <bsd.port.options.mk>

.if ${OPSYS} == FreeBSD && ${OSVERSION} >= 1300512 # 2021-07-17
CFLAGS+=	-DFREEBSD_HAS_MEMPCPY
.endif

pre-configure:
	@${CP} -a \
	    ${LOCALBASE}/share/gnulib/lib/obstack.c \
	    ${LOCALBASE}/share/gnulib/lib/obstack.h \
	    ${LOCALBASE}/share/gnulib/lib/obstack_printf.c \
	    ${WRKSRC}/lib

post-configure: # remove -Werror since it causes build failures
	@${FIND} ${WRKSRC} -name Makefile | ${XARGS} ${REINPLACE_CMD} -e 's| -Werror| |; s|-Werror ||'

.include <bsd.port.mk>
