## `haproxy:latest`

```console
$ docker pull haproxy@sha256:0727d6ecebb4d76b26084cb6a82ba58e5b7cfdbfcc9ee30521117290092ce5fd
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

### `haproxy:latest` - linux; amd64

```console
$ docker pull haproxy@sha256:9d66628439b2750a92e02ab1444bd8b543823be52483867e6daa36e82774627c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.2 MB (28211715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1b621468560ace94b350f6ae291b45c8154693b73e61d85b2a715813ffc2cb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Dec 2017 01:44:43 GMT
ADD file:f30a8b5b7cdc9ba33a250899308b490baa9f7a9b29d3a85bd16200aa0a28a04a in / 
# Tue, 12 Dec 2017 01:44:43 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 04:22:11 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		liblua5.3-0 		libpcre3 		libssl1.1 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 04:22:11 GMT
ENV HAPROXY_MAJOR=1.8
# Tue, 12 Dec 2017 04:22:11 GMT
ENV HAPROXY_VERSION=1.8.1
# Tue, 12 Dec 2017 04:22:11 GMT
ENV HAPROXY_MD5=e42892d4b6ee33200fccaa1d81837e49
# Tue, 12 Dec 2017 04:22:50 GMT
RUN set -x 		&& buildDeps=' 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre3-dev 		libssl-dev 		zlib1g-dev 		make 		wget 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "http://www.haproxy.org/download/${HAPROXY_MAJOR}/src/haproxy-${HAPROXY_VERSION}.tar.gz" 	&& echo "$HAPROXY_MD5 *haproxy.tar.gz" | md5sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE=1 PCREDIR= 		USE_ZLIB=1 	' 	&& make -C /usr/src/haproxy -j "$(nproc)" all $makeOpts 	&& make -C /usr/src/haproxy install-bin $makeOpts 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Dec 2017 04:22:50 GMT
COPY file:9489da093f9bbacb372aa24916cd4607d45b831e8054d997ab55a1be7b595c17 in / 
# Tue, 12 Dec 2017 04:22:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Dec 2017 04:22:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e7bb522d92ff6d4e5b2087409b0fc783c2e3b06acf87bee739ee47d90bf02e96`  
		Last Modified: Tue, 12 Dec 2017 01:54:56 GMT  
		Size: 22.5 MB (22485719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cdaa8b3baaf1123026bf0e84d9afea2e04e74ca8c4d3aaacf1b774b627b03f`  
		Last Modified: Tue, 12 Dec 2017 04:25:08 GMT  
		Size: 2.1 MB (2102222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27b12ec5042dc3bb3e8a01c5d6240057afc8712e8ad6ac5fc1be369f64c981e`  
		Last Modified: Tue, 12 Dec 2017 04:25:10 GMT  
		Size: 3.6 MB (3623394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc8fcb06e65eede96eb153ddc179e6b5690055f7f643e2c306d56e4563a7020`  
		Last Modified: Tue, 12 Dec 2017 04:25:08 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:46b0e3dbde78358cc0f30d6a31df4eef1b3d6313ef7094696ec20da376b68ee6
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.5 MB (26542745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f951eebd67b798893adea071d8672e51207dddd3c6aacb42ea74cc31e76a351`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Dec 2017 21:02:20 GMT
ADD file:f69e5781e9ff2a9867d94175d91d31553e07613bf4b50a1064274ed21a5ed353 in / 
# Tue, 12 Dec 2017 21:02:21 GMT
CMD ["bash"]
# Wed, 13 Dec 2017 00:26:04 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		liblua5.3-0 		libpcre3 		libssl1.1 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 00:26:05 GMT
ENV HAPROXY_MAJOR=1.8
# Wed, 13 Dec 2017 00:26:05 GMT
ENV HAPROXY_VERSION=1.8.1
# Wed, 13 Dec 2017 00:26:05 GMT
ENV HAPROXY_MD5=e42892d4b6ee33200fccaa1d81837e49
# Wed, 13 Dec 2017 00:26:37 GMT
RUN set -x 		&& buildDeps=' 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre3-dev 		libssl-dev 		zlib1g-dev 		make 		wget 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "http://www.haproxy.org/download/${HAPROXY_MAJOR}/src/haproxy-${HAPROXY_VERSION}.tar.gz" 	&& echo "$HAPROXY_MD5 *haproxy.tar.gz" | md5sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE=1 PCREDIR= 		USE_ZLIB=1 	' 	&& make -C /usr/src/haproxy -j "$(nproc)" all $makeOpts 	&& make -C /usr/src/haproxy install-bin $makeOpts 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Dec 2017 00:26:38 GMT
COPY file:9489da093f9bbacb372aa24916cd4607d45b831e8054d997ab55a1be7b595c17 in / 
# Wed, 13 Dec 2017 00:26:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Dec 2017 00:26:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:20f319b2549a8d631c2e8034bfc3f9c12042d86a686470a8addd2fb7bc8c688c`  
		Last Modified: Tue, 12 Dec 2017 21:12:53 GMT  
		Size: 21.2 MB (21160630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cf159cd0afbefc45df81a0ec1fbcc832e3df214c4081e30a7f12e14ba36995`  
		Last Modified: Wed, 13 Dec 2017 00:28:16 GMT  
		Size: 1.8 MB (1816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ebc9ff5413420cf81a30705f1045ede39467ffc21a4124612f2c2cd9f3e23f`  
		Last Modified: Wed, 13 Dec 2017 00:28:17 GMT  
		Size: 3.6 MB (3565707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e8ad2dad4db3e7a724ea45f5924021ea15ca576ea146e68cb38ee56802f481`  
		Last Modified: Wed, 13 Dec 2017 00:28:16 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:d948ed0aa78b4f87035088fa6d859882a31e178da34882d4d065c09eaaa743a2
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.5 MB (24521362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fadce531ed0b3afd4510c54802e6a9e1c92426bfa72cb126cb0959263ea0931e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Dec 2017 13:33:42 GMT
ADD file:cfde12259adb7102e76690e986f1b9b07967a8984c85d0cead09969f5de8b8cc in / 
# Tue, 12 Dec 2017 13:33:42 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:19:05 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		liblua5.3-0 		libpcre3 		libssl1.1 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:19:12 GMT
ENV HAPROXY_MAJOR=1.8
# Tue, 12 Dec 2017 14:19:12 GMT
ENV HAPROXY_VERSION=1.8.1
# Tue, 12 Dec 2017 14:19:12 GMT
ENV HAPROXY_MD5=e42892d4b6ee33200fccaa1d81837e49
# Tue, 12 Dec 2017 14:19:41 GMT
RUN set -x 		&& buildDeps=' 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre3-dev 		libssl-dev 		zlib1g-dev 		make 		wget 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "http://www.haproxy.org/download/${HAPROXY_MAJOR}/src/haproxy-${HAPROXY_VERSION}.tar.gz" 	&& echo "$HAPROXY_MD5 *haproxy.tar.gz" | md5sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE=1 PCREDIR= 		USE_ZLIB=1 	' 	&& make -C /usr/src/haproxy -j "$(nproc)" all $makeOpts 	&& make -C /usr/src/haproxy install-bin $makeOpts 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Dec 2017 14:19:42 GMT
COPY file:9489da093f9bbacb372aa24916cd4607d45b831e8054d997ab55a1be7b595c17 in / 
# Tue, 12 Dec 2017 14:19:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Dec 2017 14:19:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cd8b673adb84fd5eae3444d0475addad7e8908a8332704c4407baa97e9b0b284`  
		Last Modified: Tue, 12 Dec 2017 13:45:48 GMT  
		Size: 19.3 MB (19271028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3ef6d2c95a1ff672aabb9794a8eccc7e120ccf208f871a715332c909638dd9`  
		Last Modified: Tue, 12 Dec 2017 14:21:59 GMT  
		Size: 1.7 MB (1736097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85600cd6a6076d0de34560666b6cf8ce9903d1d3f3bbba76bc2912995c2365bf`  
		Last Modified: Tue, 12 Dec 2017 14:21:59 GMT  
		Size: 3.5 MB (3513857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde164830b19e269294e8e65a22ac3320e6bee3ede4d5b427f543c79239ad0a2`  
		Last Modified: Tue, 12 Dec 2017 14:21:58 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ddd58560f67ca1e1efa814f38b925b8d0924a116f53253e6933662bac5b29741
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25682561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7019fb6b294d5e014c6ce4a103d00989d291cb561fb5f7e3b97b09db37e4045`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Dec 2017 18:34:13 GMT
ADD file:6e068c7cc5397bfb4ec60dab4d410c5d3ba724f20ad0129d2032fb509f0eadcd in / 
# Tue, 12 Dec 2017 18:34:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2017 20:58:50 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		liblua5.3-0 		libpcre3 		libssl1.1 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2017 20:58:51 GMT
ENV HAPROXY_MAJOR=1.8
# Tue, 19 Dec 2017 20:58:52 GMT
ENV HAPROXY_VERSION=1.8.1
# Tue, 19 Dec 2017 20:58:53 GMT
ENV HAPROXY_MD5=e42892d4b6ee33200fccaa1d81837e49
# Tue, 19 Dec 2017 21:01:16 GMT
RUN set -x 		&& buildDeps=' 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre3-dev 		libssl-dev 		zlib1g-dev 		make 		wget 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "http://www.haproxy.org/download/${HAPROXY_MAJOR}/src/haproxy-${HAPROXY_VERSION}.tar.gz" 	&& echo "$HAPROXY_MD5 *haproxy.tar.gz" | md5sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE=1 PCREDIR= 		USE_ZLIB=1 	' 	&& make -C /usr/src/haproxy -j "$(nproc)" all $makeOpts 	&& make -C /usr/src/haproxy install-bin $makeOpts 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-get purge -y --auto-remove $buildDeps
# Tue, 19 Dec 2017 21:01:17 GMT
COPY file:9489da093f9bbacb372aa24916cd4607d45b831e8054d997ab55a1be7b595c17 in / 
# Tue, 19 Dec 2017 21:01:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 19 Dec 2017 21:01:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad8cfc11c78a53ccf9aafafcb3ded5044dbd181977e6255aea54fbe164f131`  
		Last Modified: Tue, 12 Dec 2017 18:49:05 GMT  
		Size: 20.3 MB (20331270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46333d8b6ada4194652a0ceb17abc634c09c7e866202ffbb946654940035b885`  
		Last Modified: Tue, 19 Dec 2017 21:02:53 GMT  
		Size: 1.8 MB (1818765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b965ac1f7d32e38aa0f1cad5afec9e299789a37c0263d7c3b2b927665698722b`  
		Last Modified: Tue, 19 Dec 2017 21:02:54 GMT  
		Size: 3.5 MB (3532146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b14342af37721b77f57ec4e41afbd31d1aee828dd20896f317109e333de7de`  
		Last Modified: Tue, 19 Dec 2017 21:02:51 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; 386

```console
$ docker pull haproxy@sha256:399feeceb73d08318a7e02b902bbd263aac873240235e9d6410b0e3cbbb92737
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28789113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed1532363e21ce0089458d3e7d20afe4927d9f4b9db7b5194caa49a5db9fb62b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Dec 2017 14:36:09 GMT
ADD file:ef60a5257bf2b5766f692e39f5922bbd6161e45de184b7b138522d53a477c7af in / 
# Tue, 12 Dec 2017 14:36:09 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 16:54:39 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		liblua5.3-0 		libpcre3 		libssl1.1 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 16:54:39 GMT
ENV HAPROXY_MAJOR=1.8
# Tue, 12 Dec 2017 16:54:39 GMT
ENV HAPROXY_VERSION=1.8.1
# Tue, 12 Dec 2017 16:54:39 GMT
ENV HAPROXY_MD5=e42892d4b6ee33200fccaa1d81837e49
# Tue, 12 Dec 2017 16:55:46 GMT
RUN set -x 		&& buildDeps=' 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre3-dev 		libssl-dev 		zlib1g-dev 		make 		wget 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "http://www.haproxy.org/download/${HAPROXY_MAJOR}/src/haproxy-${HAPROXY_VERSION}.tar.gz" 	&& echo "$HAPROXY_MD5 *haproxy.tar.gz" | md5sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE=1 PCREDIR= 		USE_ZLIB=1 	' 	&& make -C /usr/src/haproxy -j "$(nproc)" all $makeOpts 	&& make -C /usr/src/haproxy install-bin $makeOpts 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Dec 2017 16:55:46 GMT
COPY file:9489da093f9bbacb372aa24916cd4607d45b831e8054d997ab55a1be7b595c17 in / 
# Tue, 12 Dec 2017 16:55:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Dec 2017 16:55:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:4dbce982b05e209cf10a433462dc417f7816c47b0c1a151c8c93206b299b9a14`  
		Last Modified: Tue, 12 Dec 2017 15:03:13 GMT  
		Size: 23.1 MB (23122456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb9ad45fedcb1d21c2ac6eababf1d7231e50f9d7ee2724fdb567cb1009135db`  
		Last Modified: Tue, 12 Dec 2017 17:03:38 GMT  
		Size: 2.1 MB (2128528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee9996a5d01994f08a89658de456dbc48cdb2ee58a4f2f7fcdc3a428fb73232`  
		Last Modified: Tue, 12 Dec 2017 17:03:39 GMT  
		Size: 3.5 MB (3537749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14c6a459754f939607b7fadcb403028954f2f8b3f6bbf40813a7d5490ebbaab`  
		Last Modified: Tue, 12 Dec 2017 17:03:37 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; ppc64le

```console
$ docker pull haproxy@sha256:ed78b29bb37d29d36d575a1d9c1a9d3adb32ad6c0e9dd5df402306d4901ea70f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28131317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b263bca2a4e600c843540f0ec3bc05efa65c36578cb03fb30725caa2244bc1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Dec 2017 01:35:41 GMT
ADD file:896602a6d015367badb26a7ac0bcafc9aa04cbba205925631d315874b6d289ab in / 
# Tue, 12 Dec 2017 01:35:42 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:17:51 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		liblua5.3-0 		libpcre3 		libssl1.1 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 02:17:52 GMT
ENV HAPROXY_MAJOR=1.8
# Tue, 12 Dec 2017 02:17:53 GMT
ENV HAPROXY_VERSION=1.8.1
# Tue, 12 Dec 2017 02:17:54 GMT
ENV HAPROXY_MD5=e42892d4b6ee33200fccaa1d81837e49
# Tue, 12 Dec 2017 02:21:08 GMT
RUN set -x 		&& buildDeps=' 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre3-dev 		libssl-dev 		zlib1g-dev 		make 		wget 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "http://www.haproxy.org/download/${HAPROXY_MAJOR}/src/haproxy-${HAPROXY_VERSION}.tar.gz" 	&& echo "$HAPROXY_MD5 *haproxy.tar.gz" | md5sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE=1 PCREDIR= 		USE_ZLIB=1 	' 	&& make -C /usr/src/haproxy -j "$(nproc)" all $makeOpts 	&& make -C /usr/src/haproxy install-bin $makeOpts 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Dec 2017 02:21:10 GMT
COPY file:9489da093f9bbacb372aa24916cd4607d45b831e8054d997ab55a1be7b595c17 in / 
# Tue, 12 Dec 2017 02:21:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Dec 2017 02:21:13 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b8b738bec437a97371af422179183d09cdb031f677b2dba4deaed774655ee9d8`  
		Last Modified: Tue, 12 Dec 2017 01:42:57 GMT  
		Size: 22.7 MB (22739713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8a1365bd6d4c9c6db8b5c3305fe4af8e0aa7e654b4460d27bd7c19a55b3616`  
		Last Modified: Tue, 12 Dec 2017 02:22:54 GMT  
		Size: 1.8 MB (1781148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a334b7b8c7c9742f1266f43854f6b5ea6d682047a1c812e3457f6da4782f6965`  
		Last Modified: Tue, 12 Dec 2017 02:22:54 GMT  
		Size: 3.6 MB (3610077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934e8287d3c0ecff99a70a5a4143f2a682d488d8822dfeba773028aff2b356e6`  
		Last Modified: Tue, 12 Dec 2017 02:22:52 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; s390x

```console
$ docker pull haproxy@sha256:75e7c534384ca70c8b671a4beb13a8843045f112d346336c0123e1e9c822b1d5
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27883879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422e9727a211f905b42ca2e6dbc8ccbc96d4ac346ee99de04c4a6819ad8afc53`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Dec 2017 06:25:50 GMT
ADD file:8cd208817150f41f5b21f5c2b6641af023ddeaa6d842fe490190e20effe94a08 in / 
# Tue, 12 Dec 2017 06:25:51 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:19:39 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		liblua5.3-0 		libpcre3 		libssl1.1 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:19:39 GMT
ENV HAPROXY_MAJOR=1.8
# Tue, 12 Dec 2017 07:19:40 GMT
ENV HAPROXY_VERSION=1.8.1
# Tue, 12 Dec 2017 07:19:40 GMT
ENV HAPROXY_MD5=e42892d4b6ee33200fccaa1d81837e49
# Tue, 12 Dec 2017 07:20:29 GMT
RUN set -x 		&& buildDeps=' 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre3-dev 		libssl-dev 		zlib1g-dev 		make 		wget 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "http://www.haproxy.org/download/${HAPROXY_MAJOR}/src/haproxy-${HAPROXY_VERSION}.tar.gz" 	&& echo "$HAPROXY_MD5 *haproxy.tar.gz" | md5sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE=1 PCREDIR= 		USE_ZLIB=1 	' 	&& make -C /usr/src/haproxy -j "$(nproc)" all $makeOpts 	&& make -C /usr/src/haproxy install-bin $makeOpts 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Dec 2017 07:20:29 GMT
COPY file:9489da093f9bbacb372aa24916cd4607d45b831e8054d997ab55a1be7b595c17 in / 
# Tue, 12 Dec 2017 07:20:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Dec 2017 07:20:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:da91ecedba56836763b256841bfd01198234139e3e4824510318c25fa8cf140a`  
		Last Modified: Tue, 12 Dec 2017 06:31:22 GMT  
		Size: 22.3 MB (22333855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bc8a405bdaf03a9c517d128312ae2d152475467884aa84696f8c32cb39eabb`  
		Last Modified: Tue, 12 Dec 2017 07:21:49 GMT  
		Size: 1.8 MB (1841046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275f882688c782d5c571f369e8ae5ca47d7a4a066aaacf2adc036bc0d7eef566`  
		Last Modified: Tue, 12 Dec 2017 07:21:50 GMT  
		Size: 3.7 MB (3708598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdfed41e87aae78edb8b97e24532c64484c91f7c85169e59493f729d2ab9f01`  
		Last Modified: Tue, 12 Dec 2017 07:21:49 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
