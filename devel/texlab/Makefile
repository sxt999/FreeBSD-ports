PORTNAME=	texlab
DISTVERSIONPREFIX=	v
DISTVERSION=	4.1.0
CATEGORIES=	devel

MAINTAINER=	kfv@kfv.io
COMMENT=	Language Server Protocol for LaTeX

LICENSE=	GPLv3
LICENSE_FILE=	${WRKSRC}/LICENSE

USES=		cargo
USE_GITHUB=	yes
GH_ACCOUNT=	latex-lsp

CARGO_CRATES=	adler-1.0.2 \
		aho-corasick-0.7.18 \
		ansi_term-0.12.1 \
		anyhow-1.0.57 \
		assert_unordered-0.3.5 \
		atty-0.2.14 \
		autocfg-1.1.0 \
		beef-0.5.1 \
		bitflags-1.3.2 \
		block-buffer-0.7.3 \
		block-padding-0.1.5 \
		bstr-0.2.17 \
		bumpalo-3.9.1 \
		byte-tools-0.3.1 \
		byteorder-1.4.3 \
		cast-0.2.7 \
		cfg-if-1.0.0 \
		chrono-0.4.19 \
		clap-2.34.0 \
		clap-3.1.18 \
		clap_derive-3.1.18 \
		clap_lex-0.2.0 \
		console-0.15.0 \
		convert_case-0.4.0 \
		countme-3.0.1 \
		crc32fast-1.3.2 \
		criterion-0.3.5 \
		criterion-plot-0.4.4 \
		crossbeam-channel-0.5.4 \
		crossbeam-deque-0.8.1 \
		crossbeam-epoch-0.9.8 \
		crossbeam-utils-0.8.8 \
		csv-1.1.6 \
		csv-core-0.1.10 \
		dashmap-5.2.0 \
		derive_more-0.99.17 \
		digest-0.8.1 \
		either-1.6.1 \
		encode_unicode-0.3.6 \
		encoding_rs-0.8.31 \
		encoding_rs_io-0.1.7 \
		fake-simd-0.1.2 \
		fastrand-1.7.0 \
		fern-0.6.1 \
		fixedbitset-0.4.1 \
		flate2-1.0.24 \
		fnv-1.0.7 \
		form_urlencoded-1.0.1 \
		fuzzy-matcher-0.3.7 \
		generic-array-0.12.4 \
		getrandom-0.2.6 \
		half-1.8.2 \
		hashbrown-0.11.2 \
		hashbrown-0.12.1 \
		heck-0.4.0 \
		hermit-abi-0.1.19 \
		human_name-1.0.3 \
		idna-0.2.3 \
		indexmap-1.7.0 \
		insta-1.14.1 \
		instant-0.1.12 \
		isocountry-0.3.2 \
		itertools-0.10.3 \
		itoa-0.4.8 \
		itoa-1.0.2 \
		jod-thread-0.1.2 \
		js-sys-0.3.57 \
		lazy_static-1.4.0 \
		libc-0.2.126 \
		linked-hash-map-0.5.4 \
		lock_api-0.4.7 \
		log-0.4.17 \
		logos-0.12.1 \
		logos-derive-0.12.1 \
		lsp-server-0.6.0 \
		lsp-types-0.93.0 \
		maplit-1.0.2 \
		matches-0.1.9 \
		memchr-2.5.0 \
		memoffset-0.6.5 \
		miniz_oxide-0.5.1 \
		multimap-0.8.3 \
		num-integer-0.1.45 \
		num-traits-0.2.15 \
		num_cpus-1.13.1 \
		once_cell-1.12.0 \
		oorandom-11.1.3 \
		opaque-debug-0.2.3 \
		os_str_bytes-6.0.1 \
		parking_lot-0.12.0 \
		parking_lot_core-0.9.3 \
		percent-encoding-2.1.0 \
		pest-2.1.3 \
		pest_derive-2.1.0 \
		pest_generator-2.1.3 \
		pest_meta-2.1.3 \
		petgraph-0.6.2 \
		phf-0.10.1 \
		phf_generator-0.10.0 \
		phf_macros-0.10.0 \
		phf_shared-0.10.0 \
		plotters-0.3.1 \
		plotters-backend-0.3.2 \
		plotters-svg-0.3.1 \
		ppv-lite86-0.2.16 \
		proc-macro-error-1.0.4 \
		proc-macro-error-attr-1.0.4 \
		proc-macro-hack-0.5.19 \
		proc-macro2-1.0.39 \
		quote-1.0.18 \
		rand-0.8.5 \
		rand_chacha-0.3.1 \
		rand_core-0.6.3 \
		rayon-1.5.3 \
		rayon-core-1.9.3 \
		redox_syscall-0.2.13 \
		regex-1.5.6 \
		regex-automata-0.1.10 \
		regex-syntax-0.6.26 \
		remove_dir_all-0.5.3 \
		rowan-0.15.5 \
		rustc-hash-1.1.0 \
		rustc_version-0.4.0 \
		rustversion-1.0.6 \
		ryu-1.0.10 \
		same-file-1.0.6 \
		scopeguard-1.1.0 \
		semver-1.0.9 \
		serde-1.0.137 \
		serde_cbor-0.11.2 \
		serde_derive-1.0.137 \
		serde_json-1.0.81 \
		serde_repr-0.1.8 \
		serde_yaml-0.8.24 \
		sha-1-0.8.2 \
		similar-2.1.0 \
		siphasher-0.3.10 \
		smallstr-0.2.0 \
		smallvec-1.8.0 \
		smol_str-0.1.23 \
		strum-0.24.0 \
		strum_macros-0.24.0 \
		syn-1.0.95 \
		tempfile-3.3.0 \
		terminal_size-0.1.17 \
		text-size-1.1.0 \
		textwrap-0.11.0 \
		textwrap-0.15.0 \
		thiserror-1.0.31 \
		thiserror-impl-1.0.31 \
		thread_local-1.1.4 \
		threadpool-1.8.1 \
		tinytemplate-1.2.1 \
		tinyvec-1.6.0 \
		tinyvec_macros-0.1.0 \
		titlecase-1.1.0 \
		typenum-1.15.0 \
		ucd-trie-0.1.3 \
		unicode-bidi-0.3.8 \
		unicode-ident-1.0.0 \
		unicode-normalization-0.1.19 \
		unicode-segmentation-1.9.0 \
		unicode-width-0.1.9 \
		unidecode-0.3.0 \
		url-2.2.2 \
		uuid-1.1.2 \
		version_check-0.9.4 \
		walkdir-2.3.2 \
		wasi-0.10.2+wasi-snapshot-preview1 \
		wasm-bindgen-0.2.80 \
		wasm-bindgen-backend-0.2.80 \
		wasm-bindgen-macro-0.2.80 \
		wasm-bindgen-macro-support-0.2.80 \
		wasm-bindgen-shared-0.2.80 \
		web-sys-0.3.57 \
		winapi-0.3.9 \
		winapi-i686-pc-windows-gnu-0.4.0 \
		winapi-util-0.1.5 \
		winapi-x86_64-pc-windows-gnu-0.4.0 \
		windows-sys-0.36.1 \
		windows_aarch64_msvc-0.36.1 \
		windows_i686_gnu-0.36.1 \
		windows_i686_msvc-0.36.1 \
		windows_x86_64_gnu-0.36.1 \
		windows_x86_64_msvc-0.36.1 \
		yaml-rust-0.4.5

PLIST_FILES=	bin/${PORTNAME} \
		man/man1/${PORTNAME}.1.gz
PORTDOCS=	CHANGELOG.md README.md docs/*

OPTIONS_DEFINE=		DOCS
OPTIONS_DEFAULT=	DOCS

post-install:
	${STRIP_CMD} ${STAGEDIR}${PREFIX}/bin/${PORTNAME}
	${INSTALL_MAN} ${WRKSRC}/${PORTNAME}.1 \
		${STAGEDIR}${MAN1PREFIX}/man/man1

post-install-DOCS-on:
	${MKDIR} ${STAGEDIR}${DOCSDIR}
	${INSTALL_DATA} ${WRKSRC}/README.md ${STAGEDIR}${DOCSDIR}
	${INSTALL_DATA} ${WRKSRC}/CHANGELOG.md ${STAGEDIR}${DOCSDIR}
	(cd ${WRKSRC} && ${COPYTREE_SHARE} docs ${STAGEDIR}${DOCSDIR})

.include <bsd.port.mk>
