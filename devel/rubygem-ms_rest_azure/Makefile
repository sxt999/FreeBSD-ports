# Created by: Po-Chuan Hsieh <sunpoet@FreeBSD.org>

PORTNAME=	ms_rest_azure
PORTVERSION=	0.12.0
PORTREVISION=	1
CATEGORIES=	devel rubygems
MASTER_SITES=	RG

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Azure Client Library for Ruby

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE.txt

RUN_DEPENDS=	rubygem-concurrent-ruby>=1.0<2:devel/rubygem-concurrent-ruby \
		rubygem-faraday1>=0.9<2.0.0:www/rubygem-faraday1 \
		rubygem-faraday-cookie_jar>=0.0.6<0.1:devel/rubygem-faraday-cookie_jar \
		rubygem-ms_rest>=0.7.6<0.8:devel/rubygem-ms_rest

USES=		gem
USE_RUBY=	yes

NO_ARCH=	yes

.include <bsd.port.mk>
