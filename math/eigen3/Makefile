PORTNAME=	eigen
DISTVERSION=	3.4.0
CATEGORIES=	math
MASTER_SITES=	https://gitlab.com/libeigen/eigen/-/archive/${DISTVERSION}/

MAINTAINER=	kde@FreeBSD.org
COMMENT=	Lightweight library for vector and matrix math

LICENSE=	LGPL21 MPL20
LICENSE_COMB=	multi
LICENSE_FILE_LGPL21=	${WRKSRC}/COPYING.LGPL
LICENSE_FILE_MPL20=	${WRKSRC}/COPYING.MPL2

TEST_DEPENDS=	suitesparse-cholmod>0:math/suitesparse-cholmod \
		suitesparse-umfpack>0:math/suitesparse-umfpack \
		superlu>0:math/superlu	\
		adol-c>0:math/adol-c \
		fftw3>0:math/fftw3 \
		mpfr>0:math/mpfr \
		gmp>0:math/gmp \
		boost-libs>0:devel/boost-libs

USES=		cmake:testing tar:bzip2

CMAKE_ARGS=	-DPKGCONFIG_INSTALL_DIR:PATH="libdata/pkgconfig"
CMAKE_ON=	EIGEN_TEST_CXX11 # This is to set the C++ standard to C++11, instead of 03
CMAKE_TESTING_ON=	EIGEN_TEST_CUDA EIGEN_TEST_CUDA_CLANG

NO_BUILD=	yes
NO_ARCH=	yes

OPTIONS_DEFINE=	BLAS
OPTIONS_DEFAULT=BLAS

BLAS_DESC=	Adds math dependencies
BLAS_CMAKE_ON=	-DBLAS_DIR:PATH="${LOCALBASE}"
BLAS_USES=	blaslapack pkgconfig

.include <bsd.port.mk>
