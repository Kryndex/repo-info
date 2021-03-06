## `python:2-alpine3.4`

```console
$ docker pull python@sha256:78cee3882c3e4b5e5e98b4cffb558ba0f7f3a68118724d0fb74c99c67321820a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `python:2-alpine3.4` - linux; amd64

```console
$ docker pull python@sha256:36099dd9ff163cfa07eb84d23d18c0c8db945b6f06e16410cde773c9a821ce67
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26052430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64905abbb69ee7cfda81ac10e7a9082e3d902ddd71ca7c18f895c788e633b14c`
-	Default Command: `["python2"]`

```dockerfile
# Fri, 01 Dec 2017 18:49:44 GMT
ADD file:c05a199f603e2a97ea93d9f6cc210a1c8ab27eda35f3613722bfcf697da36483 in / 
# Fri, 01 Dec 2017 18:49:45 GMT
CMD ["/bin/sh"]
# Mon, 04 Dec 2017 16:40:27 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 04 Dec 2017 16:40:28 GMT
ENV LANG=C.UTF-8
# Mon, 04 Dec 2017 16:40:31 GMT
RUN apk add --no-cache ca-certificates
# Mon, 04 Dec 2017 16:48:48 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Mon, 04 Dec 2017 16:48:48 GMT
ENV PYTHON_VERSION=2.7.14
# Tue, 19 Dec 2017 22:37:06 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		openssl 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bzip2-dev 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		libc-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		zlib-dev 	&& apk del .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 	&& make install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --virtual .python-rundeps $runDeps 	&& apk del .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python
# Tue, 19 Dec 2017 22:37:06 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 19 Dec 2017 22:37:12 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps openssl; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		apk del .fetch-deps; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 19 Dec 2017 22:37:13 GMT
CMD ["python2"]
```

-	Layers:
	-	`sha256:ab7e51e37a183df284512426b1cb56d0404532b6011c823f35127c796fb97b13`  
		Last Modified: Fri, 01 Dec 2017 18:58:11 GMT  
		Size: 2.4 MB (2387532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a57a4e05b897448d0d35879e81d6e7b273d94f14b604425f9a5e9a0341a466a`  
		Last Modified: Mon, 04 Dec 2017 16:51:59 GMT  
		Size: 346.8 KB (346848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765ccb94f933250c5b82b24c7517f196b2bad10b13c6e06763992df0e9ecc963`  
		Last Modified: Tue, 19 Dec 2017 22:39:03 GMT  
		Size: 21.4 MB (21385127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cd29df27e59c6a03029c733dd45735f0508902d27cf19127db4492de160f1e`  
		Last Modified: Tue, 19 Dec 2017 22:38:57 GMT  
		Size: 1.9 MB (1932923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
