## `openjdk:9-jre`

```console
$ docker pull openjdk@sha256:989f18b03f5a5f8d322a2bc7476c523164581d529679016e4226f22fadb57964
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `openjdk:9-jre` - linux; amd64

```console
$ docker pull openjdk@sha256:8fe4be01849eec3313af890f0e28fc18b4308195d875371c51e7276f06627db5
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.6 MB (266649174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:684d135285233f746fb1a0db33dc31863041bc90af76b9ebf17c6fcc1b33b375`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 01:43:09 GMT
ADD file:f4f0ede88e0b0edf8235b2a5ff46ab7d8de71d56720cb7dc3032bca0e1872695 in / 
# Tue, 12 Dec 2017 01:43:10 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:51:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:51:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 15:35:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:35:08 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:35:09 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 15:35:10 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 15:35:10 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Dec 2017 15:35:11 GMT
ENV JAVA_VERSION=9.0.1+11
# Tue, 12 Dec 2017 15:35:11 GMT
ENV JAVA_DEBIAN_VERSION=9.0.1+11-1
# Tue, 12 Dec 2017 15:36:40 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-9-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:a8797cd0c76e8b1532d95708a0a38554c89e6fa0cdd856dbede8555225cdea00`  
		Last Modified: Tue, 12 Dec 2017 01:51:30 GMT  
		Size: 48.4 MB (48429060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdce62b256df9c745afac618b5a44d73531cede1a187586e73ed27bd7e1c508`  
		Last Modified: Tue, 12 Dec 2017 08:01:58 GMT  
		Size: 8.6 MB (8636787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c93763e33f35c3974631198e261ac389cb564d90b37f0443650ce34fee2dba2`  
		Last Modified: Tue, 12 Dec 2017 08:01:57 GMT  
		Size: 9.0 MB (8973876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b42e2b6acf2a08ab33b82572cb072d8e1cfd20c7d010dd6c41ede9f0dbb203c`  
		Last Modified: Tue, 12 Dec 2017 16:23:43 GMT  
		Size: 856.3 KB (856290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70c0c61f6ccce429addc51d385196e97bf3ba304c01fad9b18c6271c2a75748`  
		Last Modified: Tue, 12 Dec 2017 16:23:43 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7808b0c016fd3ac7ac75aaebae9a3eee2244b419df4fdd9adaed1ad41b376633`  
		Last Modified: Tue, 12 Dec 2017 16:23:43 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861e7ea31247a5bb3256a6cc6e0b6aedb0b9e72c5063d61de2730ae30560963a`  
		Last Modified: Tue, 12 Dec 2017 16:24:36 GMT  
		Size: 199.8 MB (199752783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:9-jre` - linux; arm variant v5

```console
$ docker pull openjdk@sha256:fa8a2b58ade0ac58c7425fe6946214c4eda3466350554c22cc2efea38d701d36
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.6 MB (245641334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc77697a6da2cf4bfa3ad6318658f9032bfade3f396270d41edbbdf23fffc30a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 20:59:59 GMT
ADD file:af4cd7d5c7a1769f049a442dfd7a1b0fa6359ce5306569a5130c55609ec5175e in / 
# Tue, 12 Dec 2017 20:59:59 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 22:56:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:56:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 23:43:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 23:43:43 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 23:43:44 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 23:43:45 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 23:43:45 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Dec 2017 23:43:46 GMT
ENV JAVA_VERSION=9.0.1+11
# Tue, 12 Dec 2017 23:43:46 GMT
ENV JAVA_DEBIAN_VERSION=9.0.1+11-1
# Tue, 12 Dec 2017 23:45:43 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-9-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:acff8687551d235a654afe80e0891cce1bd27c306fff4e41bb6b44b226a473e4`  
		Last Modified: Tue, 12 Dec 2017 21:10:06 GMT  
		Size: 46.9 MB (46876188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12a8cc19c8faf784e145d3a3c486d1b5a0892e4af7a81189d15f0eb18053a58`  
		Last Modified: Tue, 12 Dec 2017 23:08:24 GMT  
		Size: 7.8 MB (7808219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93c884700496b57c386401815cba851f8f8f992a0295e68194990608ff2dea2`  
		Last Modified: Tue, 12 Dec 2017 23:08:23 GMT  
		Size: 8.7 MB (8718966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddbd75681696fa7b3b62dd3fd7842ac4be43019cf6f706d6042ed3b41d4adbd`  
		Last Modified: Wed, 13 Dec 2017 00:01:18 GMT  
		Size: 849.3 KB (849337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc789f2e38f7d5b8cd70cb0cc222351233f130f5d9c96706d3d505851cb7c37`  
		Last Modified: Wed, 13 Dec 2017 00:01:18 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f823dfaba955af64fa3d668b036b56dc0fd62fcfafbc643e1fea11de3c8a799`  
		Last Modified: Wed, 13 Dec 2017 00:01:18 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368e80a821a4507e4b2ceaa6f96722cbf0f842713a4c6a6f1a3afa9385bc7e21`  
		Last Modified: Wed, 13 Dec 2017 00:02:06 GMT  
		Size: 181.4 MB (181388246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:9-jre` - linux; arm variant v7

```console
$ docker pull openjdk@sha256:0b35f770266d148101d779975e852eaa34547debd6f72f50810c654aae25f8c8
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.5 MB (241512030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86573f4a305f3bddef55c1cf2ff17d0491339d28fff4bc327615c1555de64668`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 13:30:47 GMT
ADD file:b788e24f4cada715c58008741a4bc6b55912bf54f897e9febf55038c7259474a in / 
# Tue, 12 Dec 2017 13:30:48 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:18:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 15:24:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:24:03 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:24:04 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 15:24:05 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 15:24:05 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Dec 2017 15:24:06 GMT
ENV JAVA_VERSION=9.0.1+11
# Tue, 12 Dec 2017 15:24:06 GMT
ENV JAVA_DEBIAN_VERSION=9.0.1+11-1
# Tue, 12 Dec 2017 15:25:01 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-9-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:ee9da7ca0ecfb9e496d4e6a11a2de17d38b2676f64081ca6643b85f1026bd24a`  
		Last Modified: Tue, 12 Dec 2017 13:42:33 GMT  
		Size: 44.8 MB (44836300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9035433aec00afaaa737a1213c4367cab1ef3d7a572aa2cb952e73854b963d0`  
		Last Modified: Tue, 12 Dec 2017 14:32:26 GMT  
		Size: 7.5 MB (7534247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d036c584b8f46f4616710df516ffdb5657ef66387fcf24bd3752cdeaf9091427`  
		Last Modified: Tue, 12 Dec 2017 14:32:26 GMT  
		Size: 8.4 MB (8438419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8053ed8fc580846cce780616eb015dd48cb75ce50026b0651185fdc9b68f4d`  
		Last Modified: Tue, 12 Dec 2017 15:40:57 GMT  
		Size: 833.0 KB (833006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0b66db551911f881340feffd442e3e6e7cfb7fd8eb95cab7ec3f997a023348`  
		Last Modified: Tue, 12 Dec 2017 15:40:57 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6687521354339ce192f9f65105ca6daea26726b87076dc6da633f404d61bd94e`  
		Last Modified: Tue, 12 Dec 2017 15:40:57 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217d742570881fbcd9c5d15560ccf4cf3c6420826f6177844d143b41791c819b`  
		Last Modified: Tue, 12 Dec 2017 15:41:40 GMT  
		Size: 179.9 MB (179869680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:9-jre` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:17beac0b8f1c40bf3f9e61d0e4cbd8371a1588b93ec00346292207b47df8acf9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.0 MB (247047968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59286c82137c7472748077f7329bee8efa97af036f07a1b1fb5ebe040e3e4dc3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 18:28:41 GMT
ADD file:7487b447e9ae95ddff2e8f1bbdc2b089a3a6fb70edf7f218bf3c662727c19ade in / 
# Tue, 12 Dec 2017 18:28:42 GMT
CMD ["bash"]
# Fri, 15 Dec 2017 16:02:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 Dec 2017 16:03:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 Dec 2017 21:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 Dec 2017 21:13:57 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2017 21:13:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 15 Dec 2017 21:14:01 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Fri, 15 Dec 2017 21:14:02 GMT
ENV JAVA_HOME=/docker-java-home
# Fri, 15 Dec 2017 21:14:02 GMT
ENV JAVA_VERSION=9.0.1+11
# Fri, 15 Dec 2017 21:14:03 GMT
ENV JAVA_DEBIAN_VERSION=9.0.1+11-1
# Fri, 15 Dec 2017 21:20:37 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-9-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:aa10cf671b46f67e3e12579e72f085c7b8402ff25ccafb8616eb9e1cbe71bf85`  
		Last Modified: Tue, 12 Dec 2017 18:44:03 GMT  
		Size: 46.2 MB (46188985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cce7e08176846c9ad6c15ff845d12c630e1d4ab1a0f8ef1e7a0786ec45ad2b`  
		Last Modified: Fri, 15 Dec 2017 17:17:29 GMT  
		Size: 7.9 MB (7856875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a14a037f71e9308ee97c32436f3203d1f06a675930a80dba9a16c2f5c78166`  
		Last Modified: Fri, 15 Dec 2017 17:17:29 GMT  
		Size: 8.7 MB (8712398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fa8eea21357a0c5faac2654ad9623138d46d73e90554a9372aa7cfd9111e7d`  
		Last Modified: Fri, 15 Dec 2017 21:25:45 GMT  
		Size: 842.5 KB (842524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a502faa1b54b0c96a1a1b64613e97f02285a02216632af1113aa4e2ebfb7ee`  
		Last Modified: Fri, 15 Dec 2017 21:25:44 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a78d44f8315eda6986a14238b45fbfd8eb7fe7f29cb41cb2f714c17cc7ad746`  
		Last Modified: Fri, 15 Dec 2017 21:25:43 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9e3cbfbdc6558d77c9dca3e84299b6a78206769fdd9355ed91d4d7d8eaeed3`  
		Last Modified: Fri, 15 Dec 2017 21:26:38 GMT  
		Size: 183.4 MB (183446807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:9-jre` - linux; 386

```console
$ docker pull openjdk@sha256:6c82174130d2954db2267497c872af5357ec04f64ab530eb06de1a123bf2c5cd
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.9 MB (276918384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d00d77d5cc92fd3900dc03852548d6b64ff2b2dad631dbcc01dbfd1f49098378`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 14:24:56 GMT
ADD file:7e72f60be83facf3a36831facc1a26f572f3ae83fc49b2bc4c8de0b6e3321e84 in / 
# Tue, 12 Dec 2017 14:24:56 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 17:02:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 17:02:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 19:07:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 19:07:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 19:07:12 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 19:07:13 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 19:07:13 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Dec 2017 19:07:13 GMT
ENV JAVA_VERSION=9.0.1+11
# Tue, 12 Dec 2017 19:07:14 GMT
ENV JAVA_DEBIAN_VERSION=9.0.1+11-1
# Tue, 12 Dec 2017 19:09:07 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-9-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:c3cf1d3d69aef55e4aef2c1f0a9455d1dfbbb7ae17d15a0d963e8c55e6e61af4`  
		Last Modified: Tue, 12 Dec 2017 14:58:13 GMT  
		Size: 49.3 MB (49250980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e767ba54897a1df6013ec3b06fd1546d3123979a02ac1f8f8eb0f079fd928126`  
		Last Modified: Tue, 12 Dec 2017 17:33:48 GMT  
		Size: 8.6 MB (8608693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936341216c1a183dced55abc7be29ddca5b53a3fe1a3d85f00538784bd1a090d`  
		Last Modified: Tue, 12 Dec 2017 17:33:48 GMT  
		Size: 9.3 MB (9251281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8218fb4c74ebf68ad66d2edba5ca7160ff1fba80f1227ba2660c7b88290f00b`  
		Last Modified: Tue, 12 Dec 2017 20:06:42 GMT  
		Size: 864.9 KB (864922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d277b185f0070b638e3c50ec9acdd09e4350fef5e204bc34823ec98ea25adf`  
		Last Modified: Tue, 12 Dec 2017 20:06:42 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d694e119754e7a127a91005e34fae3b7e6c09c42170b19181296893abf2a233a`  
		Last Modified: Tue, 12 Dec 2017 20:06:43 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253cf52d52ea4125630fedf8fa9a34ef6dcf36a0884365973a6a02f3e92f2f5d`  
		Last Modified: Tue, 12 Dec 2017 20:07:41 GMT  
		Size: 208.9 MB (208942130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:9-jre` - linux; ppc64le

```console
$ docker pull openjdk@sha256:6a826e0742ccd3f40ce712d192a106510f5fc598f12a45b18db3c8e10c63daee
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.5 MB (257541298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:731930f6e56d67f5ef962ef034c1e322cfce234c2b923ee289ba0c6de606615d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 01:34:15 GMT
ADD file:7904a0f79cc86767c6e3ac367f0df06aa262c6639e79e39652eac766c3faf4b6 in / 
# Tue, 12 Dec 2017 01:34:16 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 03:12:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 03:13:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 Dec 2017 06:36:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 Dec 2017 06:36:06 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2017 06:36:10 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 15 Dec 2017 06:36:13 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Fri, 15 Dec 2017 06:36:15 GMT
ENV JAVA_HOME=/docker-java-home
# Fri, 15 Dec 2017 06:36:16 GMT
ENV JAVA_VERSION=9.0.1+11
# Fri, 15 Dec 2017 06:36:22 GMT
ENV JAVA_DEBIAN_VERSION=9.0.1+11-1
# Fri, 15 Dec 2017 06:45:24 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-9-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:21b73404fd38d2445a6ecbcf148b2dd5047623273b33ea9546ddf6796601ec9b`  
		Last Modified: Tue, 12 Dec 2017 01:40:28 GMT  
		Size: 49.7 MB (49652013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3d5e1672290a07cf756dbcee37e26f4e406df9a113e8e2dc11abbc2b31d867`  
		Last Modified: Tue, 12 Dec 2017 03:54:16 GMT  
		Size: 8.2 MB (8207114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7d8032257e5508a59f355bd1eb60e35584078939f47f0f54ca3e647ed03f71`  
		Last Modified: Tue, 12 Dec 2017 03:54:18 GMT  
		Size: 9.2 MB (9192961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945b80e81b6e809ec6e645912b39082de0ebda6755597c055b08cc36afbd1170`  
		Last Modified: Fri, 15 Dec 2017 06:49:32 GMT  
		Size: 852.3 KB (852281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173a50be8418ebd52bf529d947c8c2a513a234b4c8f0043b08810f154aebadc2`  
		Last Modified: Fri, 15 Dec 2017 06:49:41 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e42f1ee3d7c5170848cf90b8a6795fe46f073f9c30a573b3ff3d46b2862dd80`  
		Last Modified: Fri, 15 Dec 2017 06:49:32 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84d91d612bfca2eba2e97e82a6ae91698608b1127f69eee9e6cfe6cc312c998`  
		Last Modified: Fri, 15 Dec 2017 06:50:20 GMT  
		Size: 189.6 MB (189636548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:9-jre` - linux; s390x

```console
$ docker pull openjdk@sha256:74eab3b89b7480eb226942167d9752abd544bf830e54e51c3e7125e84f9f2fa2
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.6 MB (232568499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e7695a4eff897df6a86cb46860e501adbb2f0ec37ffb6e4da0c04d428abdde`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 06:24:08 GMT
ADD file:8ee198fa6df35cac591aebbfa42175a2cab73b8096a422f1a8f995252c8883e8 in / 
# Tue, 12 Dec 2017 06:24:09 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 06:56:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 06:56:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:44:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:44:15 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 07:44:16 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 07:44:16 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 07:44:16 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Dec 2017 07:44:16 GMT
ENV JAVA_VERSION=9.0.1+11
# Tue, 12 Dec 2017 07:44:17 GMT
ENV JAVA_DEBIAN_VERSION=9.0.1+11-1
# Tue, 12 Dec 2017 07:45:05 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-9-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:2556c296741d957f26b83c22fed075dd4d9d0b7075925e7992bc685a3a29eb16`  
		Last Modified: Tue, 12 Dec 2017 06:29:30 GMT  
		Size: 48.1 MB (48137286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d413a8c982037396464e6f9e6eb0e7845e1cc272707609ed8b23d2643e2f1b6`  
		Last Modified: Tue, 12 Dec 2017 07:04:24 GMT  
		Size: 8.2 MB (8168898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ebc4a1cf8c2fc6a586a0d02ce61a52505ac06659ca8124aee9a85f72cdb510`  
		Last Modified: Tue, 12 Dec 2017 07:04:25 GMT  
		Size: 9.0 MB (8950206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3cee7715672e615c4223e9e3b3f09e986bab1eb594298ed475593abdb69ea5`  
		Last Modified: Tue, 12 Dec 2017 07:52:05 GMT  
		Size: 866.9 KB (866864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70e4fb7bcc69c297ecbf5523e21de762cf9d8ca927f7c5b5e10ca8f312d9d93`  
		Last Modified: Tue, 12 Dec 2017 07:52:04 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116e7a6600ef364c687500c418d4cd5c442774a176747a059735b068a03a7389`  
		Last Modified: Tue, 12 Dec 2017 07:52:04 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912d93af40c3c1ef904886dab4b3492abf16a9d8486c021a7a8b2365137b8f0a`  
		Last Modified: Tue, 12 Dec 2017 07:52:29 GMT  
		Size: 166.4 MB (166444866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
