## `ruby:2-alpine3.7`

```console
$ docker pull ruby@sha256:a2e088faadd7e55bc5742119782da144f7d6697c88ae14e3d2cafc73c88a755a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ruby:2-alpine3.7` - linux; amd64

```console
$ docker pull ruby@sha256:04d79fc6a92b49a5c7c4f3dbb000a5ccc64416f52fcb74c920e187758d87adff
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33067109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcbe56f29e107a3b4043ea3cb0417830cb6e699a6908e20474d6bd2c0c0d4d64`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 01 Dec 2017 18:48:48 GMT
ADD file:2b00f26f6004576e2f8faeb3fb0517a14f79ea89a059fe096b54cbecf5da512e in / 
# Fri, 01 Dec 2017 18:48:48 GMT
CMD ["/bin/sh"]
# Sat, 09 Dec 2017 01:44:51 GMT
RUN mkdir -p /usr/local/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 09 Dec 2017 01:52:58 GMT
ENV RUBY_MAJOR=2.4
# Sat, 09 Dec 2017 01:52:58 GMT
ENV RUBY_VERSION=2.4.2
# Sat, 09 Dec 2017 01:52:58 GMT
ENV RUBY_DOWNLOAD_SHA256=748a8980d30141bd1a4124e11745bb105b436fb1890826e0d2b9ea31af27f735
# Sat, 09 Dec 2017 01:52:59 GMT
ENV RUBYGEMS_VERSION=2.7.3
# Sat, 09 Dec 2017 01:52:59 GMT
ENV BUNDLER_VERSION=1.16.0
# Sat, 09 Dec 2017 01:56:13 GMT
RUN set -ex 		&& apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libressl 		libressl-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 		&& wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz" 	&& echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum -c - 		&& mkdir -p /usr/src/ruby 	&& tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1 	&& rm ruby.tar.xz 		&& cd /usr/src/ruby 		&& { 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new 	&& mv file.c.new file.c 		&& autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& export ac_cv_func_isnan=yes ac_cv_func_isinf=yes 	&& ./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	&& make -j "$(nproc)" 	&& make install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --virtual .ruby-rundeps $runDeps 		bzip2 		ca-certificates 		libffi-dev 		libressl-dev 		procps 		yaml-dev 		zlib-dev 	&& apk del .ruby-builddeps 	&& cd / 	&& rm -r /usr/src/ruby 		&& gem update --system "$RUBYGEMS_VERSION" 	&& gem install bundler --version "$BUNDLER_VERSION" --force
# Sat, 09 Dec 2017 01:56:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 09 Dec 2017 01:56:15 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_BIN=/usr/local/bundle/bin BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 09 Dec 2017 01:56:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2017 01:56:16 GMT
RUN mkdir -p "$GEM_HOME" "$BUNDLE_BIN" 	&& chmod 777 "$GEM_HOME" "$BUNDLE_BIN"
# Sat, 09 Dec 2017 01:56:16 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:2fdfe1cd78c20d05774f0919be19bc1a3e4729bce219968e4188e7e0f1af679d`  
		Last Modified: Fri, 01 Dec 2017 18:50:32 GMT  
		Size: 2.1 MB (2064911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a57127c4cc4bcc3cae1995a44c16104340fe677bef232e0b4c87f727f236a4`  
		Last Modified: Sat, 09 Dec 2017 01:57:02 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62173c354fef2fb9d9fdad42aa0cb21898cb6d5524c72ce1e91fadaaa28f8bf`  
		Last Modified: Sat, 09 Dec 2017 01:58:21 GMT  
		Size: 31.0 MB (31001839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3204663c53876436f4228762cd575f4b4f76dfe78f9b2a6e317d2ee52b899e83`  
		Last Modified: Sat, 09 Dec 2017 01:58:15 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-alpine3.7` - linux; 386

```console
$ docker pull ruby@sha256:d03ee878b3644232eb5c19ca4af9060a70231c9e338c9cbe1091b7f28e741bb9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32145617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf09489282687068aa1c834c077cc3731f9d05962fd8289e24066359312606fc`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 01 Dec 2017 18:46:48 GMT
ADD file:614c07101e677db9a4118a71c852a2be45a337d94c5bedfb48ae8c4cad21d625 in / 
# Fri, 01 Dec 2017 18:46:48 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Fri, 01 Dec 2017 18:46:48 GMT
CMD ["/bin/sh"]
# Sat, 09 Dec 2017 03:40:07 GMT
RUN mkdir -p /usr/local/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 09 Dec 2017 03:47:49 GMT
ENV RUBY_MAJOR=2.4
# Sat, 09 Dec 2017 03:47:49 GMT
ENV RUBY_VERSION=2.4.2
# Sat, 09 Dec 2017 03:47:49 GMT
ENV RUBY_DOWNLOAD_SHA256=748a8980d30141bd1a4124e11745bb105b436fb1890826e0d2b9ea31af27f735
# Sat, 09 Dec 2017 03:47:49 GMT
ENV RUBYGEMS_VERSION=2.7.3
# Sat, 09 Dec 2017 03:47:49 GMT
ENV BUNDLER_VERSION=1.16.0
# Sat, 09 Dec 2017 03:51:57 GMT
RUN set -ex 		&& apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libressl 		libressl-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 		&& wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz" 	&& echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum -c - 		&& mkdir -p /usr/src/ruby 	&& tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1 	&& rm ruby.tar.xz 		&& cd /usr/src/ruby 		&& { 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new 	&& mv file.c.new file.c 		&& autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& export ac_cv_func_isnan=yes ac_cv_func_isinf=yes 	&& ./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	&& make -j "$(nproc)" 	&& make install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --virtual .ruby-rundeps $runDeps 		bzip2 		ca-certificates 		libffi-dev 		libressl-dev 		procps 		yaml-dev 		zlib-dev 	&& apk del .ruby-builddeps 	&& cd / 	&& rm -r /usr/src/ruby 		&& gem update --system "$RUBYGEMS_VERSION" 	&& gem install bundler --version "$BUNDLER_VERSION" --force
# Sat, 09 Dec 2017 03:51:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 09 Dec 2017 03:51:57 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_BIN=/usr/local/bundle/bin BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 09 Dec 2017 03:51:57 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2017 03:51:58 GMT
RUN mkdir -p "$GEM_HOME" "$BUNDLE_BIN" 	&& chmod 777 "$GEM_HOME" "$BUNDLE_BIN"
# Sat, 09 Dec 2017 03:51:58 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:381c1d4107a4401d75b916e6dc4331efddc01adac41f49eeaa711ab898606a1a`  
		Last Modified: Fri, 01 Dec 2017 18:47:24 GMT  
		Size: 2.1 MB (2126217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29cce73050e1b58c218a1c94cd8c9f719d38530500ab97333eac5fdaf385dbc`  
		Last Modified: Fri, 01 Dec 2017 18:47:24 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c00137141498e58cca1612ba60e7c43ceb2c48d52d508547b6aa2ebee17b4e`  
		Last Modified: Sat, 09 Dec 2017 03:56:30 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb242f53acf0ec46f501fabf90b922b5576b5f3c96616b274eaacd20b3db843`  
		Last Modified: Sat, 09 Dec 2017 03:57:53 GMT  
		Size: 30.0 MB (30018868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ebde212ded40be3816122a264e9efbe7a8c62cb8c8b309b6976d1ae2e05050`  
		Last Modified: Sat, 09 Dec 2017 03:57:47 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-alpine3.7` - linux; ppc64le

```console
$ docker pull ruby@sha256:726b3e042c78bd50671a90119e04255c476647a4432053d9feb9196068aab2b6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33110702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f16e4c49f8873294732884a706bfe6bdf3496f578d3ff65f09f4506ec365ba`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 01 Dec 2017 18:41:54 GMT
ADD file:791370adae5cfa8feec749693f5a995a01f58f0462b7aa675fc5bf991e1282b5 in / 
# Fri, 01 Dec 2017 18:41:55 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Fri, 01 Dec 2017 18:41:57 GMT
CMD ["/bin/sh"]
# Sat, 09 Dec 2017 01:16:48 GMT
RUN mkdir -p /usr/local/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 09 Dec 2017 01:20:42 GMT
ENV RUBY_MAJOR=2.4
# Sat, 09 Dec 2017 01:20:43 GMT
ENV RUBY_VERSION=2.4.2
# Sat, 09 Dec 2017 01:20:46 GMT
ENV RUBY_DOWNLOAD_SHA256=748a8980d30141bd1a4124e11745bb105b436fb1890826e0d2b9ea31af27f735
# Sat, 09 Dec 2017 01:20:48 GMT
ENV RUBYGEMS_VERSION=2.7.3
# Sat, 09 Dec 2017 01:20:49 GMT
ENV BUNDLER_VERSION=1.16.0
# Sat, 09 Dec 2017 01:25:28 GMT
RUN set -ex 		&& apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libressl 		libressl-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 		&& wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz" 	&& echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum -c - 		&& mkdir -p /usr/src/ruby 	&& tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1 	&& rm ruby.tar.xz 		&& cd /usr/src/ruby 		&& { 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new 	&& mv file.c.new file.c 		&& autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& export ac_cv_func_isnan=yes ac_cv_func_isinf=yes 	&& ./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	&& make -j "$(nproc)" 	&& make install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --virtual .ruby-rundeps $runDeps 		bzip2 		ca-certificates 		libffi-dev 		libressl-dev 		procps 		yaml-dev 		zlib-dev 	&& apk del .ruby-builddeps 	&& cd / 	&& rm -r /usr/src/ruby 		&& gem update --system "$RUBYGEMS_VERSION" 	&& gem install bundler --version "$BUNDLER_VERSION" --force
# Sat, 09 Dec 2017 01:25:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 09 Dec 2017 01:25:31 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_BIN=/usr/local/bundle/bin BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 09 Dec 2017 01:25:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2017 01:25:35 GMT
RUN mkdir -p "$GEM_HOME" "$BUNDLE_BIN" 	&& chmod 777 "$GEM_HOME" "$BUNDLE_BIN"
# Sat, 09 Dec 2017 01:25:37 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:0da653ea85b50d280ec56ca2eafb7e8b37590630356e043fa9ff162d55732a23`  
		Last Modified: Fri, 01 Dec 2017 18:42:14 GMT  
		Size: 2.1 MB (2081469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd90b777cc38b5b6ca1b2407e647fdc22ef31b57ef98e924e7e0635adffc385`  
		Last Modified: Fri, 01 Dec 2017 18:42:15 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f420090043a7126cb62ce2b71c078a254e7b675bc53fa77b918c77ca5da65b`  
		Last Modified: Sat, 09 Dec 2017 01:26:42 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af590814c16deb06ecadba6b4bf44f2e0d57bd445f37f8e8ba83fe3829e5b7c4`  
		Last Modified: Sat, 09 Dec 2017 01:27:35 GMT  
		Size: 31.0 MB (31028640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4e3cd774157929606d0fcfdbda191352987a05bda24475314178c8bbf1c978`  
		Last Modified: Sat, 09 Dec 2017 01:27:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-alpine3.7` - linux; s390x

```console
$ docker pull ruby@sha256:264f862ad23e10de5ee379fa06dcd25c2d4cf89ea5d6ac48132ad82e859ccb7d
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34930012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30810ceb9063eeff504aabae806682c0215b4dae44fc45d4254cf958b26eab71`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 01 Dec 2017 18:41:57 GMT
ADD file:9c09dfc247c393ab1c6205a4b7857047a3d88e398e8d35aede30f7d613ef1de9 in / 
# Fri, 01 Dec 2017 18:41:58 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Fri, 01 Dec 2017 18:41:58 GMT
CMD ["/bin/sh"]
# Sat, 09 Dec 2017 09:30:02 GMT
RUN mkdir -p /usr/local/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 09 Dec 2017 09:33:16 GMT
ENV RUBY_MAJOR=2.4
# Sat, 09 Dec 2017 09:33:16 GMT
ENV RUBY_VERSION=2.4.2
# Sat, 09 Dec 2017 09:33:16 GMT
ENV RUBY_DOWNLOAD_SHA256=748a8980d30141bd1a4124e11745bb105b436fb1890826e0d2b9ea31af27f735
# Sat, 09 Dec 2017 09:33:16 GMT
ENV RUBYGEMS_VERSION=2.7.3
# Sat, 09 Dec 2017 09:33:17 GMT
ENV BUNDLER_VERSION=1.16.0
# Sat, 09 Dec 2017 09:36:42 GMT
RUN set -ex 		&& apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libressl 		libressl-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 		&& wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz" 	&& echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum -c - 		&& mkdir -p /usr/src/ruby 	&& tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1 	&& rm ruby.tar.xz 		&& cd /usr/src/ruby 		&& { 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new 	&& mv file.c.new file.c 		&& autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& export ac_cv_func_isnan=yes ac_cv_func_isinf=yes 	&& ./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	&& make -j "$(nproc)" 	&& make install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --virtual .ruby-rundeps $runDeps 		bzip2 		ca-certificates 		libffi-dev 		libressl-dev 		procps 		yaml-dev 		zlib-dev 	&& apk del .ruby-builddeps 	&& cd / 	&& rm -r /usr/src/ruby 		&& gem update --system "$RUBYGEMS_VERSION" 	&& gem install bundler --version "$BUNDLER_VERSION" --force
# Sat, 09 Dec 2017 09:36:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 09 Dec 2017 09:36:43 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_BIN=/usr/local/bundle/bin BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 09 Dec 2017 09:36:43 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2017 09:36:44 GMT
RUN mkdir -p "$GEM_HOME" "$BUNDLE_BIN" 	&& chmod 777 "$GEM_HOME" "$BUNDLE_BIN"
# Sat, 09 Dec 2017 09:36:45 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:11e7bc85614a236b32043d147930fd2bc9055af8642fe30e5e56142590572b0e`  
		Last Modified: Fri, 01 Dec 2017 18:42:22 GMT  
		Size: 2.2 MB (2185231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f825cbb729285f1fe2a0cd1d4d36897e3fe2191c5ee044ce11a5d301dc64a34`  
		Last Modified: Fri, 01 Dec 2017 18:42:22 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b39d01f8122b6523ea65219c65c70ce7cf6204f750b3c46cc706bd00081c40`  
		Last Modified: Sat, 09 Dec 2017 09:37:34 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e5da7f4fdbcd7b2803dbf96d0f86fc1fc8525c1696f88fba82fc41d93413c1`  
		Last Modified: Sat, 09 Dec 2017 09:38:21 GMT  
		Size: 32.7 MB (32744249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b78fcc60232effe1ec7d6d6dfbc5c7a7f0fb48c163fbc9fd270b8d37b47799`  
		Last Modified: Sat, 09 Dec 2017 09:38:15 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip