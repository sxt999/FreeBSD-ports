PORTNAME=	elasticsearch-model
PORTVERSION=	7.2.1
CATEGORIES=	textproc rubygems
MASTER_SITES=	RG
PKGNAMESUFFIX=	713

MAINTAINER=	mfechner@FreeBSD.org
COMMENT=	ActiveModel/Record integrations for Elasticsearch

LICENSE=	APACHE20
LICENSE_FILE=	${WRKSRC}/LICENSE.txt

RUN_DEPENDS=	rubygem-activesupport61>=3:devel/rubygem-activesupport61 \
		rubygem-elasticsearch713>=7<8:textproc/rubygem-elasticsearch713 \
		rubygem-hashie>=0:devel/rubygem-hashie

USES=		gem
USE_RUBY=	yes

NO_ARCH=	yes

.include <bsd.port.mk>
