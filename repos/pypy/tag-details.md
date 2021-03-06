<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `pypy`

-	[`pypy:2`](#pypy2)
-	[`pypy:2-5`](#pypy2-5)
-	[`pypy:2-5.9`](#pypy2-59)
-	[`pypy:2-5.9.0`](#pypy2-590)
-	[`pypy:2-5.9.0-onbuild`](#pypy2-590-onbuild)
-	[`pypy:2-5.9.0-slim`](#pypy2-590-slim)
-	[`pypy:2-5.9-onbuild`](#pypy2-59-onbuild)
-	[`pypy:2-5.9-slim`](#pypy2-59-slim)
-	[`pypy:2-5-onbuild`](#pypy2-5-onbuild)
-	[`pypy:2-5-slim`](#pypy2-5-slim)
-	[`pypy:2-onbuild`](#pypy2-onbuild)
-	[`pypy:2-slim`](#pypy2-slim)
-	[`pypy:3`](#pypy3)
-	[`pypy:3-5`](#pypy3-5)
-	[`pypy:3-5.9`](#pypy3-59)
-	[`pypy:3-5.9.0`](#pypy3-590)
-	[`pypy:3-5.9.0-onbuild`](#pypy3-590-onbuild)
-	[`pypy:3-5.9.0-slim`](#pypy3-590-slim)
-	[`pypy:3-5.9-onbuild`](#pypy3-59-onbuild)
-	[`pypy:3-5.9-slim`](#pypy3-59-slim)
-	[`pypy:3-5-onbuild`](#pypy3-5-onbuild)
-	[`pypy:3-5-slim`](#pypy3-5-slim)
-	[`pypy:3-onbuild`](#pypy3-onbuild)
-	[`pypy:3-slim`](#pypy3-slim)
-	[`pypy:latest`](#pypylatest)
-	[`pypy:onbuild`](#pypyonbuild)
-	[`pypy:slim`](#pypyslim)

## `pypy:2`

```console
$ docker pull pypy@sha256:0a8ed0e6e50de0df4bc75dc1460539a08f2a6cd9fcfb21eff42c14eaabb0b8f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `pypy:2` - linux; amd64

```console
$ docker pull pypy@sha256:55ca52e21c9fc2b03a36772c75421a614990e887a5ed3fac7254737b7e576100
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.7 MB (281745795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cc4803a7f4c72a3fd8d4ae67d728abd25981aad0874e3e4ac63d49fad5250a`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:26:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 16:26:50 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:26:51 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b75493037494e7826da77e8b48bee4d15a7171acf45733e6ad9c22a32fea422`  
		Last Modified: Tue, 12 Dec 2017 16:28:25 GMT  
		Size: 24.8 MB (24771051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c1a97faf28f3e02142023746ac1899f3809d62878d41fccd35b16d6564ee7b`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.7 MB (3719646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2` - linux; arm variant v5

```console
$ docker pull pypy@sha256:5388354e7a371e1102e6c68aaa813f1005ebe32f0a3b527d5be7cb19a255fc33
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.3 MB (255292828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5daaf58e724b6d54c900bfcf6de571e40486e7ce2321dd547f42898aace2087`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 20:57:00 GMT
ADD file:2c2c6b8bfbbc9860c0ddd8a2ba3d769171576fc13d5d99fb50a852f6b03618d1 in / 
# Tue, 12 Dec 2017 20:57:00 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 22:52:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:52:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 22:54:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:56:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:52:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Dec 2017 00:52:55 GMT
ENV LANG=C.UTF-8
# Wed, 13 Dec 2017 00:53:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYPY_VERSION=5.9.0
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Wed, 13 Dec 2017 00:53:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Wed, 13 Dec 2017 00:54:00 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Wed, 13 Dec 2017 00:54:07 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:fbe67b6ec6f136174afee77eff07fd99e5764d9db2b13d0dc1189bf8203d289b`  
		Last Modified: Tue, 12 Dec 2017 21:06:47 GMT  
		Size: 50.9 MB (50882486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20452f83e704c3737bc38610443b6ca94edbe5388fb654b5c4c3c4308150785`  
		Last Modified: Tue, 12 Dec 2017 23:07:02 GMT  
		Size: 18.7 MB (18656894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b1e0d12986adcbf53895fa51052184e9f935a6424e8665bfad080be921ffec`  
		Last Modified: Tue, 12 Dec 2017 23:07:28 GMT  
		Size: 41.1 MB (41102373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3294d0e239416dcce73960614fcb72ab7e3034c5c0473cfc88120b49aaf8cf3`  
		Last Modified: Tue, 12 Dec 2017 23:08:09 GMT  
		Size: 115.7 MB (115740327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb10d9e21822b5858804af1906f60f0a667e581d0927089d9432869f10e7a5d9`  
		Last Modified: Wed, 13 Dec 2017 00:54:47 GMT  
		Size: 3.0 MB (3020433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc53514aa99843675aa2221aef86a6c1bce138eac6de239d2572e41717aff0b7`  
		Last Modified: Wed, 13 Dec 2017 00:54:55 GMT  
		Size: 22.2 MB (22170095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eea423ab6f26f0f128727c59477cda481f3e511e088be3cddaa4b548b3013b`  
		Last Modified: Wed, 13 Dec 2017 00:54:48 GMT  
		Size: 3.7 MB (3720220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2` - linux; arm variant v7

```console
$ docker pull pypy@sha256:73837d45c7a7977d9bf46de86520479011dcb029323314ce13c43f0b3672b9df
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249620434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52a767a974c50d09d53b411f172ce6870ca0da44b82726dda3c7c69b9fb02058`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:05 GMT
ADD file:aeb57f3a84dc1b93e1d38a80409a407df553344149d5070ed79b656865c90c54 in / 
# Tue, 12 Dec 2017 13:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:14:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:14:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 14:15:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:17:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 15:44:25 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:44:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 15:45:06 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 15:45:32 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 15:45:32 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:95e140a16c792899abc97cadee0138064dd21346fe51aa332ca4cbbd5563383c`  
		Last Modified: Tue, 12 Dec 2017 13:38:47 GMT  
		Size: 48.7 MB (48691755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237499cbbf2c5155fadc128c997700f0c5ec6355ba9704d0ec3f81c29640c9c4`  
		Last Modified: Tue, 12 Dec 2017 14:30:53 GMT  
		Size: 18.3 MB (18265038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f718f16c2f9a8213b99fcb49e72dad0036d1426f09c089f1e389b684f26520`  
		Last Modified: Tue, 12 Dec 2017 14:31:23 GMT  
		Size: 39.7 MB (39727713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affc0d5be2fb6b1dbb9d86ff0f533d88026215828cb4b1893257572ebf86f8d2`  
		Last Modified: Tue, 12 Dec 2017 14:32:10 GMT  
		Size: 114.1 MB (114057010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da492c2b2a6e64125a549432bf2b25c5d8fdb672fa3d27e1c9e5b6b493c28d4`  
		Last Modified: Tue, 12 Dec 2017 15:48:41 GMT  
		Size: 2.9 MB (2896866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1c900e416825525de3c49e77a9f71287afa1fa01ad6469e936a60f4e73bc30`  
		Last Modified: Tue, 12 Dec 2017 15:48:49 GMT  
		Size: 22.3 MB (22261764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e32dc2fb8080f66c1c6edb12faa4bf81f8660e27080c4eb0a8b61177203e308`  
		Last Modified: Tue, 12 Dec 2017 15:48:42 GMT  
		Size: 3.7 MB (3720288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2` - linux; 386

```console
$ docker pull pypy@sha256:13ea8b99309c3c217fdb96185fc657da43bfbc1ba8f7c26e33943eeea674b754
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281365939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8ab8d69ea517b7864e862c6a03e3f34b1d8723585681cf3f866fb9054fc7f63`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 14:19:55 GMT
ADD file:235a40e05b677eb2ae7e7a3cc5cbb0cda242ff15dddb87cb8dc9bb0cd2d6aed8 in / 
# Tue, 12 Dec 2017 14:19:55 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 16:53:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:53:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 16:54:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:56:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 21:56:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 21:56:55 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 21:57:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:03:46 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 22:03:56 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 22:03:56 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:d99577c7ee3d4d82987bedaeb10f3244ff7e19e41c5259bb8cac00568d1c4271`  
		Last Modified: Tue, 12 Dec 2017 14:46:26 GMT  
		Size: 52.8 MB (52777369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94aafa6d6f35f82e1fdc93cd4f7f6ab829f6297c8defaaa911dfb2de063bf3d`  
		Last Modified: Tue, 12 Dec 2017 17:27:39 GMT  
		Size: 21.6 MB (21596374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd19391b0ebd36e15e21cb3a6728c5950937634b9c81ecc7e3d1422b1dc25eb`  
		Last Modified: Tue, 12 Dec 2017 17:28:18 GMT  
		Size: 43.9 MB (43918299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8333879ca1894c745f67c724a7e4ad35542f5966a47bb050928910a944130ea0`  
		Last Modified: Tue, 12 Dec 2017 17:29:10 GMT  
		Size: 135.1 MB (135144789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5718f0e07ebd0ba7b1a182304b0f07394be9021b2ebad934f2a0b913390619cc`  
		Last Modified: Tue, 12 Dec 2017 22:10:00 GMT  
		Size: 3.3 MB (3271878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6c0ee3ad02226742c48a9260127e316949ec9b18e8e28c47f14bb1362fc38`  
		Last Modified: Tue, 12 Dec 2017 22:10:07 GMT  
		Size: 20.9 MB (20937530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aafba35b4500cd3009de7d3936f41dfcf9c23f56f743eb34541b0e9e82f67e`  
		Last Modified: Tue, 12 Dec 2017 22:09:59 GMT  
		Size: 3.7 MB (3719700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:2-5`

```console
$ docker pull pypy@sha256:0a8ed0e6e50de0df4bc75dc1460539a08f2a6cd9fcfb21eff42c14eaabb0b8f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `pypy:2-5` - linux; amd64

```console
$ docker pull pypy@sha256:55ca52e21c9fc2b03a36772c75421a614990e887a5ed3fac7254737b7e576100
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.7 MB (281745795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cc4803a7f4c72a3fd8d4ae67d728abd25981aad0874e3e4ac63d49fad5250a`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:26:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 16:26:50 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:26:51 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b75493037494e7826da77e8b48bee4d15a7171acf45733e6ad9c22a32fea422`  
		Last Modified: Tue, 12 Dec 2017 16:28:25 GMT  
		Size: 24.8 MB (24771051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c1a97faf28f3e02142023746ac1899f3809d62878d41fccd35b16d6564ee7b`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.7 MB (3719646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5` - linux; arm variant v5

```console
$ docker pull pypy@sha256:5388354e7a371e1102e6c68aaa813f1005ebe32f0a3b527d5be7cb19a255fc33
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.3 MB (255292828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5daaf58e724b6d54c900bfcf6de571e40486e7ce2321dd547f42898aace2087`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 20:57:00 GMT
ADD file:2c2c6b8bfbbc9860c0ddd8a2ba3d769171576fc13d5d99fb50a852f6b03618d1 in / 
# Tue, 12 Dec 2017 20:57:00 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 22:52:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:52:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 22:54:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:56:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:52:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Dec 2017 00:52:55 GMT
ENV LANG=C.UTF-8
# Wed, 13 Dec 2017 00:53:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYPY_VERSION=5.9.0
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Wed, 13 Dec 2017 00:53:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Wed, 13 Dec 2017 00:54:00 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Wed, 13 Dec 2017 00:54:07 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:fbe67b6ec6f136174afee77eff07fd99e5764d9db2b13d0dc1189bf8203d289b`  
		Last Modified: Tue, 12 Dec 2017 21:06:47 GMT  
		Size: 50.9 MB (50882486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20452f83e704c3737bc38610443b6ca94edbe5388fb654b5c4c3c4308150785`  
		Last Modified: Tue, 12 Dec 2017 23:07:02 GMT  
		Size: 18.7 MB (18656894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b1e0d12986adcbf53895fa51052184e9f935a6424e8665bfad080be921ffec`  
		Last Modified: Tue, 12 Dec 2017 23:07:28 GMT  
		Size: 41.1 MB (41102373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3294d0e239416dcce73960614fcb72ab7e3034c5c0473cfc88120b49aaf8cf3`  
		Last Modified: Tue, 12 Dec 2017 23:08:09 GMT  
		Size: 115.7 MB (115740327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb10d9e21822b5858804af1906f60f0a667e581d0927089d9432869f10e7a5d9`  
		Last Modified: Wed, 13 Dec 2017 00:54:47 GMT  
		Size: 3.0 MB (3020433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc53514aa99843675aa2221aef86a6c1bce138eac6de239d2572e41717aff0b7`  
		Last Modified: Wed, 13 Dec 2017 00:54:55 GMT  
		Size: 22.2 MB (22170095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eea423ab6f26f0f128727c59477cda481f3e511e088be3cddaa4b548b3013b`  
		Last Modified: Wed, 13 Dec 2017 00:54:48 GMT  
		Size: 3.7 MB (3720220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5` - linux; arm variant v7

```console
$ docker pull pypy@sha256:73837d45c7a7977d9bf46de86520479011dcb029323314ce13c43f0b3672b9df
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249620434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52a767a974c50d09d53b411f172ce6870ca0da44b82726dda3c7c69b9fb02058`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:05 GMT
ADD file:aeb57f3a84dc1b93e1d38a80409a407df553344149d5070ed79b656865c90c54 in / 
# Tue, 12 Dec 2017 13:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:14:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:14:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 14:15:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:17:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 15:44:25 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:44:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 15:45:06 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 15:45:32 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 15:45:32 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:95e140a16c792899abc97cadee0138064dd21346fe51aa332ca4cbbd5563383c`  
		Last Modified: Tue, 12 Dec 2017 13:38:47 GMT  
		Size: 48.7 MB (48691755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237499cbbf2c5155fadc128c997700f0c5ec6355ba9704d0ec3f81c29640c9c4`  
		Last Modified: Tue, 12 Dec 2017 14:30:53 GMT  
		Size: 18.3 MB (18265038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f718f16c2f9a8213b99fcb49e72dad0036d1426f09c089f1e389b684f26520`  
		Last Modified: Tue, 12 Dec 2017 14:31:23 GMT  
		Size: 39.7 MB (39727713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affc0d5be2fb6b1dbb9d86ff0f533d88026215828cb4b1893257572ebf86f8d2`  
		Last Modified: Tue, 12 Dec 2017 14:32:10 GMT  
		Size: 114.1 MB (114057010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da492c2b2a6e64125a549432bf2b25c5d8fdb672fa3d27e1c9e5b6b493c28d4`  
		Last Modified: Tue, 12 Dec 2017 15:48:41 GMT  
		Size: 2.9 MB (2896866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1c900e416825525de3c49e77a9f71287afa1fa01ad6469e936a60f4e73bc30`  
		Last Modified: Tue, 12 Dec 2017 15:48:49 GMT  
		Size: 22.3 MB (22261764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e32dc2fb8080f66c1c6edb12faa4bf81f8660e27080c4eb0a8b61177203e308`  
		Last Modified: Tue, 12 Dec 2017 15:48:42 GMT  
		Size: 3.7 MB (3720288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5` - linux; 386

```console
$ docker pull pypy@sha256:13ea8b99309c3c217fdb96185fc657da43bfbc1ba8f7c26e33943eeea674b754
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281365939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8ab8d69ea517b7864e862c6a03e3f34b1d8723585681cf3f866fb9054fc7f63`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 14:19:55 GMT
ADD file:235a40e05b677eb2ae7e7a3cc5cbb0cda242ff15dddb87cb8dc9bb0cd2d6aed8 in / 
# Tue, 12 Dec 2017 14:19:55 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 16:53:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:53:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 16:54:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:56:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 21:56:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 21:56:55 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 21:57:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:03:46 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 22:03:56 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 22:03:56 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:d99577c7ee3d4d82987bedaeb10f3244ff7e19e41c5259bb8cac00568d1c4271`  
		Last Modified: Tue, 12 Dec 2017 14:46:26 GMT  
		Size: 52.8 MB (52777369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94aafa6d6f35f82e1fdc93cd4f7f6ab829f6297c8defaaa911dfb2de063bf3d`  
		Last Modified: Tue, 12 Dec 2017 17:27:39 GMT  
		Size: 21.6 MB (21596374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd19391b0ebd36e15e21cb3a6728c5950937634b9c81ecc7e3d1422b1dc25eb`  
		Last Modified: Tue, 12 Dec 2017 17:28:18 GMT  
		Size: 43.9 MB (43918299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8333879ca1894c745f67c724a7e4ad35542f5966a47bb050928910a944130ea0`  
		Last Modified: Tue, 12 Dec 2017 17:29:10 GMT  
		Size: 135.1 MB (135144789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5718f0e07ebd0ba7b1a182304b0f07394be9021b2ebad934f2a0b913390619cc`  
		Last Modified: Tue, 12 Dec 2017 22:10:00 GMT  
		Size: 3.3 MB (3271878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6c0ee3ad02226742c48a9260127e316949ec9b18e8e28c47f14bb1362fc38`  
		Last Modified: Tue, 12 Dec 2017 22:10:07 GMT  
		Size: 20.9 MB (20937530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aafba35b4500cd3009de7d3936f41dfcf9c23f56f743eb34541b0e9e82f67e`  
		Last Modified: Tue, 12 Dec 2017 22:09:59 GMT  
		Size: 3.7 MB (3719700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:2-5.9`

```console
$ docker pull pypy@sha256:0a8ed0e6e50de0df4bc75dc1460539a08f2a6cd9fcfb21eff42c14eaabb0b8f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `pypy:2-5.9` - linux; amd64

```console
$ docker pull pypy@sha256:55ca52e21c9fc2b03a36772c75421a614990e887a5ed3fac7254737b7e576100
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.7 MB (281745795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cc4803a7f4c72a3fd8d4ae67d728abd25981aad0874e3e4ac63d49fad5250a`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:26:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 16:26:50 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:26:51 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b75493037494e7826da77e8b48bee4d15a7171acf45733e6ad9c22a32fea422`  
		Last Modified: Tue, 12 Dec 2017 16:28:25 GMT  
		Size: 24.8 MB (24771051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c1a97faf28f3e02142023746ac1899f3809d62878d41fccd35b16d6564ee7b`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.7 MB (3719646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9` - linux; arm variant v5

```console
$ docker pull pypy@sha256:5388354e7a371e1102e6c68aaa813f1005ebe32f0a3b527d5be7cb19a255fc33
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.3 MB (255292828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5daaf58e724b6d54c900bfcf6de571e40486e7ce2321dd547f42898aace2087`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 20:57:00 GMT
ADD file:2c2c6b8bfbbc9860c0ddd8a2ba3d769171576fc13d5d99fb50a852f6b03618d1 in / 
# Tue, 12 Dec 2017 20:57:00 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 22:52:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:52:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 22:54:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:56:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:52:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Dec 2017 00:52:55 GMT
ENV LANG=C.UTF-8
# Wed, 13 Dec 2017 00:53:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYPY_VERSION=5.9.0
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Wed, 13 Dec 2017 00:53:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Wed, 13 Dec 2017 00:54:00 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Wed, 13 Dec 2017 00:54:07 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:fbe67b6ec6f136174afee77eff07fd99e5764d9db2b13d0dc1189bf8203d289b`  
		Last Modified: Tue, 12 Dec 2017 21:06:47 GMT  
		Size: 50.9 MB (50882486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20452f83e704c3737bc38610443b6ca94edbe5388fb654b5c4c3c4308150785`  
		Last Modified: Tue, 12 Dec 2017 23:07:02 GMT  
		Size: 18.7 MB (18656894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b1e0d12986adcbf53895fa51052184e9f935a6424e8665bfad080be921ffec`  
		Last Modified: Tue, 12 Dec 2017 23:07:28 GMT  
		Size: 41.1 MB (41102373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3294d0e239416dcce73960614fcb72ab7e3034c5c0473cfc88120b49aaf8cf3`  
		Last Modified: Tue, 12 Dec 2017 23:08:09 GMT  
		Size: 115.7 MB (115740327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb10d9e21822b5858804af1906f60f0a667e581d0927089d9432869f10e7a5d9`  
		Last Modified: Wed, 13 Dec 2017 00:54:47 GMT  
		Size: 3.0 MB (3020433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc53514aa99843675aa2221aef86a6c1bce138eac6de239d2572e41717aff0b7`  
		Last Modified: Wed, 13 Dec 2017 00:54:55 GMT  
		Size: 22.2 MB (22170095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eea423ab6f26f0f128727c59477cda481f3e511e088be3cddaa4b548b3013b`  
		Last Modified: Wed, 13 Dec 2017 00:54:48 GMT  
		Size: 3.7 MB (3720220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9` - linux; arm variant v7

```console
$ docker pull pypy@sha256:73837d45c7a7977d9bf46de86520479011dcb029323314ce13c43f0b3672b9df
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249620434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52a767a974c50d09d53b411f172ce6870ca0da44b82726dda3c7c69b9fb02058`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:05 GMT
ADD file:aeb57f3a84dc1b93e1d38a80409a407df553344149d5070ed79b656865c90c54 in / 
# Tue, 12 Dec 2017 13:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:14:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:14:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 14:15:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:17:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 15:44:25 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:44:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 15:45:06 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 15:45:32 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 15:45:32 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:95e140a16c792899abc97cadee0138064dd21346fe51aa332ca4cbbd5563383c`  
		Last Modified: Tue, 12 Dec 2017 13:38:47 GMT  
		Size: 48.7 MB (48691755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237499cbbf2c5155fadc128c997700f0c5ec6355ba9704d0ec3f81c29640c9c4`  
		Last Modified: Tue, 12 Dec 2017 14:30:53 GMT  
		Size: 18.3 MB (18265038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f718f16c2f9a8213b99fcb49e72dad0036d1426f09c089f1e389b684f26520`  
		Last Modified: Tue, 12 Dec 2017 14:31:23 GMT  
		Size: 39.7 MB (39727713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affc0d5be2fb6b1dbb9d86ff0f533d88026215828cb4b1893257572ebf86f8d2`  
		Last Modified: Tue, 12 Dec 2017 14:32:10 GMT  
		Size: 114.1 MB (114057010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da492c2b2a6e64125a549432bf2b25c5d8fdb672fa3d27e1c9e5b6b493c28d4`  
		Last Modified: Tue, 12 Dec 2017 15:48:41 GMT  
		Size: 2.9 MB (2896866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1c900e416825525de3c49e77a9f71287afa1fa01ad6469e936a60f4e73bc30`  
		Last Modified: Tue, 12 Dec 2017 15:48:49 GMT  
		Size: 22.3 MB (22261764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e32dc2fb8080f66c1c6edb12faa4bf81f8660e27080c4eb0a8b61177203e308`  
		Last Modified: Tue, 12 Dec 2017 15:48:42 GMT  
		Size: 3.7 MB (3720288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9` - linux; 386

```console
$ docker pull pypy@sha256:13ea8b99309c3c217fdb96185fc657da43bfbc1ba8f7c26e33943eeea674b754
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281365939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8ab8d69ea517b7864e862c6a03e3f34b1d8723585681cf3f866fb9054fc7f63`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 14:19:55 GMT
ADD file:235a40e05b677eb2ae7e7a3cc5cbb0cda242ff15dddb87cb8dc9bb0cd2d6aed8 in / 
# Tue, 12 Dec 2017 14:19:55 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 16:53:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:53:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 16:54:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:56:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 21:56:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 21:56:55 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 21:57:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:03:46 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 22:03:56 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 22:03:56 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:d99577c7ee3d4d82987bedaeb10f3244ff7e19e41c5259bb8cac00568d1c4271`  
		Last Modified: Tue, 12 Dec 2017 14:46:26 GMT  
		Size: 52.8 MB (52777369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94aafa6d6f35f82e1fdc93cd4f7f6ab829f6297c8defaaa911dfb2de063bf3d`  
		Last Modified: Tue, 12 Dec 2017 17:27:39 GMT  
		Size: 21.6 MB (21596374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd19391b0ebd36e15e21cb3a6728c5950937634b9c81ecc7e3d1422b1dc25eb`  
		Last Modified: Tue, 12 Dec 2017 17:28:18 GMT  
		Size: 43.9 MB (43918299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8333879ca1894c745f67c724a7e4ad35542f5966a47bb050928910a944130ea0`  
		Last Modified: Tue, 12 Dec 2017 17:29:10 GMT  
		Size: 135.1 MB (135144789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5718f0e07ebd0ba7b1a182304b0f07394be9021b2ebad934f2a0b913390619cc`  
		Last Modified: Tue, 12 Dec 2017 22:10:00 GMT  
		Size: 3.3 MB (3271878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6c0ee3ad02226742c48a9260127e316949ec9b18e8e28c47f14bb1362fc38`  
		Last Modified: Tue, 12 Dec 2017 22:10:07 GMT  
		Size: 20.9 MB (20937530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aafba35b4500cd3009de7d3936f41dfcf9c23f56f743eb34541b0e9e82f67e`  
		Last Modified: Tue, 12 Dec 2017 22:09:59 GMT  
		Size: 3.7 MB (3719700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:2-5.9.0`

```console
$ docker pull pypy@sha256:0a8ed0e6e50de0df4bc75dc1460539a08f2a6cd9fcfb21eff42c14eaabb0b8f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `pypy:2-5.9.0` - linux; amd64

```console
$ docker pull pypy@sha256:55ca52e21c9fc2b03a36772c75421a614990e887a5ed3fac7254737b7e576100
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.7 MB (281745795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cc4803a7f4c72a3fd8d4ae67d728abd25981aad0874e3e4ac63d49fad5250a`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:26:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 16:26:50 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:26:51 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b75493037494e7826da77e8b48bee4d15a7171acf45733e6ad9c22a32fea422`  
		Last Modified: Tue, 12 Dec 2017 16:28:25 GMT  
		Size: 24.8 MB (24771051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c1a97faf28f3e02142023746ac1899f3809d62878d41fccd35b16d6564ee7b`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.7 MB (3719646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9.0` - linux; arm variant v5

```console
$ docker pull pypy@sha256:5388354e7a371e1102e6c68aaa813f1005ebe32f0a3b527d5be7cb19a255fc33
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.3 MB (255292828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5daaf58e724b6d54c900bfcf6de571e40486e7ce2321dd547f42898aace2087`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 20:57:00 GMT
ADD file:2c2c6b8bfbbc9860c0ddd8a2ba3d769171576fc13d5d99fb50a852f6b03618d1 in / 
# Tue, 12 Dec 2017 20:57:00 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 22:52:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:52:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 22:54:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:56:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:52:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Dec 2017 00:52:55 GMT
ENV LANG=C.UTF-8
# Wed, 13 Dec 2017 00:53:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYPY_VERSION=5.9.0
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Wed, 13 Dec 2017 00:53:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Wed, 13 Dec 2017 00:54:00 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Wed, 13 Dec 2017 00:54:07 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:fbe67b6ec6f136174afee77eff07fd99e5764d9db2b13d0dc1189bf8203d289b`  
		Last Modified: Tue, 12 Dec 2017 21:06:47 GMT  
		Size: 50.9 MB (50882486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20452f83e704c3737bc38610443b6ca94edbe5388fb654b5c4c3c4308150785`  
		Last Modified: Tue, 12 Dec 2017 23:07:02 GMT  
		Size: 18.7 MB (18656894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b1e0d12986adcbf53895fa51052184e9f935a6424e8665bfad080be921ffec`  
		Last Modified: Tue, 12 Dec 2017 23:07:28 GMT  
		Size: 41.1 MB (41102373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3294d0e239416dcce73960614fcb72ab7e3034c5c0473cfc88120b49aaf8cf3`  
		Last Modified: Tue, 12 Dec 2017 23:08:09 GMT  
		Size: 115.7 MB (115740327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb10d9e21822b5858804af1906f60f0a667e581d0927089d9432869f10e7a5d9`  
		Last Modified: Wed, 13 Dec 2017 00:54:47 GMT  
		Size: 3.0 MB (3020433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc53514aa99843675aa2221aef86a6c1bce138eac6de239d2572e41717aff0b7`  
		Last Modified: Wed, 13 Dec 2017 00:54:55 GMT  
		Size: 22.2 MB (22170095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eea423ab6f26f0f128727c59477cda481f3e511e088be3cddaa4b548b3013b`  
		Last Modified: Wed, 13 Dec 2017 00:54:48 GMT  
		Size: 3.7 MB (3720220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9.0` - linux; arm variant v7

```console
$ docker pull pypy@sha256:73837d45c7a7977d9bf46de86520479011dcb029323314ce13c43f0b3672b9df
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249620434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52a767a974c50d09d53b411f172ce6870ca0da44b82726dda3c7c69b9fb02058`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:05 GMT
ADD file:aeb57f3a84dc1b93e1d38a80409a407df553344149d5070ed79b656865c90c54 in / 
# Tue, 12 Dec 2017 13:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:14:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:14:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 14:15:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:17:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 15:44:25 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:44:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 15:45:06 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 15:45:32 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 15:45:32 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:95e140a16c792899abc97cadee0138064dd21346fe51aa332ca4cbbd5563383c`  
		Last Modified: Tue, 12 Dec 2017 13:38:47 GMT  
		Size: 48.7 MB (48691755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237499cbbf2c5155fadc128c997700f0c5ec6355ba9704d0ec3f81c29640c9c4`  
		Last Modified: Tue, 12 Dec 2017 14:30:53 GMT  
		Size: 18.3 MB (18265038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f718f16c2f9a8213b99fcb49e72dad0036d1426f09c089f1e389b684f26520`  
		Last Modified: Tue, 12 Dec 2017 14:31:23 GMT  
		Size: 39.7 MB (39727713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affc0d5be2fb6b1dbb9d86ff0f533d88026215828cb4b1893257572ebf86f8d2`  
		Last Modified: Tue, 12 Dec 2017 14:32:10 GMT  
		Size: 114.1 MB (114057010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da492c2b2a6e64125a549432bf2b25c5d8fdb672fa3d27e1c9e5b6b493c28d4`  
		Last Modified: Tue, 12 Dec 2017 15:48:41 GMT  
		Size: 2.9 MB (2896866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1c900e416825525de3c49e77a9f71287afa1fa01ad6469e936a60f4e73bc30`  
		Last Modified: Tue, 12 Dec 2017 15:48:49 GMT  
		Size: 22.3 MB (22261764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e32dc2fb8080f66c1c6edb12faa4bf81f8660e27080c4eb0a8b61177203e308`  
		Last Modified: Tue, 12 Dec 2017 15:48:42 GMT  
		Size: 3.7 MB (3720288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9.0` - linux; 386

```console
$ docker pull pypy@sha256:13ea8b99309c3c217fdb96185fc657da43bfbc1ba8f7c26e33943eeea674b754
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281365939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8ab8d69ea517b7864e862c6a03e3f34b1d8723585681cf3f866fb9054fc7f63`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 14:19:55 GMT
ADD file:235a40e05b677eb2ae7e7a3cc5cbb0cda242ff15dddb87cb8dc9bb0cd2d6aed8 in / 
# Tue, 12 Dec 2017 14:19:55 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 16:53:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:53:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 16:54:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:56:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 21:56:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 21:56:55 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 21:57:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:03:46 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 22:03:56 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 22:03:56 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:d99577c7ee3d4d82987bedaeb10f3244ff7e19e41c5259bb8cac00568d1c4271`  
		Last Modified: Tue, 12 Dec 2017 14:46:26 GMT  
		Size: 52.8 MB (52777369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94aafa6d6f35f82e1fdc93cd4f7f6ab829f6297c8defaaa911dfb2de063bf3d`  
		Last Modified: Tue, 12 Dec 2017 17:27:39 GMT  
		Size: 21.6 MB (21596374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd19391b0ebd36e15e21cb3a6728c5950937634b9c81ecc7e3d1422b1dc25eb`  
		Last Modified: Tue, 12 Dec 2017 17:28:18 GMT  
		Size: 43.9 MB (43918299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8333879ca1894c745f67c724a7e4ad35542f5966a47bb050928910a944130ea0`  
		Last Modified: Tue, 12 Dec 2017 17:29:10 GMT  
		Size: 135.1 MB (135144789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5718f0e07ebd0ba7b1a182304b0f07394be9021b2ebad934f2a0b913390619cc`  
		Last Modified: Tue, 12 Dec 2017 22:10:00 GMT  
		Size: 3.3 MB (3271878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6c0ee3ad02226742c48a9260127e316949ec9b18e8e28c47f14bb1362fc38`  
		Last Modified: Tue, 12 Dec 2017 22:10:07 GMT  
		Size: 20.9 MB (20937530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aafba35b4500cd3009de7d3936f41dfcf9c23f56f743eb34541b0e9e82f67e`  
		Last Modified: Tue, 12 Dec 2017 22:09:59 GMT  
		Size: 3.7 MB (3719700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:2-5.9.0-onbuild`

```console
$ docker pull pypy@sha256:58df33485c9d0a54a46525dcdfdf0f62d128d3cc9bd561697569e2a6236d2337
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `pypy:2-5.9.0-onbuild` - linux; amd64

```console
$ docker pull pypy@sha256:cbb4e4d19e76e0074d1defb33ee58833b953c1de0e342afb24a2263227e10320
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.7 MB (281745927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e51bd583a797c3bca6cb502f1a48b7ee142cd6af03033b5376d55201f9c0f32b`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:26:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 16:26:50 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:26:51 GMT
CMD ["pypy"]
# Tue, 12 Dec 2017 16:27:12 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 16:27:12 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 16:27:12 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 16:27:13 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 16:27:13 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b75493037494e7826da77e8b48bee4d15a7171acf45733e6ad9c22a32fea422`  
		Last Modified: Tue, 12 Dec 2017 16:28:25 GMT  
		Size: 24.8 MB (24771051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c1a97faf28f3e02142023746ac1899f3809d62878d41fccd35b16d6564ee7b`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.7 MB (3719646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c73e8333ea54a6ccd0af1dc19b3d01e43e9634a8efb6f7f4b92d27908b236a`  
		Last Modified: Tue, 12 Dec 2017 16:29:15 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9.0-onbuild` - linux; arm variant v5

```console
$ docker pull pypy@sha256:ead1ac231c6aca599292aae016ca59d0b44ecc96595d9207534181f286dfa8a5
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.3 MB (255292993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d4d9360eeb526d829828552047ac1dcfcf3f3ce683e8d99e9a421634975764`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 20:57:00 GMT
ADD file:2c2c6b8bfbbc9860c0ddd8a2ba3d769171576fc13d5d99fb50a852f6b03618d1 in / 
# Tue, 12 Dec 2017 20:57:00 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 22:52:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:52:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 22:54:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:56:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:52:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Dec 2017 00:52:55 GMT
ENV LANG=C.UTF-8
# Wed, 13 Dec 2017 00:53:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYPY_VERSION=5.9.0
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Wed, 13 Dec 2017 00:53:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Wed, 13 Dec 2017 00:54:00 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Wed, 13 Dec 2017 00:54:07 GMT
CMD ["pypy"]
# Wed, 13 Dec 2017 00:54:30 GMT
RUN mkdir -p /usr/src/app
# Wed, 13 Dec 2017 00:54:30 GMT
WORKDIR /usr/src/app
# Wed, 13 Dec 2017 00:54:30 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Wed, 13 Dec 2017 00:54:31 GMT
ONBUILD RUN pip install -r requirements.txt
# Wed, 13 Dec 2017 00:54:31 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:fbe67b6ec6f136174afee77eff07fd99e5764d9db2b13d0dc1189bf8203d289b`  
		Last Modified: Tue, 12 Dec 2017 21:06:47 GMT  
		Size: 50.9 MB (50882486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20452f83e704c3737bc38610443b6ca94edbe5388fb654b5c4c3c4308150785`  
		Last Modified: Tue, 12 Dec 2017 23:07:02 GMT  
		Size: 18.7 MB (18656894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b1e0d12986adcbf53895fa51052184e9f935a6424e8665bfad080be921ffec`  
		Last Modified: Tue, 12 Dec 2017 23:07:28 GMT  
		Size: 41.1 MB (41102373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3294d0e239416dcce73960614fcb72ab7e3034c5c0473cfc88120b49aaf8cf3`  
		Last Modified: Tue, 12 Dec 2017 23:08:09 GMT  
		Size: 115.7 MB (115740327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb10d9e21822b5858804af1906f60f0a667e581d0927089d9432869f10e7a5d9`  
		Last Modified: Wed, 13 Dec 2017 00:54:47 GMT  
		Size: 3.0 MB (3020433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc53514aa99843675aa2221aef86a6c1bce138eac6de239d2572e41717aff0b7`  
		Last Modified: Wed, 13 Dec 2017 00:54:55 GMT  
		Size: 22.2 MB (22170095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eea423ab6f26f0f128727c59477cda481f3e511e088be3cddaa4b548b3013b`  
		Last Modified: Wed, 13 Dec 2017 00:54:48 GMT  
		Size: 3.7 MB (3720220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f655a96258796da628a9bfe71df82779071ca0516242b076bc799eaeb165eb4`  
		Last Modified: Wed, 13 Dec 2017 00:55:34 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9.0-onbuild` - linux; arm variant v7

```console
$ docker pull pypy@sha256:8fb93eb68f4c911e321528719d69ddcc84af317771961d8c954f5d4be9f0dc6f
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249620597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac28a04335460f2d03c5a2298b30d71d8b90ab531e0943414e06b2cdf24a70bd`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:05 GMT
ADD file:aeb57f3a84dc1b93e1d38a80409a407df553344149d5070ed79b656865c90c54 in / 
# Tue, 12 Dec 2017 13:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:14:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:14:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 14:15:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:17:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 15:44:25 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:44:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 15:45:06 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 15:45:32 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 15:45:32 GMT
CMD ["pypy"]
# Tue, 12 Dec 2017 15:48:21 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 15:48:21 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 15:48:22 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 15:48:22 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 15:48:22 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:95e140a16c792899abc97cadee0138064dd21346fe51aa332ca4cbbd5563383c`  
		Last Modified: Tue, 12 Dec 2017 13:38:47 GMT  
		Size: 48.7 MB (48691755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237499cbbf2c5155fadc128c997700f0c5ec6355ba9704d0ec3f81c29640c9c4`  
		Last Modified: Tue, 12 Dec 2017 14:30:53 GMT  
		Size: 18.3 MB (18265038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f718f16c2f9a8213b99fcb49e72dad0036d1426f09c089f1e389b684f26520`  
		Last Modified: Tue, 12 Dec 2017 14:31:23 GMT  
		Size: 39.7 MB (39727713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affc0d5be2fb6b1dbb9d86ff0f533d88026215828cb4b1893257572ebf86f8d2`  
		Last Modified: Tue, 12 Dec 2017 14:32:10 GMT  
		Size: 114.1 MB (114057010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da492c2b2a6e64125a549432bf2b25c5d8fdb672fa3d27e1c9e5b6b493c28d4`  
		Last Modified: Tue, 12 Dec 2017 15:48:41 GMT  
		Size: 2.9 MB (2896866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1c900e416825525de3c49e77a9f71287afa1fa01ad6469e936a60f4e73bc30`  
		Last Modified: Tue, 12 Dec 2017 15:48:49 GMT  
		Size: 22.3 MB (22261764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e32dc2fb8080f66c1c6edb12faa4bf81f8660e27080c4eb0a8b61177203e308`  
		Last Modified: Tue, 12 Dec 2017 15:48:42 GMT  
		Size: 3.7 MB (3720288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6de7019ddc357de708f6542fac5dbb2a00898b592f55581d094d2958c1a72e8`  
		Last Modified: Tue, 12 Dec 2017 15:50:30 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9.0-onbuild` - linux; 386

```console
$ docker pull pypy@sha256:abce1ce483117a2aa8e27648543aedf0532fee84205bd6babbbf8a1fe3c40b64
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281366071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:765310362b69c1fd19344acbe069dc44a5615499f0f61b909d5a50921669446d`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 14:19:55 GMT
ADD file:235a40e05b677eb2ae7e7a3cc5cbb0cda242ff15dddb87cb8dc9bb0cd2d6aed8 in / 
# Tue, 12 Dec 2017 14:19:55 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 16:53:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:53:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 16:54:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:56:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 21:56:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 21:56:55 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 21:57:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:03:46 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 22:03:56 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 22:03:56 GMT
CMD ["pypy"]
# Tue, 12 Dec 2017 22:09:39 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 22:09:39 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 22:09:39 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 22:09:39 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 22:09:40 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:d99577c7ee3d4d82987bedaeb10f3244ff7e19e41c5259bb8cac00568d1c4271`  
		Last Modified: Tue, 12 Dec 2017 14:46:26 GMT  
		Size: 52.8 MB (52777369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94aafa6d6f35f82e1fdc93cd4f7f6ab829f6297c8defaaa911dfb2de063bf3d`  
		Last Modified: Tue, 12 Dec 2017 17:27:39 GMT  
		Size: 21.6 MB (21596374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd19391b0ebd36e15e21cb3a6728c5950937634b9c81ecc7e3d1422b1dc25eb`  
		Last Modified: Tue, 12 Dec 2017 17:28:18 GMT  
		Size: 43.9 MB (43918299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8333879ca1894c745f67c724a7e4ad35542f5966a47bb050928910a944130ea0`  
		Last Modified: Tue, 12 Dec 2017 17:29:10 GMT  
		Size: 135.1 MB (135144789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5718f0e07ebd0ba7b1a182304b0f07394be9021b2ebad934f2a0b913390619cc`  
		Last Modified: Tue, 12 Dec 2017 22:10:00 GMT  
		Size: 3.3 MB (3271878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6c0ee3ad02226742c48a9260127e316949ec9b18e8e28c47f14bb1362fc38`  
		Last Modified: Tue, 12 Dec 2017 22:10:07 GMT  
		Size: 20.9 MB (20937530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aafba35b4500cd3009de7d3936f41dfcf9c23f56f743eb34541b0e9e82f67e`  
		Last Modified: Tue, 12 Dec 2017 22:09:59 GMT  
		Size: 3.7 MB (3719700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5023694a0d55bd510c6e9cf8ff7f7e924f82f23f8dc2d62eddf991b36d275e1`  
		Last Modified: Tue, 12 Dec 2017 22:14:40 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:2-5.9.0-slim`

```console
$ docker pull pypy@sha256:f6273e4a29678a968239b91ce0c130404fa73146bfc26fa9d5b9b06edc259cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `pypy:2-5.9.0-slim` - linux; amd64

```console
$ docker pull pypy@sha256:c08046309aa3c069d4271a6b528ca89bc1b81354b8f8d60ae2b966c5063edd51
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61704534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9499c15fb67f97f95a978ce2b597b22b20b437873c82bafbe62cae4b4ce894`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 06:21:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 06:21:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 06:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 06:22:17 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 06:26:44 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ed6d99248693c2acd5109ff75533464052952167eca48dbf989268a392ebb3`  
		Last Modified: Tue, 12 Dec 2017 06:28:04 GMT  
		Size: 2.9 MB (2859578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23aa754ac2ff99b4b15fd8d3a949cbcab6921a922c40364c70d4a50f86f0094`  
		Last Modified: Tue, 12 Dec 2017 06:28:13 GMT  
		Size: 28.7 MB (28730437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9.0-slim` - linux; arm variant v5

```console
$ docker pull pypy@sha256:8eca5d74aa8367146860be6ebc278d243c949b309c469e5643c691a10e3aac61
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57159408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9bbc15f5cbca846158f77e88492d3f89ec922df0734b6345e2d6cfff6eb7c58`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 20:57:33 GMT
ADD file:29d0e44ebcc6f8dc2cfbc86c5034380677d263e9eec27a22ba045e0810836f81 in / 
# Tue, 12 Dec 2017 20:57:34 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 21:39:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 21:39:31 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 22:43:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:43:51 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:43:52 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:45:01 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 22:45:01 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:51e696f556166d0e25b3b27c824c4aafbddd5adcfd3f5186c09707f7baa3b312`  
		Last Modified: Tue, 12 Dec 2017 21:07:41 GMT  
		Size: 28.4 MB (28423526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e1f15069f149f59c18e22308fea3709837800f0d2954fbbc664799384ce6f`  
		Last Modified: Tue, 12 Dec 2017 22:45:35 GMT  
		Size: 2.6 MB (2608019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d5ced759aea47a18744948db8210418d363f4c785c37621006690d33a849d0`  
		Last Modified: Tue, 12 Dec 2017 22:45:43 GMT  
		Size: 26.1 MB (26127863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9.0-slim` - linux; arm variant v7

```console
$ docker pull pypy@sha256:99f5e7c41121ec0002d2b6d42a6c1a6a70752d3b4fe9a7489903466fc26a4794
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54978226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c84e3fcb1b4f28072773a645e9289b7d71f4f40e437045dbf21bcfb8fdbe57f`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:47 GMT
ADD file:1f5de474caa19da14d698a3f9c3d161abfa1e19e258a596d64f3dfc9e2f17686 in / 
# Tue, 12 Dec 2017 13:27:47 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 15:45:53 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 15:45:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:46:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:46:40 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 15:46:40 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 15:47:55 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 15:47:56 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:4b9c0f1a415433a98643bdda391dcf4fe5d9653fc3ed3845c7ac1be99eb43399`  
		Last Modified: Tue, 12 Dec 2017 13:39:52 GMT  
		Size: 26.3 MB (26282714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b37d60058a7d8edcada55701fe95ca118eff0b137ab3206001d6474c585038`  
		Last Modified: Tue, 12 Dec 2017 15:49:35 GMT  
		Size: 2.5 MB (2476158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93ad39ea9b5f53578215b6778f1e247029486b986e315e7f3df940b6942295a`  
		Last Modified: Tue, 12 Dec 2017 15:49:45 GMT  
		Size: 26.2 MB (26219354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9.0-slim` - linux; 386

```console
$ docker pull pypy@sha256:beb12510a29e6079a3e3ebfdbaaffc9855b40c4853111082582388e60bb703c9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60124197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2723d47c4e453dcbe9be3f47a500402f6d2ff3f4f35564870d48a636551f1481`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 14:21:05 GMT
ADD file:d31765999b40e32b628f3ec72b762f007f4918b08c507484e425adc990c87c26 in / 
# Tue, 12 Dec 2017 14:21:05 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 22:02:21 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 22:02:22 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 22:08:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:08:30 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:08:30 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:09:17 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 22:09:18 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:6b323e7c684c46ec9e577d3acb692c7e1c0c26ffbea6a4530dbe784a7eedf0f7`  
		Last Modified: Tue, 12 Dec 2017 14:49:35 GMT  
		Size: 30.3 MB (30266257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846baa5afdbb2caec4218e67e02a9b0793718ada3ec4d2a8c4d9ebe7c73c0713`  
		Last Modified: Tue, 12 Dec 2017 22:13:37 GMT  
		Size: 5.0 MB (4957755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e87231048cecb4fc4c3514e7c9e469c45e7eb6123e8ac4862540fd894f63612`  
		Last Modified: Tue, 12 Dec 2017 22:13:45 GMT  
		Size: 24.9 MB (24900185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:2-5.9-onbuild`

```console
$ docker pull pypy@sha256:58df33485c9d0a54a46525dcdfdf0f62d128d3cc9bd561697569e2a6236d2337
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `pypy:2-5.9-onbuild` - linux; amd64

```console
$ docker pull pypy@sha256:cbb4e4d19e76e0074d1defb33ee58833b953c1de0e342afb24a2263227e10320
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.7 MB (281745927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e51bd583a797c3bca6cb502f1a48b7ee142cd6af03033b5376d55201f9c0f32b`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:26:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 16:26:50 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:26:51 GMT
CMD ["pypy"]
# Tue, 12 Dec 2017 16:27:12 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 16:27:12 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 16:27:12 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 16:27:13 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 16:27:13 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b75493037494e7826da77e8b48bee4d15a7171acf45733e6ad9c22a32fea422`  
		Last Modified: Tue, 12 Dec 2017 16:28:25 GMT  
		Size: 24.8 MB (24771051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c1a97faf28f3e02142023746ac1899f3809d62878d41fccd35b16d6564ee7b`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.7 MB (3719646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c73e8333ea54a6ccd0af1dc19b3d01e43e9634a8efb6f7f4b92d27908b236a`  
		Last Modified: Tue, 12 Dec 2017 16:29:15 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9-onbuild` - linux; arm variant v5

```console
$ docker pull pypy@sha256:ead1ac231c6aca599292aae016ca59d0b44ecc96595d9207534181f286dfa8a5
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.3 MB (255292993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d4d9360eeb526d829828552047ac1dcfcf3f3ce683e8d99e9a421634975764`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 20:57:00 GMT
ADD file:2c2c6b8bfbbc9860c0ddd8a2ba3d769171576fc13d5d99fb50a852f6b03618d1 in / 
# Tue, 12 Dec 2017 20:57:00 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 22:52:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:52:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 22:54:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:56:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:52:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Dec 2017 00:52:55 GMT
ENV LANG=C.UTF-8
# Wed, 13 Dec 2017 00:53:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYPY_VERSION=5.9.0
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Wed, 13 Dec 2017 00:53:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Wed, 13 Dec 2017 00:54:00 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Wed, 13 Dec 2017 00:54:07 GMT
CMD ["pypy"]
# Wed, 13 Dec 2017 00:54:30 GMT
RUN mkdir -p /usr/src/app
# Wed, 13 Dec 2017 00:54:30 GMT
WORKDIR /usr/src/app
# Wed, 13 Dec 2017 00:54:30 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Wed, 13 Dec 2017 00:54:31 GMT
ONBUILD RUN pip install -r requirements.txt
# Wed, 13 Dec 2017 00:54:31 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:fbe67b6ec6f136174afee77eff07fd99e5764d9db2b13d0dc1189bf8203d289b`  
		Last Modified: Tue, 12 Dec 2017 21:06:47 GMT  
		Size: 50.9 MB (50882486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20452f83e704c3737bc38610443b6ca94edbe5388fb654b5c4c3c4308150785`  
		Last Modified: Tue, 12 Dec 2017 23:07:02 GMT  
		Size: 18.7 MB (18656894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b1e0d12986adcbf53895fa51052184e9f935a6424e8665bfad080be921ffec`  
		Last Modified: Tue, 12 Dec 2017 23:07:28 GMT  
		Size: 41.1 MB (41102373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3294d0e239416dcce73960614fcb72ab7e3034c5c0473cfc88120b49aaf8cf3`  
		Last Modified: Tue, 12 Dec 2017 23:08:09 GMT  
		Size: 115.7 MB (115740327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb10d9e21822b5858804af1906f60f0a667e581d0927089d9432869f10e7a5d9`  
		Last Modified: Wed, 13 Dec 2017 00:54:47 GMT  
		Size: 3.0 MB (3020433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc53514aa99843675aa2221aef86a6c1bce138eac6de239d2572e41717aff0b7`  
		Last Modified: Wed, 13 Dec 2017 00:54:55 GMT  
		Size: 22.2 MB (22170095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eea423ab6f26f0f128727c59477cda481f3e511e088be3cddaa4b548b3013b`  
		Last Modified: Wed, 13 Dec 2017 00:54:48 GMT  
		Size: 3.7 MB (3720220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f655a96258796da628a9bfe71df82779071ca0516242b076bc799eaeb165eb4`  
		Last Modified: Wed, 13 Dec 2017 00:55:34 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9-onbuild` - linux; arm variant v7

```console
$ docker pull pypy@sha256:8fb93eb68f4c911e321528719d69ddcc84af317771961d8c954f5d4be9f0dc6f
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249620597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac28a04335460f2d03c5a2298b30d71d8b90ab531e0943414e06b2cdf24a70bd`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:05 GMT
ADD file:aeb57f3a84dc1b93e1d38a80409a407df553344149d5070ed79b656865c90c54 in / 
# Tue, 12 Dec 2017 13:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:14:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:14:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 14:15:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:17:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 15:44:25 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:44:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 15:45:06 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 15:45:32 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 15:45:32 GMT
CMD ["pypy"]
# Tue, 12 Dec 2017 15:48:21 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 15:48:21 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 15:48:22 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 15:48:22 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 15:48:22 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:95e140a16c792899abc97cadee0138064dd21346fe51aa332ca4cbbd5563383c`  
		Last Modified: Tue, 12 Dec 2017 13:38:47 GMT  
		Size: 48.7 MB (48691755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237499cbbf2c5155fadc128c997700f0c5ec6355ba9704d0ec3f81c29640c9c4`  
		Last Modified: Tue, 12 Dec 2017 14:30:53 GMT  
		Size: 18.3 MB (18265038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f718f16c2f9a8213b99fcb49e72dad0036d1426f09c089f1e389b684f26520`  
		Last Modified: Tue, 12 Dec 2017 14:31:23 GMT  
		Size: 39.7 MB (39727713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affc0d5be2fb6b1dbb9d86ff0f533d88026215828cb4b1893257572ebf86f8d2`  
		Last Modified: Tue, 12 Dec 2017 14:32:10 GMT  
		Size: 114.1 MB (114057010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da492c2b2a6e64125a549432bf2b25c5d8fdb672fa3d27e1c9e5b6b493c28d4`  
		Last Modified: Tue, 12 Dec 2017 15:48:41 GMT  
		Size: 2.9 MB (2896866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1c900e416825525de3c49e77a9f71287afa1fa01ad6469e936a60f4e73bc30`  
		Last Modified: Tue, 12 Dec 2017 15:48:49 GMT  
		Size: 22.3 MB (22261764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e32dc2fb8080f66c1c6edb12faa4bf81f8660e27080c4eb0a8b61177203e308`  
		Last Modified: Tue, 12 Dec 2017 15:48:42 GMT  
		Size: 3.7 MB (3720288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6de7019ddc357de708f6542fac5dbb2a00898b592f55581d094d2958c1a72e8`  
		Last Modified: Tue, 12 Dec 2017 15:50:30 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9-onbuild` - linux; 386

```console
$ docker pull pypy@sha256:abce1ce483117a2aa8e27648543aedf0532fee84205bd6babbbf8a1fe3c40b64
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281366071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:765310362b69c1fd19344acbe069dc44a5615499f0f61b909d5a50921669446d`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 14:19:55 GMT
ADD file:235a40e05b677eb2ae7e7a3cc5cbb0cda242ff15dddb87cb8dc9bb0cd2d6aed8 in / 
# Tue, 12 Dec 2017 14:19:55 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 16:53:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:53:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 16:54:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:56:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 21:56:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 21:56:55 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 21:57:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:03:46 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 22:03:56 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 22:03:56 GMT
CMD ["pypy"]
# Tue, 12 Dec 2017 22:09:39 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 22:09:39 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 22:09:39 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 22:09:39 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 22:09:40 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:d99577c7ee3d4d82987bedaeb10f3244ff7e19e41c5259bb8cac00568d1c4271`  
		Last Modified: Tue, 12 Dec 2017 14:46:26 GMT  
		Size: 52.8 MB (52777369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94aafa6d6f35f82e1fdc93cd4f7f6ab829f6297c8defaaa911dfb2de063bf3d`  
		Last Modified: Tue, 12 Dec 2017 17:27:39 GMT  
		Size: 21.6 MB (21596374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd19391b0ebd36e15e21cb3a6728c5950937634b9c81ecc7e3d1422b1dc25eb`  
		Last Modified: Tue, 12 Dec 2017 17:28:18 GMT  
		Size: 43.9 MB (43918299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8333879ca1894c745f67c724a7e4ad35542f5966a47bb050928910a944130ea0`  
		Last Modified: Tue, 12 Dec 2017 17:29:10 GMT  
		Size: 135.1 MB (135144789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5718f0e07ebd0ba7b1a182304b0f07394be9021b2ebad934f2a0b913390619cc`  
		Last Modified: Tue, 12 Dec 2017 22:10:00 GMT  
		Size: 3.3 MB (3271878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6c0ee3ad02226742c48a9260127e316949ec9b18e8e28c47f14bb1362fc38`  
		Last Modified: Tue, 12 Dec 2017 22:10:07 GMT  
		Size: 20.9 MB (20937530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aafba35b4500cd3009de7d3936f41dfcf9c23f56f743eb34541b0e9e82f67e`  
		Last Modified: Tue, 12 Dec 2017 22:09:59 GMT  
		Size: 3.7 MB (3719700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5023694a0d55bd510c6e9cf8ff7f7e924f82f23f8dc2d62eddf991b36d275e1`  
		Last Modified: Tue, 12 Dec 2017 22:14:40 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:2-5.9-slim`

```console
$ docker pull pypy@sha256:f6273e4a29678a968239b91ce0c130404fa73146bfc26fa9d5b9b06edc259cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `pypy:2-5.9-slim` - linux; amd64

```console
$ docker pull pypy@sha256:c08046309aa3c069d4271a6b528ca89bc1b81354b8f8d60ae2b966c5063edd51
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61704534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9499c15fb67f97f95a978ce2b597b22b20b437873c82bafbe62cae4b4ce894`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 06:21:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 06:21:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 06:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 06:22:17 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 06:26:44 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ed6d99248693c2acd5109ff75533464052952167eca48dbf989268a392ebb3`  
		Last Modified: Tue, 12 Dec 2017 06:28:04 GMT  
		Size: 2.9 MB (2859578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23aa754ac2ff99b4b15fd8d3a949cbcab6921a922c40364c70d4a50f86f0094`  
		Last Modified: Tue, 12 Dec 2017 06:28:13 GMT  
		Size: 28.7 MB (28730437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9-slim` - linux; arm variant v5

```console
$ docker pull pypy@sha256:8eca5d74aa8367146860be6ebc278d243c949b309c469e5643c691a10e3aac61
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57159408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9bbc15f5cbca846158f77e88492d3f89ec922df0734b6345e2d6cfff6eb7c58`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 20:57:33 GMT
ADD file:29d0e44ebcc6f8dc2cfbc86c5034380677d263e9eec27a22ba045e0810836f81 in / 
# Tue, 12 Dec 2017 20:57:34 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 21:39:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 21:39:31 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 22:43:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:43:51 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:43:52 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:45:01 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 22:45:01 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:51e696f556166d0e25b3b27c824c4aafbddd5adcfd3f5186c09707f7baa3b312`  
		Last Modified: Tue, 12 Dec 2017 21:07:41 GMT  
		Size: 28.4 MB (28423526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e1f15069f149f59c18e22308fea3709837800f0d2954fbbc664799384ce6f`  
		Last Modified: Tue, 12 Dec 2017 22:45:35 GMT  
		Size: 2.6 MB (2608019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d5ced759aea47a18744948db8210418d363f4c785c37621006690d33a849d0`  
		Last Modified: Tue, 12 Dec 2017 22:45:43 GMT  
		Size: 26.1 MB (26127863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9-slim` - linux; arm variant v7

```console
$ docker pull pypy@sha256:99f5e7c41121ec0002d2b6d42a6c1a6a70752d3b4fe9a7489903466fc26a4794
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54978226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c84e3fcb1b4f28072773a645e9289b7d71f4f40e437045dbf21bcfb8fdbe57f`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:47 GMT
ADD file:1f5de474caa19da14d698a3f9c3d161abfa1e19e258a596d64f3dfc9e2f17686 in / 
# Tue, 12 Dec 2017 13:27:47 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 15:45:53 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 15:45:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:46:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:46:40 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 15:46:40 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 15:47:55 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 15:47:56 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:4b9c0f1a415433a98643bdda391dcf4fe5d9653fc3ed3845c7ac1be99eb43399`  
		Last Modified: Tue, 12 Dec 2017 13:39:52 GMT  
		Size: 26.3 MB (26282714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b37d60058a7d8edcada55701fe95ca118eff0b137ab3206001d6474c585038`  
		Last Modified: Tue, 12 Dec 2017 15:49:35 GMT  
		Size: 2.5 MB (2476158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93ad39ea9b5f53578215b6778f1e247029486b986e315e7f3df940b6942295a`  
		Last Modified: Tue, 12 Dec 2017 15:49:45 GMT  
		Size: 26.2 MB (26219354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5.9-slim` - linux; 386

```console
$ docker pull pypy@sha256:beb12510a29e6079a3e3ebfdbaaffc9855b40c4853111082582388e60bb703c9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60124197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2723d47c4e453dcbe9be3f47a500402f6d2ff3f4f35564870d48a636551f1481`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 14:21:05 GMT
ADD file:d31765999b40e32b628f3ec72b762f007f4918b08c507484e425adc990c87c26 in / 
# Tue, 12 Dec 2017 14:21:05 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 22:02:21 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 22:02:22 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 22:08:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:08:30 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:08:30 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:09:17 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 22:09:18 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:6b323e7c684c46ec9e577d3acb692c7e1c0c26ffbea6a4530dbe784a7eedf0f7`  
		Last Modified: Tue, 12 Dec 2017 14:49:35 GMT  
		Size: 30.3 MB (30266257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846baa5afdbb2caec4218e67e02a9b0793718ada3ec4d2a8c4d9ebe7c73c0713`  
		Last Modified: Tue, 12 Dec 2017 22:13:37 GMT  
		Size: 5.0 MB (4957755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e87231048cecb4fc4c3514e7c9e469c45e7eb6123e8ac4862540fd894f63612`  
		Last Modified: Tue, 12 Dec 2017 22:13:45 GMT  
		Size: 24.9 MB (24900185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:2-5-onbuild`

```console
$ docker pull pypy@sha256:58df33485c9d0a54a46525dcdfdf0f62d128d3cc9bd561697569e2a6236d2337
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `pypy:2-5-onbuild` - linux; amd64

```console
$ docker pull pypy@sha256:cbb4e4d19e76e0074d1defb33ee58833b953c1de0e342afb24a2263227e10320
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.7 MB (281745927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e51bd583a797c3bca6cb502f1a48b7ee142cd6af03033b5376d55201f9c0f32b`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:26:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 16:26:50 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:26:51 GMT
CMD ["pypy"]
# Tue, 12 Dec 2017 16:27:12 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 16:27:12 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 16:27:12 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 16:27:13 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 16:27:13 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b75493037494e7826da77e8b48bee4d15a7171acf45733e6ad9c22a32fea422`  
		Last Modified: Tue, 12 Dec 2017 16:28:25 GMT  
		Size: 24.8 MB (24771051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c1a97faf28f3e02142023746ac1899f3809d62878d41fccd35b16d6564ee7b`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.7 MB (3719646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c73e8333ea54a6ccd0af1dc19b3d01e43e9634a8efb6f7f4b92d27908b236a`  
		Last Modified: Tue, 12 Dec 2017 16:29:15 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5-onbuild` - linux; arm variant v5

```console
$ docker pull pypy@sha256:ead1ac231c6aca599292aae016ca59d0b44ecc96595d9207534181f286dfa8a5
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.3 MB (255292993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d4d9360eeb526d829828552047ac1dcfcf3f3ce683e8d99e9a421634975764`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 20:57:00 GMT
ADD file:2c2c6b8bfbbc9860c0ddd8a2ba3d769171576fc13d5d99fb50a852f6b03618d1 in / 
# Tue, 12 Dec 2017 20:57:00 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 22:52:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:52:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 22:54:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:56:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:52:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Dec 2017 00:52:55 GMT
ENV LANG=C.UTF-8
# Wed, 13 Dec 2017 00:53:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYPY_VERSION=5.9.0
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Wed, 13 Dec 2017 00:53:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Wed, 13 Dec 2017 00:54:00 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Wed, 13 Dec 2017 00:54:07 GMT
CMD ["pypy"]
# Wed, 13 Dec 2017 00:54:30 GMT
RUN mkdir -p /usr/src/app
# Wed, 13 Dec 2017 00:54:30 GMT
WORKDIR /usr/src/app
# Wed, 13 Dec 2017 00:54:30 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Wed, 13 Dec 2017 00:54:31 GMT
ONBUILD RUN pip install -r requirements.txt
# Wed, 13 Dec 2017 00:54:31 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:fbe67b6ec6f136174afee77eff07fd99e5764d9db2b13d0dc1189bf8203d289b`  
		Last Modified: Tue, 12 Dec 2017 21:06:47 GMT  
		Size: 50.9 MB (50882486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20452f83e704c3737bc38610443b6ca94edbe5388fb654b5c4c3c4308150785`  
		Last Modified: Tue, 12 Dec 2017 23:07:02 GMT  
		Size: 18.7 MB (18656894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b1e0d12986adcbf53895fa51052184e9f935a6424e8665bfad080be921ffec`  
		Last Modified: Tue, 12 Dec 2017 23:07:28 GMT  
		Size: 41.1 MB (41102373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3294d0e239416dcce73960614fcb72ab7e3034c5c0473cfc88120b49aaf8cf3`  
		Last Modified: Tue, 12 Dec 2017 23:08:09 GMT  
		Size: 115.7 MB (115740327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb10d9e21822b5858804af1906f60f0a667e581d0927089d9432869f10e7a5d9`  
		Last Modified: Wed, 13 Dec 2017 00:54:47 GMT  
		Size: 3.0 MB (3020433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc53514aa99843675aa2221aef86a6c1bce138eac6de239d2572e41717aff0b7`  
		Last Modified: Wed, 13 Dec 2017 00:54:55 GMT  
		Size: 22.2 MB (22170095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eea423ab6f26f0f128727c59477cda481f3e511e088be3cddaa4b548b3013b`  
		Last Modified: Wed, 13 Dec 2017 00:54:48 GMT  
		Size: 3.7 MB (3720220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f655a96258796da628a9bfe71df82779071ca0516242b076bc799eaeb165eb4`  
		Last Modified: Wed, 13 Dec 2017 00:55:34 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5-onbuild` - linux; arm variant v7

```console
$ docker pull pypy@sha256:8fb93eb68f4c911e321528719d69ddcc84af317771961d8c954f5d4be9f0dc6f
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249620597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac28a04335460f2d03c5a2298b30d71d8b90ab531e0943414e06b2cdf24a70bd`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:05 GMT
ADD file:aeb57f3a84dc1b93e1d38a80409a407df553344149d5070ed79b656865c90c54 in / 
# Tue, 12 Dec 2017 13:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:14:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:14:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 14:15:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:17:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 15:44:25 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:44:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 15:45:06 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 15:45:32 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 15:45:32 GMT
CMD ["pypy"]
# Tue, 12 Dec 2017 15:48:21 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 15:48:21 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 15:48:22 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 15:48:22 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 15:48:22 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:95e140a16c792899abc97cadee0138064dd21346fe51aa332ca4cbbd5563383c`  
		Last Modified: Tue, 12 Dec 2017 13:38:47 GMT  
		Size: 48.7 MB (48691755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237499cbbf2c5155fadc128c997700f0c5ec6355ba9704d0ec3f81c29640c9c4`  
		Last Modified: Tue, 12 Dec 2017 14:30:53 GMT  
		Size: 18.3 MB (18265038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f718f16c2f9a8213b99fcb49e72dad0036d1426f09c089f1e389b684f26520`  
		Last Modified: Tue, 12 Dec 2017 14:31:23 GMT  
		Size: 39.7 MB (39727713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affc0d5be2fb6b1dbb9d86ff0f533d88026215828cb4b1893257572ebf86f8d2`  
		Last Modified: Tue, 12 Dec 2017 14:32:10 GMT  
		Size: 114.1 MB (114057010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da492c2b2a6e64125a549432bf2b25c5d8fdb672fa3d27e1c9e5b6b493c28d4`  
		Last Modified: Tue, 12 Dec 2017 15:48:41 GMT  
		Size: 2.9 MB (2896866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1c900e416825525de3c49e77a9f71287afa1fa01ad6469e936a60f4e73bc30`  
		Last Modified: Tue, 12 Dec 2017 15:48:49 GMT  
		Size: 22.3 MB (22261764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e32dc2fb8080f66c1c6edb12faa4bf81f8660e27080c4eb0a8b61177203e308`  
		Last Modified: Tue, 12 Dec 2017 15:48:42 GMT  
		Size: 3.7 MB (3720288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6de7019ddc357de708f6542fac5dbb2a00898b592f55581d094d2958c1a72e8`  
		Last Modified: Tue, 12 Dec 2017 15:50:30 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5-onbuild` - linux; 386

```console
$ docker pull pypy@sha256:abce1ce483117a2aa8e27648543aedf0532fee84205bd6babbbf8a1fe3c40b64
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281366071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:765310362b69c1fd19344acbe069dc44a5615499f0f61b909d5a50921669446d`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 14:19:55 GMT
ADD file:235a40e05b677eb2ae7e7a3cc5cbb0cda242ff15dddb87cb8dc9bb0cd2d6aed8 in / 
# Tue, 12 Dec 2017 14:19:55 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 16:53:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:53:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 16:54:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:56:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 21:56:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 21:56:55 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 21:57:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:03:46 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 22:03:56 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 22:03:56 GMT
CMD ["pypy"]
# Tue, 12 Dec 2017 22:09:39 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 22:09:39 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 22:09:39 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 22:09:39 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 22:09:40 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:d99577c7ee3d4d82987bedaeb10f3244ff7e19e41c5259bb8cac00568d1c4271`  
		Last Modified: Tue, 12 Dec 2017 14:46:26 GMT  
		Size: 52.8 MB (52777369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94aafa6d6f35f82e1fdc93cd4f7f6ab829f6297c8defaaa911dfb2de063bf3d`  
		Last Modified: Tue, 12 Dec 2017 17:27:39 GMT  
		Size: 21.6 MB (21596374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd19391b0ebd36e15e21cb3a6728c5950937634b9c81ecc7e3d1422b1dc25eb`  
		Last Modified: Tue, 12 Dec 2017 17:28:18 GMT  
		Size: 43.9 MB (43918299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8333879ca1894c745f67c724a7e4ad35542f5966a47bb050928910a944130ea0`  
		Last Modified: Tue, 12 Dec 2017 17:29:10 GMT  
		Size: 135.1 MB (135144789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5718f0e07ebd0ba7b1a182304b0f07394be9021b2ebad934f2a0b913390619cc`  
		Last Modified: Tue, 12 Dec 2017 22:10:00 GMT  
		Size: 3.3 MB (3271878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6c0ee3ad02226742c48a9260127e316949ec9b18e8e28c47f14bb1362fc38`  
		Last Modified: Tue, 12 Dec 2017 22:10:07 GMT  
		Size: 20.9 MB (20937530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aafba35b4500cd3009de7d3936f41dfcf9c23f56f743eb34541b0e9e82f67e`  
		Last Modified: Tue, 12 Dec 2017 22:09:59 GMT  
		Size: 3.7 MB (3719700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5023694a0d55bd510c6e9cf8ff7f7e924f82f23f8dc2d62eddf991b36d275e1`  
		Last Modified: Tue, 12 Dec 2017 22:14:40 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:2-5-slim`

```console
$ docker pull pypy@sha256:f6273e4a29678a968239b91ce0c130404fa73146bfc26fa9d5b9b06edc259cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `pypy:2-5-slim` - linux; amd64

```console
$ docker pull pypy@sha256:c08046309aa3c069d4271a6b528ca89bc1b81354b8f8d60ae2b966c5063edd51
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61704534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9499c15fb67f97f95a978ce2b597b22b20b437873c82bafbe62cae4b4ce894`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 06:21:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 06:21:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 06:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 06:22:17 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 06:26:44 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ed6d99248693c2acd5109ff75533464052952167eca48dbf989268a392ebb3`  
		Last Modified: Tue, 12 Dec 2017 06:28:04 GMT  
		Size: 2.9 MB (2859578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23aa754ac2ff99b4b15fd8d3a949cbcab6921a922c40364c70d4a50f86f0094`  
		Last Modified: Tue, 12 Dec 2017 06:28:13 GMT  
		Size: 28.7 MB (28730437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5-slim` - linux; arm variant v5

```console
$ docker pull pypy@sha256:8eca5d74aa8367146860be6ebc278d243c949b309c469e5643c691a10e3aac61
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57159408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9bbc15f5cbca846158f77e88492d3f89ec922df0734b6345e2d6cfff6eb7c58`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 20:57:33 GMT
ADD file:29d0e44ebcc6f8dc2cfbc86c5034380677d263e9eec27a22ba045e0810836f81 in / 
# Tue, 12 Dec 2017 20:57:34 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 21:39:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 21:39:31 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 22:43:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:43:51 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:43:52 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:45:01 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 22:45:01 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:51e696f556166d0e25b3b27c824c4aafbddd5adcfd3f5186c09707f7baa3b312`  
		Last Modified: Tue, 12 Dec 2017 21:07:41 GMT  
		Size: 28.4 MB (28423526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e1f15069f149f59c18e22308fea3709837800f0d2954fbbc664799384ce6f`  
		Last Modified: Tue, 12 Dec 2017 22:45:35 GMT  
		Size: 2.6 MB (2608019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d5ced759aea47a18744948db8210418d363f4c785c37621006690d33a849d0`  
		Last Modified: Tue, 12 Dec 2017 22:45:43 GMT  
		Size: 26.1 MB (26127863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5-slim` - linux; arm variant v7

```console
$ docker pull pypy@sha256:99f5e7c41121ec0002d2b6d42a6c1a6a70752d3b4fe9a7489903466fc26a4794
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54978226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c84e3fcb1b4f28072773a645e9289b7d71f4f40e437045dbf21bcfb8fdbe57f`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:47 GMT
ADD file:1f5de474caa19da14d698a3f9c3d161abfa1e19e258a596d64f3dfc9e2f17686 in / 
# Tue, 12 Dec 2017 13:27:47 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 15:45:53 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 15:45:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:46:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:46:40 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 15:46:40 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 15:47:55 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 15:47:56 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:4b9c0f1a415433a98643bdda391dcf4fe5d9653fc3ed3845c7ac1be99eb43399`  
		Last Modified: Tue, 12 Dec 2017 13:39:52 GMT  
		Size: 26.3 MB (26282714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b37d60058a7d8edcada55701fe95ca118eff0b137ab3206001d6474c585038`  
		Last Modified: Tue, 12 Dec 2017 15:49:35 GMT  
		Size: 2.5 MB (2476158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93ad39ea9b5f53578215b6778f1e247029486b986e315e7f3df940b6942295a`  
		Last Modified: Tue, 12 Dec 2017 15:49:45 GMT  
		Size: 26.2 MB (26219354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-5-slim` - linux; 386

```console
$ docker pull pypy@sha256:beb12510a29e6079a3e3ebfdbaaffc9855b40c4853111082582388e60bb703c9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60124197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2723d47c4e453dcbe9be3f47a500402f6d2ff3f4f35564870d48a636551f1481`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 14:21:05 GMT
ADD file:d31765999b40e32b628f3ec72b762f007f4918b08c507484e425adc990c87c26 in / 
# Tue, 12 Dec 2017 14:21:05 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 22:02:21 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 22:02:22 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 22:08:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:08:30 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:08:30 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:09:17 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 22:09:18 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:6b323e7c684c46ec9e577d3acb692c7e1c0c26ffbea6a4530dbe784a7eedf0f7`  
		Last Modified: Tue, 12 Dec 2017 14:49:35 GMT  
		Size: 30.3 MB (30266257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846baa5afdbb2caec4218e67e02a9b0793718ada3ec4d2a8c4d9ebe7c73c0713`  
		Last Modified: Tue, 12 Dec 2017 22:13:37 GMT  
		Size: 5.0 MB (4957755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e87231048cecb4fc4c3514e7c9e469c45e7eb6123e8ac4862540fd894f63612`  
		Last Modified: Tue, 12 Dec 2017 22:13:45 GMT  
		Size: 24.9 MB (24900185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:2-onbuild`

```console
$ docker pull pypy@sha256:58df33485c9d0a54a46525dcdfdf0f62d128d3cc9bd561697569e2a6236d2337
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `pypy:2-onbuild` - linux; amd64

```console
$ docker pull pypy@sha256:cbb4e4d19e76e0074d1defb33ee58833b953c1de0e342afb24a2263227e10320
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.7 MB (281745927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e51bd583a797c3bca6cb502f1a48b7ee142cd6af03033b5376d55201f9c0f32b`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:26:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 16:26:50 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:26:51 GMT
CMD ["pypy"]
# Tue, 12 Dec 2017 16:27:12 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 16:27:12 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 16:27:12 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 16:27:13 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 16:27:13 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b75493037494e7826da77e8b48bee4d15a7171acf45733e6ad9c22a32fea422`  
		Last Modified: Tue, 12 Dec 2017 16:28:25 GMT  
		Size: 24.8 MB (24771051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c1a97faf28f3e02142023746ac1899f3809d62878d41fccd35b16d6564ee7b`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.7 MB (3719646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c73e8333ea54a6ccd0af1dc19b3d01e43e9634a8efb6f7f4b92d27908b236a`  
		Last Modified: Tue, 12 Dec 2017 16:29:15 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-onbuild` - linux; arm variant v5

```console
$ docker pull pypy@sha256:ead1ac231c6aca599292aae016ca59d0b44ecc96595d9207534181f286dfa8a5
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.3 MB (255292993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d4d9360eeb526d829828552047ac1dcfcf3f3ce683e8d99e9a421634975764`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 20:57:00 GMT
ADD file:2c2c6b8bfbbc9860c0ddd8a2ba3d769171576fc13d5d99fb50a852f6b03618d1 in / 
# Tue, 12 Dec 2017 20:57:00 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 22:52:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:52:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 22:54:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:56:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:52:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Dec 2017 00:52:55 GMT
ENV LANG=C.UTF-8
# Wed, 13 Dec 2017 00:53:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYPY_VERSION=5.9.0
# Wed, 13 Dec 2017 00:53:28 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Wed, 13 Dec 2017 00:53:37 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Wed, 13 Dec 2017 00:54:00 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Wed, 13 Dec 2017 00:54:07 GMT
CMD ["pypy"]
# Wed, 13 Dec 2017 00:54:30 GMT
RUN mkdir -p /usr/src/app
# Wed, 13 Dec 2017 00:54:30 GMT
WORKDIR /usr/src/app
# Wed, 13 Dec 2017 00:54:30 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Wed, 13 Dec 2017 00:54:31 GMT
ONBUILD RUN pip install -r requirements.txt
# Wed, 13 Dec 2017 00:54:31 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:fbe67b6ec6f136174afee77eff07fd99e5764d9db2b13d0dc1189bf8203d289b`  
		Last Modified: Tue, 12 Dec 2017 21:06:47 GMT  
		Size: 50.9 MB (50882486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20452f83e704c3737bc38610443b6ca94edbe5388fb654b5c4c3c4308150785`  
		Last Modified: Tue, 12 Dec 2017 23:07:02 GMT  
		Size: 18.7 MB (18656894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b1e0d12986adcbf53895fa51052184e9f935a6424e8665bfad080be921ffec`  
		Last Modified: Tue, 12 Dec 2017 23:07:28 GMT  
		Size: 41.1 MB (41102373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3294d0e239416dcce73960614fcb72ab7e3034c5c0473cfc88120b49aaf8cf3`  
		Last Modified: Tue, 12 Dec 2017 23:08:09 GMT  
		Size: 115.7 MB (115740327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb10d9e21822b5858804af1906f60f0a667e581d0927089d9432869f10e7a5d9`  
		Last Modified: Wed, 13 Dec 2017 00:54:47 GMT  
		Size: 3.0 MB (3020433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc53514aa99843675aa2221aef86a6c1bce138eac6de239d2572e41717aff0b7`  
		Last Modified: Wed, 13 Dec 2017 00:54:55 GMT  
		Size: 22.2 MB (22170095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eea423ab6f26f0f128727c59477cda481f3e511e088be3cddaa4b548b3013b`  
		Last Modified: Wed, 13 Dec 2017 00:54:48 GMT  
		Size: 3.7 MB (3720220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f655a96258796da628a9bfe71df82779071ca0516242b076bc799eaeb165eb4`  
		Last Modified: Wed, 13 Dec 2017 00:55:34 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-onbuild` - linux; arm variant v7

```console
$ docker pull pypy@sha256:8fb93eb68f4c911e321528719d69ddcc84af317771961d8c954f5d4be9f0dc6f
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249620597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac28a04335460f2d03c5a2298b30d71d8b90ab531e0943414e06b2cdf24a70bd`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:05 GMT
ADD file:aeb57f3a84dc1b93e1d38a80409a407df553344149d5070ed79b656865c90c54 in / 
# Tue, 12 Dec 2017 13:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:14:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:14:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 14:15:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:17:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 15:44:25 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:44:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 15:44:58 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 15:45:06 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 15:45:32 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 15:45:32 GMT
CMD ["pypy"]
# Tue, 12 Dec 2017 15:48:21 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 15:48:21 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 15:48:22 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 15:48:22 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 15:48:22 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:95e140a16c792899abc97cadee0138064dd21346fe51aa332ca4cbbd5563383c`  
		Last Modified: Tue, 12 Dec 2017 13:38:47 GMT  
		Size: 48.7 MB (48691755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237499cbbf2c5155fadc128c997700f0c5ec6355ba9704d0ec3f81c29640c9c4`  
		Last Modified: Tue, 12 Dec 2017 14:30:53 GMT  
		Size: 18.3 MB (18265038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f718f16c2f9a8213b99fcb49e72dad0036d1426f09c089f1e389b684f26520`  
		Last Modified: Tue, 12 Dec 2017 14:31:23 GMT  
		Size: 39.7 MB (39727713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affc0d5be2fb6b1dbb9d86ff0f533d88026215828cb4b1893257572ebf86f8d2`  
		Last Modified: Tue, 12 Dec 2017 14:32:10 GMT  
		Size: 114.1 MB (114057010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da492c2b2a6e64125a549432bf2b25c5d8fdb672fa3d27e1c9e5b6b493c28d4`  
		Last Modified: Tue, 12 Dec 2017 15:48:41 GMT  
		Size: 2.9 MB (2896866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1c900e416825525de3c49e77a9f71287afa1fa01ad6469e936a60f4e73bc30`  
		Last Modified: Tue, 12 Dec 2017 15:48:49 GMT  
		Size: 22.3 MB (22261764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e32dc2fb8080f66c1c6edb12faa4bf81f8660e27080c4eb0a8b61177203e308`  
		Last Modified: Tue, 12 Dec 2017 15:48:42 GMT  
		Size: 3.7 MB (3720288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6de7019ddc357de708f6542fac5dbb2a00898b592f55581d094d2958c1a72e8`  
		Last Modified: Tue, 12 Dec 2017 15:50:30 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-onbuild` - linux; 386

```console
$ docker pull pypy@sha256:abce1ce483117a2aa8e27648543aedf0532fee84205bd6babbbf8a1fe3c40b64
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281366071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:765310362b69c1fd19344acbe069dc44a5615499f0f61b909d5a50921669446d`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 14:19:55 GMT
ADD file:235a40e05b677eb2ae7e7a3cc5cbb0cda242ff15dddb87cb8dc9bb0cd2d6aed8 in / 
# Tue, 12 Dec 2017 14:19:55 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 16:53:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:53:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 16:54:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:56:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 21:56:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 21:56:55 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 21:57:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:03:35 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:03:46 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version
# Tue, 12 Dec 2017 22:03:56 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 22:03:56 GMT
CMD ["pypy"]
# Tue, 12 Dec 2017 22:09:39 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 22:09:39 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 22:09:39 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 22:09:39 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 22:09:40 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:d99577c7ee3d4d82987bedaeb10f3244ff7e19e41c5259bb8cac00568d1c4271`  
		Last Modified: Tue, 12 Dec 2017 14:46:26 GMT  
		Size: 52.8 MB (52777369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94aafa6d6f35f82e1fdc93cd4f7f6ab829f6297c8defaaa911dfb2de063bf3d`  
		Last Modified: Tue, 12 Dec 2017 17:27:39 GMT  
		Size: 21.6 MB (21596374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd19391b0ebd36e15e21cb3a6728c5950937634b9c81ecc7e3d1422b1dc25eb`  
		Last Modified: Tue, 12 Dec 2017 17:28:18 GMT  
		Size: 43.9 MB (43918299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8333879ca1894c745f67c724a7e4ad35542f5966a47bb050928910a944130ea0`  
		Last Modified: Tue, 12 Dec 2017 17:29:10 GMT  
		Size: 135.1 MB (135144789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5718f0e07ebd0ba7b1a182304b0f07394be9021b2ebad934f2a0b913390619cc`  
		Last Modified: Tue, 12 Dec 2017 22:10:00 GMT  
		Size: 3.3 MB (3271878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6c0ee3ad02226742c48a9260127e316949ec9b18e8e28c47f14bb1362fc38`  
		Last Modified: Tue, 12 Dec 2017 22:10:07 GMT  
		Size: 20.9 MB (20937530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aafba35b4500cd3009de7d3936f41dfcf9c23f56f743eb34541b0e9e82f67e`  
		Last Modified: Tue, 12 Dec 2017 22:09:59 GMT  
		Size: 3.7 MB (3719700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5023694a0d55bd510c6e9cf8ff7f7e924f82f23f8dc2d62eddf991b36d275e1`  
		Last Modified: Tue, 12 Dec 2017 22:14:40 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:2-slim`

```console
$ docker pull pypy@sha256:f6273e4a29678a968239b91ce0c130404fa73146bfc26fa9d5b9b06edc259cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `pypy:2-slim` - linux; amd64

```console
$ docker pull pypy@sha256:c08046309aa3c069d4271a6b528ca89bc1b81354b8f8d60ae2b966c5063edd51
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61704534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9499c15fb67f97f95a978ce2b597b22b20b437873c82bafbe62cae4b4ce894`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 06:21:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 06:21:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 06:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 06:22:17 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 06:26:44 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ed6d99248693c2acd5109ff75533464052952167eca48dbf989268a392ebb3`  
		Last Modified: Tue, 12 Dec 2017 06:28:04 GMT  
		Size: 2.9 MB (2859578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23aa754ac2ff99b4b15fd8d3a949cbcab6921a922c40364c70d4a50f86f0094`  
		Last Modified: Tue, 12 Dec 2017 06:28:13 GMT  
		Size: 28.7 MB (28730437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-slim` - linux; arm variant v5

```console
$ docker pull pypy@sha256:8eca5d74aa8367146860be6ebc278d243c949b309c469e5643c691a10e3aac61
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57159408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9bbc15f5cbca846158f77e88492d3f89ec922df0734b6345e2d6cfff6eb7c58`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 20:57:33 GMT
ADD file:29d0e44ebcc6f8dc2cfbc86c5034380677d263e9eec27a22ba045e0810836f81 in / 
# Tue, 12 Dec 2017 20:57:34 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 21:39:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 21:39:31 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 22:43:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:43:51 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:43:52 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:45:01 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 22:45:01 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:51e696f556166d0e25b3b27c824c4aafbddd5adcfd3f5186c09707f7baa3b312`  
		Last Modified: Tue, 12 Dec 2017 21:07:41 GMT  
		Size: 28.4 MB (28423526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e1f15069f149f59c18e22308fea3709837800f0d2954fbbc664799384ce6f`  
		Last Modified: Tue, 12 Dec 2017 22:45:35 GMT  
		Size: 2.6 MB (2608019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d5ced759aea47a18744948db8210418d363f4c785c37621006690d33a849d0`  
		Last Modified: Tue, 12 Dec 2017 22:45:43 GMT  
		Size: 26.1 MB (26127863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-slim` - linux; arm variant v7

```console
$ docker pull pypy@sha256:99f5e7c41121ec0002d2b6d42a6c1a6a70752d3b4fe9a7489903466fc26a4794
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54978226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c84e3fcb1b4f28072773a645e9289b7d71f4f40e437045dbf21bcfb8fdbe57f`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 13:27:47 GMT
ADD file:1f5de474caa19da14d698a3f9c3d161abfa1e19e258a596d64f3dfc9e2f17686 in / 
# Tue, 12 Dec 2017 13:27:47 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 15:45:53 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 15:45:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:46:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:46:40 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 15:46:40 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 15:47:55 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 15:47:56 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:4b9c0f1a415433a98643bdda391dcf4fe5d9653fc3ed3845c7ac1be99eb43399`  
		Last Modified: Tue, 12 Dec 2017 13:39:52 GMT  
		Size: 26.3 MB (26282714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b37d60058a7d8edcada55701fe95ca118eff0b137ab3206001d6474c585038`  
		Last Modified: Tue, 12 Dec 2017 15:49:35 GMT  
		Size: 2.5 MB (2476158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93ad39ea9b5f53578215b6778f1e247029486b986e315e7f3df940b6942295a`  
		Last Modified: Tue, 12 Dec 2017 15:49:45 GMT  
		Size: 26.2 MB (26219354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-slim` - linux; 386

```console
$ docker pull pypy@sha256:beb12510a29e6079a3e3ebfdbaaffc9855b40c4853111082582388e60bb703c9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60124197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2723d47c4e453dcbe9be3f47a500402f6d2ff3f4f35564870d48a636551f1481`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 12 Dec 2017 14:21:05 GMT
ADD file:d31765999b40e32b628f3ec72b762f007f4918b08c507484e425adc990c87c26 in / 
# Tue, 12 Dec 2017 14:21:05 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 22:02:21 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 22:02:22 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 22:08:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:08:30 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 22:08:30 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 22:09:17 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='790febd4f09e22d6e2f81154efc7dc4b2feec72712aaf4f82aa91b550abb4b48' ;; 		armel) pypyArch='linux-armel'; sha256='ac0676d91dfb388c799ec5c2845f42018a666423376f52f3ae13d61fd2e6f87d' ;; 		armhf) pypyArch='linux-armhf-raring'; sha256='2597b7b21acdef4f2b81074a594157c9450363c74a17f005548c6b102f93cff4' ;; 		i386) pypyArch='linux32'; sha256='a2431a9e4ef879da1a2b56b111013b4a6efb87d4173a37bf650de47834ac5fe4' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy2-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 22:09:18 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:6b323e7c684c46ec9e577d3acb692c7e1c0c26ffbea6a4530dbe784a7eedf0f7`  
		Last Modified: Tue, 12 Dec 2017 14:49:35 GMT  
		Size: 30.3 MB (30266257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846baa5afdbb2caec4218e67e02a9b0793718ada3ec4d2a8c4d9ebe7c73c0713`  
		Last Modified: Tue, 12 Dec 2017 22:13:37 GMT  
		Size: 5.0 MB (4957755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e87231048cecb4fc4c3514e7c9e469c45e7eb6123e8ac4862540fd894f63612`  
		Last Modified: Tue, 12 Dec 2017 22:13:45 GMT  
		Size: 24.9 MB (24900185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:3`

```console
$ docker pull pypy@sha256:c278aadae4fbde2d150923b237011a0e9f3d52a41a47d42a7e77f7a6c45d9472
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:3` - linux; amd64

```console
$ docker pull pypy@sha256:ef2a768bd444e0db71a15c0a8fd2f1a9a469532c8144c9245dee9045f894b883
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.7 MB (282733829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e768a7f911361723ddc64022402067d960b3340282ecefb86e91efba0f6b98`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:27:39 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version
# Tue, 12 Dec 2017 16:27:52 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:27:52 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e9b028e52f19d4499fef7b5124e78a03adac776f518eae325ed99cb3ce5fb3`  
		Last Modified: Tue, 12 Dec 2017 16:30:14 GMT  
		Size: 25.3 MB (25305144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee65405971a25347ac7d2f8d967e946a192e4a4a6fbc4df5d336f10b99c6a6cd`  
		Last Modified: Tue, 12 Dec 2017 16:30:08 GMT  
		Size: 4.2 MB (4173587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:3-5`

```console
$ docker pull pypy@sha256:c278aadae4fbde2d150923b237011a0e9f3d52a41a47d42a7e77f7a6c45d9472
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:3-5` - linux; amd64

```console
$ docker pull pypy@sha256:ef2a768bd444e0db71a15c0a8fd2f1a9a469532c8144c9245dee9045f894b883
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.7 MB (282733829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e768a7f911361723ddc64022402067d960b3340282ecefb86e91efba0f6b98`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:27:39 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version
# Tue, 12 Dec 2017 16:27:52 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:27:52 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e9b028e52f19d4499fef7b5124e78a03adac776f518eae325ed99cb3ce5fb3`  
		Last Modified: Tue, 12 Dec 2017 16:30:14 GMT  
		Size: 25.3 MB (25305144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee65405971a25347ac7d2f8d967e946a192e4a4a6fbc4df5d336f10b99c6a6cd`  
		Last Modified: Tue, 12 Dec 2017 16:30:08 GMT  
		Size: 4.2 MB (4173587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:3-5.9`

```console
$ docker pull pypy@sha256:c278aadae4fbde2d150923b237011a0e9f3d52a41a47d42a7e77f7a6c45d9472
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:3-5.9` - linux; amd64

```console
$ docker pull pypy@sha256:ef2a768bd444e0db71a15c0a8fd2f1a9a469532c8144c9245dee9045f894b883
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.7 MB (282733829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e768a7f911361723ddc64022402067d960b3340282ecefb86e91efba0f6b98`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:27:39 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version
# Tue, 12 Dec 2017 16:27:52 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:27:52 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e9b028e52f19d4499fef7b5124e78a03adac776f518eae325ed99cb3ce5fb3`  
		Last Modified: Tue, 12 Dec 2017 16:30:14 GMT  
		Size: 25.3 MB (25305144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee65405971a25347ac7d2f8d967e946a192e4a4a6fbc4df5d336f10b99c6a6cd`  
		Last Modified: Tue, 12 Dec 2017 16:30:08 GMT  
		Size: 4.2 MB (4173587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:3-5.9.0`

```console
$ docker pull pypy@sha256:c278aadae4fbde2d150923b237011a0e9f3d52a41a47d42a7e77f7a6c45d9472
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:3-5.9.0` - linux; amd64

```console
$ docker pull pypy@sha256:ef2a768bd444e0db71a15c0a8fd2f1a9a469532c8144c9245dee9045f894b883
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.7 MB (282733829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e768a7f911361723ddc64022402067d960b3340282ecefb86e91efba0f6b98`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:27:39 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version
# Tue, 12 Dec 2017 16:27:52 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:27:52 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e9b028e52f19d4499fef7b5124e78a03adac776f518eae325ed99cb3ce5fb3`  
		Last Modified: Tue, 12 Dec 2017 16:30:14 GMT  
		Size: 25.3 MB (25305144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee65405971a25347ac7d2f8d967e946a192e4a4a6fbc4df5d336f10b99c6a6cd`  
		Last Modified: Tue, 12 Dec 2017 16:30:08 GMT  
		Size: 4.2 MB (4173587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:3-5.9.0-onbuild`

```console
$ docker pull pypy@sha256:a675ac6d32d30f00298115e7a428f1f1069e5577fddcadb8493e3256fa37b947
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:3-5.9.0-onbuild` - linux; amd64

```console
$ docker pull pypy@sha256:a5f78b6cde0e81f6dffe84eb0a24db0d95234942c0a9265a01e484c8889a29d4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.7 MB (282733961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f559a3ba3832c1eb8cf7db289e5d456e84ef32e4c830a6ae71dfe02b8c0edff`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:27:39 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version
# Tue, 12 Dec 2017 16:27:52 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:27:52 GMT
CMD ["pypy3"]
# Tue, 12 Dec 2017 16:28:02 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 16:28:02 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 16:28:02 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 16:28:02 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 16:28:03 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e9b028e52f19d4499fef7b5124e78a03adac776f518eae325ed99cb3ce5fb3`  
		Last Modified: Tue, 12 Dec 2017 16:30:14 GMT  
		Size: 25.3 MB (25305144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee65405971a25347ac7d2f8d967e946a192e4a4a6fbc4df5d336f10b99c6a6cd`  
		Last Modified: Tue, 12 Dec 2017 16:30:08 GMT  
		Size: 4.2 MB (4173587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89b61d544df4f7f9e32ace5502607095efdb9b0ed3c9cf924e547d4b9f762eb`  
		Last Modified: Tue, 12 Dec 2017 16:31:26 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:3-5.9.0-slim`

```console
$ docker pull pypy@sha256:8e1a64f28581c0ab1e9cf8e54c52644ec3ebb68c6ee8663c74e491dd66ab6db7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:3-5.9.0-slim` - linux; amd64

```console
$ docker pull pypy@sha256:e296f17128e5a549a71dcea9f6a7fd3abedcf9203bbdc3d3073ed9c971cb9c36
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62751328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebdc0f0f45622fe90ead8acf85e77fb7f1ac6aaf5db8c083736347d3aec4dd8f`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 06:21:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 06:21:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 06:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 06:27:38 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 06:27:38 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ed6d99248693c2acd5109ff75533464052952167eca48dbf989268a392ebb3`  
		Last Modified: Tue, 12 Dec 2017 06:28:04 GMT  
		Size: 2.9 MB (2859578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af11562222d940dc258b1b84b125ce27dc650550602b677b1f49b73a1b490e53`  
		Last Modified: Tue, 12 Dec 2017 06:29:20 GMT  
		Size: 29.8 MB (29777231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:3-5.9-onbuild`

```console
$ docker pull pypy@sha256:a675ac6d32d30f00298115e7a428f1f1069e5577fddcadb8493e3256fa37b947
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:3-5.9-onbuild` - linux; amd64

```console
$ docker pull pypy@sha256:a5f78b6cde0e81f6dffe84eb0a24db0d95234942c0a9265a01e484c8889a29d4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.7 MB (282733961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f559a3ba3832c1eb8cf7db289e5d456e84ef32e4c830a6ae71dfe02b8c0edff`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:27:39 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version
# Tue, 12 Dec 2017 16:27:52 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:27:52 GMT
CMD ["pypy3"]
# Tue, 12 Dec 2017 16:28:02 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 16:28:02 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 16:28:02 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 16:28:02 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 16:28:03 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e9b028e52f19d4499fef7b5124e78a03adac776f518eae325ed99cb3ce5fb3`  
		Last Modified: Tue, 12 Dec 2017 16:30:14 GMT  
		Size: 25.3 MB (25305144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee65405971a25347ac7d2f8d967e946a192e4a4a6fbc4df5d336f10b99c6a6cd`  
		Last Modified: Tue, 12 Dec 2017 16:30:08 GMT  
		Size: 4.2 MB (4173587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89b61d544df4f7f9e32ace5502607095efdb9b0ed3c9cf924e547d4b9f762eb`  
		Last Modified: Tue, 12 Dec 2017 16:31:26 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:3-5.9-slim`

```console
$ docker pull pypy@sha256:8e1a64f28581c0ab1e9cf8e54c52644ec3ebb68c6ee8663c74e491dd66ab6db7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:3-5.9-slim` - linux; amd64

```console
$ docker pull pypy@sha256:e296f17128e5a549a71dcea9f6a7fd3abedcf9203bbdc3d3073ed9c971cb9c36
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62751328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebdc0f0f45622fe90ead8acf85e77fb7f1ac6aaf5db8c083736347d3aec4dd8f`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 06:21:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 06:21:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 06:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 06:27:38 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 06:27:38 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ed6d99248693c2acd5109ff75533464052952167eca48dbf989268a392ebb3`  
		Last Modified: Tue, 12 Dec 2017 06:28:04 GMT  
		Size: 2.9 MB (2859578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af11562222d940dc258b1b84b125ce27dc650550602b677b1f49b73a1b490e53`  
		Last Modified: Tue, 12 Dec 2017 06:29:20 GMT  
		Size: 29.8 MB (29777231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:3-5-onbuild`

```console
$ docker pull pypy@sha256:a675ac6d32d30f00298115e7a428f1f1069e5577fddcadb8493e3256fa37b947
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:3-5-onbuild` - linux; amd64

```console
$ docker pull pypy@sha256:a5f78b6cde0e81f6dffe84eb0a24db0d95234942c0a9265a01e484c8889a29d4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.7 MB (282733961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f559a3ba3832c1eb8cf7db289e5d456e84ef32e4c830a6ae71dfe02b8c0edff`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:27:39 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version
# Tue, 12 Dec 2017 16:27:52 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:27:52 GMT
CMD ["pypy3"]
# Tue, 12 Dec 2017 16:28:02 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 16:28:02 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 16:28:02 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 16:28:02 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 16:28:03 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e9b028e52f19d4499fef7b5124e78a03adac776f518eae325ed99cb3ce5fb3`  
		Last Modified: Tue, 12 Dec 2017 16:30:14 GMT  
		Size: 25.3 MB (25305144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee65405971a25347ac7d2f8d967e946a192e4a4a6fbc4df5d336f10b99c6a6cd`  
		Last Modified: Tue, 12 Dec 2017 16:30:08 GMT  
		Size: 4.2 MB (4173587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89b61d544df4f7f9e32ace5502607095efdb9b0ed3c9cf924e547d4b9f762eb`  
		Last Modified: Tue, 12 Dec 2017 16:31:26 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:3-5-slim`

```console
$ docker pull pypy@sha256:8e1a64f28581c0ab1e9cf8e54c52644ec3ebb68c6ee8663c74e491dd66ab6db7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:3-5-slim` - linux; amd64

```console
$ docker pull pypy@sha256:e296f17128e5a549a71dcea9f6a7fd3abedcf9203bbdc3d3073ed9c971cb9c36
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62751328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebdc0f0f45622fe90ead8acf85e77fb7f1ac6aaf5db8c083736347d3aec4dd8f`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 06:21:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 06:21:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 06:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 06:27:38 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 06:27:38 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ed6d99248693c2acd5109ff75533464052952167eca48dbf989268a392ebb3`  
		Last Modified: Tue, 12 Dec 2017 06:28:04 GMT  
		Size: 2.9 MB (2859578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af11562222d940dc258b1b84b125ce27dc650550602b677b1f49b73a1b490e53`  
		Last Modified: Tue, 12 Dec 2017 06:29:20 GMT  
		Size: 29.8 MB (29777231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:3-onbuild`

```console
$ docker pull pypy@sha256:a675ac6d32d30f00298115e7a428f1f1069e5577fddcadb8493e3256fa37b947
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:3-onbuild` - linux; amd64

```console
$ docker pull pypy@sha256:a5f78b6cde0e81f6dffe84eb0a24db0d95234942c0a9265a01e484c8889a29d4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.7 MB (282733961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f559a3ba3832c1eb8cf7db289e5d456e84ef32e4c830a6ae71dfe02b8c0edff`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:27:39 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version
# Tue, 12 Dec 2017 16:27:52 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:27:52 GMT
CMD ["pypy3"]
# Tue, 12 Dec 2017 16:28:02 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 16:28:02 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 16:28:02 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 16:28:02 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 16:28:03 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e9b028e52f19d4499fef7b5124e78a03adac776f518eae325ed99cb3ce5fb3`  
		Last Modified: Tue, 12 Dec 2017 16:30:14 GMT  
		Size: 25.3 MB (25305144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee65405971a25347ac7d2f8d967e946a192e4a4a6fbc4df5d336f10b99c6a6cd`  
		Last Modified: Tue, 12 Dec 2017 16:30:08 GMT  
		Size: 4.2 MB (4173587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89b61d544df4f7f9e32ace5502607095efdb9b0ed3c9cf924e547d4b9f762eb`  
		Last Modified: Tue, 12 Dec 2017 16:31:26 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:3-slim`

```console
$ docker pull pypy@sha256:8e1a64f28581c0ab1e9cf8e54c52644ec3ebb68c6ee8663c74e491dd66ab6db7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:3-slim` - linux; amd64

```console
$ docker pull pypy@sha256:e296f17128e5a549a71dcea9f6a7fd3abedcf9203bbdc3d3073ed9c971cb9c36
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62751328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebdc0f0f45622fe90ead8acf85e77fb7f1ac6aaf5db8c083736347d3aec4dd8f`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 06:21:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 06:21:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 06:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 06:27:38 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 06:27:38 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ed6d99248693c2acd5109ff75533464052952167eca48dbf989268a392ebb3`  
		Last Modified: Tue, 12 Dec 2017 06:28:04 GMT  
		Size: 2.9 MB (2859578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af11562222d940dc258b1b84b125ce27dc650550602b677b1f49b73a1b490e53`  
		Last Modified: Tue, 12 Dec 2017 06:29:20 GMT  
		Size: 29.8 MB (29777231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:latest`

```console
$ docker pull pypy@sha256:c278aadae4fbde2d150923b237011a0e9f3d52a41a47d42a7e77f7a6c45d9472
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:latest` - linux; amd64

```console
$ docker pull pypy@sha256:ef2a768bd444e0db71a15c0a8fd2f1a9a469532c8144c9245dee9045f894b883
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.7 MB (282733829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e768a7f911361723ddc64022402067d960b3340282ecefb86e91efba0f6b98`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:27:39 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version
# Tue, 12 Dec 2017 16:27:52 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:27:52 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e9b028e52f19d4499fef7b5124e78a03adac776f518eae325ed99cb3ce5fb3`  
		Last Modified: Tue, 12 Dec 2017 16:30:14 GMT  
		Size: 25.3 MB (25305144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee65405971a25347ac7d2f8d967e946a192e4a4a6fbc4df5d336f10b99c6a6cd`  
		Last Modified: Tue, 12 Dec 2017 16:30:08 GMT  
		Size: 4.2 MB (4173587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:onbuild`

```console
$ docker pull pypy@sha256:a675ac6d32d30f00298115e7a428f1f1069e5577fddcadb8493e3256fa37b947
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:onbuild` - linux; amd64

```console
$ docker pull pypy@sha256:a5f78b6cde0e81f6dffe84eb0a24db0d95234942c0a9265a01e484c8889a29d4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.7 MB (282733961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f559a3ba3832c1eb8cf7db289e5d456e84ef32e4c830a6ae71dfe02b8c0edff`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:49:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:49:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:50:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 16:26:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 16:26:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		tcl 		tk 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:26:26 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 16:26:27 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 16:27:39 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version
# Tue, 12 Dec 2017 16:27:52 GMT
RUN set -ex; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py
# Tue, 12 Dec 2017 16:27:52 GMT
CMD ["pypy3"]
# Tue, 12 Dec 2017 16:28:02 GMT
RUN mkdir -p /usr/src/app
# Tue, 12 Dec 2017 16:28:02 GMT
WORKDIR /usr/src/app
# Tue, 12 Dec 2017 16:28:02 GMT
ONBUILD COPY requirements.txt /usr/src/app/
# Tue, 12 Dec 2017 16:28:02 GMT
ONBUILD RUN pip install -r requirements.txt
# Tue, 12 Dec 2017 16:28:03 GMT
ONBUILD COPY . /usr/src/app
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b491c575b06601bb07a2d88bfc3ace6c6005edc1b4d8da3ba6e37e04e9592d6`  
		Last Modified: Tue, 12 Dec 2017 08:00:34 GMT  
		Size: 19.3 MB (19266203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313b08bab3b8bbcf0de4171a2a80a01e67fab094f272819b76a58705d21ab28`  
		Last Modified: Tue, 12 Dec 2017 08:01:02 GMT  
		Size: 43.3 MB (43253338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6678c3f0e0c6e2b58b51ad100912b7c0e4dfedf98a1808417216fd5d948e5`  
		Last Modified: Tue, 12 Dec 2017 08:01:40 GMT  
		Size: 135.0 MB (134968174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f35bd58db288964a8bb8698b5f41bfb05df1758e54c2aad2f3fda3c38b240a`  
		Last Modified: Tue, 12 Dec 2017 16:28:20 GMT  
		Size: 3.2 MB (3167686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e9b028e52f19d4499fef7b5124e78a03adac776f518eae325ed99cb3ce5fb3`  
		Last Modified: Tue, 12 Dec 2017 16:30:14 GMT  
		Size: 25.3 MB (25305144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee65405971a25347ac7d2f8d967e946a192e4a4a6fbc4df5d336f10b99c6a6cd`  
		Last Modified: Tue, 12 Dec 2017 16:30:08 GMT  
		Size: 4.2 MB (4173587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89b61d544df4f7f9e32ace5502607095efdb9b0ed3c9cf924e547d4b9f762eb`  
		Last Modified: Tue, 12 Dec 2017 16:31:26 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `pypy:slim`

```console
$ docker pull pypy@sha256:8e1a64f28581c0ab1e9cf8e54c52644ec3ebb68c6ee8663c74e491dd66ab6db7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `pypy:slim` - linux; amd64

```console
$ docker pull pypy@sha256:e296f17128e5a549a71dcea9f6a7fd3abedcf9203bbdc3d3073ed9c971cb9c36
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62751328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebdc0f0f45622fe90ead8acf85e77fb7f1ac6aaf5db8c083736347d3aec4dd8f`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 06:21:38 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2017 06:21:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 06:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYPY_VERSION=5.9.0
# Tue, 12 Dec 2017 06:21:51 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 12 Dec 2017 06:27:38 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d8c41ede3758127718944cc2fd6bf78ed4303d946f85596cac91281ccce36165' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		fetchDeps=' 		bzip2 		wget 	'; 	apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/*; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3-v${PYPY_VERSION}-${pypyArch}.tar.bz2"; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	rm pypy.tar.bz2; 		pypy3 --version; 		wget -O get-pip.py 'https://bootstrap.pypa.io/get-pip.py'; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		rm -f get-pip.py; 		apt-get purge -y --auto-remove $fetchDeps
# Tue, 12 Dec 2017 06:27:38 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ed6d99248693c2acd5109ff75533464052952167eca48dbf989268a392ebb3`  
		Last Modified: Tue, 12 Dec 2017 06:28:04 GMT  
		Size: 2.9 MB (2859578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af11562222d940dc258b1b84b125ce27dc650550602b677b1f49b73a1b490e53`  
		Last Modified: Tue, 12 Dec 2017 06:29:20 GMT  
		Size: 29.8 MB (29777231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
