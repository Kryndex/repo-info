## `docker:stable-dind`

```console
$ docker pull docker@sha256:bbd9b34b01fba0240641544571cb7d2b0d2ae4dc2d57d2959432bb5b5b798f11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `docker:stable-dind` - linux; amd64

```console
$ docker pull docker@sha256:93685e1b1f8e93383adc38c9ed9d67a0cc64657ec063863f22fc89f9a4026514
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37110074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3226220d8fad6e5a1109b312197287f25d67a6dcc9e24f0f7c565866245e5cc`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 01 Dec 2017 18:46:26 GMT
ADD file:cb381165dec3689cf77e902c07ea78ca4da6bce4f5ac1909eebd40dba3273bfe in / 
# Fri, 01 Dec 2017 18:46:26 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2017 20:06:17 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 01 Dec 2017 20:06:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 01 Dec 2017 20:07:41 GMT
ENV DOCKER_CHANNEL=stable
# Sat, 09 Dec 2017 01:54:17 GMT
ENV DOCKER_VERSION=17.09.1-ce
# Sat, 09 Dec 2017 01:54:23 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		curl 		tar 	; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		aarch64) dockerArch='aarch64' ;; 		ppc64le) dockerArch='ppc64le' ;; 		s390x) dockerArch='s390x' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! curl -fL -o docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		apk del .fetch-deps; 		dockerd -v; 	docker -v
# Sat, 09 Dec 2017 01:54:24 GMT
COPY file:016ebcc5aefa6b28f6c484a299057d5b236e1d4f3baf44cc76eb4cd578821691 in /usr/local/bin/modprobe 
# Sat, 09 Dec 2017 01:54:24 GMT
COPY file:0d94e1cd679f133aab807891a1b00b6aef1a9f1f884108e7a17ddf50ab88f1fb in /usr/local/bin/ 
# Sat, 09 Dec 2017 01:54:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 09 Dec 2017 01:54:25 GMT
CMD ["sh"]
# Sat, 09 Dec 2017 01:54:43 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		xfsprogs 		xz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 09 Dec 2017 01:54:44 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 09 Dec 2017 01:54:44 GMT
ENV DIND_COMMIT=3b5fac462d21ca164b3778647420016315289034
# Sat, 09 Dec 2017 01:54:47 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps libressl; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind; 	apk del .fetch-deps
# Sat, 09 Dec 2017 01:54:47 GMT
COPY file:14215a2b157618f9ff66709b019144b953b95bbd7273096e970306475e524820 in /usr/local/bin/ 
# Sat, 09 Dec 2017 01:54:48 GMT
VOLUME [/var/lib/docker]
# Sat, 09 Dec 2017 01:54:48 GMT
EXPOSE 2375/tcp
# Sat, 09 Dec 2017 01:54:48 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 09 Dec 2017 01:54:48 GMT
CMD []
```

-	Layers:
	-	`sha256:1160f4abea84cbe2f316db6306839d2704f09a04af763ee493dd92cb066c0865`  
		Last Modified: Fri, 01 Dec 2017 18:50:17 GMT  
		Size: 2.0 MB (1991501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9ac44c1841d6907db77d1476941b90fbf7c3499440bf9068a83a66aecc237f`  
		Last Modified: Fri, 01 Dec 2017 20:09:01 GMT  
		Size: 351.0 KB (351004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a848dcd23bd7ecdadc08642cb18c81b6fd36e0f0b99ee7660d13bf5cf244dfc9`  
		Last Modified: Fri, 01 Dec 2017 20:09:02 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c8a92427a446cf0ac3fc603353df13a4f4dbb5bb1da64f8d47a761ce132fc6`  
		Last Modified: Sat, 09 Dec 2017 01:57:40 GMT  
		Size: 30.7 MB (30699780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04cef24525b0e1c60ec7c2b2b58aacf6a8f689eb407188d399d59da14221eec`  
		Last Modified: Sat, 09 Dec 2017 01:57:32 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c545e0de1bf07f02abc2c63bfa308bf400b7b3715d2784724a7cc1743381d6`  
		Last Modified: Sat, 09 Dec 2017 01:57:31 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079de5dcdaeb3120b62dda71c5f750908e601a6a921447bae460ba833e663d39`  
		Last Modified: Sat, 09 Dec 2017 01:58:31 GMT  
		Size: 3.9 MB (3884805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cff50df8898fb06065e77b59af382e839cb73f3549a90607be779d22126cc47`  
		Last Modified: Sat, 09 Dec 2017 01:58:30 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6286d3cc725eafe9d720158ce85c3270252da856340dbcf84e61989bc7774233`  
		Last Modified: Sat, 09 Dec 2017 01:58:30 GMT  
		Size: 179.8 KB (179760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878a13c67e52100af96e3e3d686ede2dfdf9034c7bb63a39e166f7d9ff5ce641`  
		Last Modified: Sat, 09 Dec 2017 01:58:31 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:258696d6435658aa2286a24197e2d8d49bbf08f14ba7b7e0d9264dd1187621f2
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34735538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c64edacf076e2026519a7a6c308ee3836b3b657ce20a4f626c8cecef1bffea`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 25 Oct 2017 23:28:58 GMT
ADD file:45b5d3b8d5490ba7edfca2cf6f54cdcf49c772b0b3a2302ce69a7af061007aa4 in / 
# Wed, 25 Oct 2017 23:28:59 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:59 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 05:15:41 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 26 Oct 2017 05:15:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 26 Oct 2017 05:17:23 GMT
ENV DOCKER_CHANNEL=stable
# Sat, 09 Dec 2017 07:03:01 GMT
ENV DOCKER_VERSION=17.09.1-ce
# Sat, 09 Dec 2017 07:03:09 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		curl 		tar 	; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		aarch64) dockerArch='aarch64' ;; 		ppc64le) dockerArch='ppc64le' ;; 		s390x) dockerArch='s390x' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! curl -fL -o docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		apk del .fetch-deps; 		dockerd -v; 	docker -v
# Sat, 09 Dec 2017 07:03:10 GMT
COPY file:016ebcc5aefa6b28f6c484a299057d5b236e1d4f3baf44cc76eb4cd578821691 in /usr/local/bin/modprobe 
# Sat, 09 Dec 2017 07:03:11 GMT
COPY file:0d94e1cd679f133aab807891a1b00b6aef1a9f1f884108e7a17ddf50ab88f1fb in /usr/local/bin/ 
# Sat, 09 Dec 2017 07:03:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 09 Dec 2017 07:03:12 GMT
CMD ["sh"]
# Sat, 09 Dec 2017 07:03:40 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		xfsprogs 		xz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 09 Dec 2017 07:03:42 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 09 Dec 2017 07:03:42 GMT
ENV DIND_COMMIT=3b5fac462d21ca164b3778647420016315289034
# Sat, 09 Dec 2017 07:03:46 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps libressl; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind; 	apk del .fetch-deps
# Sat, 09 Dec 2017 07:03:47 GMT
COPY file:14215a2b157618f9ff66709b019144b953b95bbd7273096e970306475e524820 in /usr/local/bin/ 
# Sat, 09 Dec 2017 07:03:48 GMT
VOLUME [/var/lib/docker]
# Sat, 09 Dec 2017 07:03:48 GMT
EXPOSE 2375/tcp
# Sat, 09 Dec 2017 07:03:49 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 09 Dec 2017 07:03:50 GMT
CMD []
```

-	Layers:
	-	`sha256:bb473f0ebc12fde1bd45c1bd3c46f2d3aab367b1b7739464771455b9972f7894`  
		Last Modified: Thu, 06 Jul 2017 09:54:42 GMT  
		Size: 1.9 MB (1914748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ff6b7ff3a208b8399e701e7ea1b7edbdc654c8c60d33c6f09a7803e2dda776`  
		Last Modified: Wed, 25 Oct 2017 23:29:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae44a9d929a0f7f774a276b1abeda949212ff63805c2d35fd8e1856cb1e47859`  
		Last Modified: Thu, 26 Oct 2017 05:18:54 GMT  
		Size: 351.5 KB (351492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11fa162bc593505d0e792ade6064701834ba4262cf5fda38fdbe83d0ba13951`  
		Last Modified: Thu, 26 Oct 2017 05:18:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc93ab73b2b68d04f98e12db7fe71ae86ddd9e2f34087838f257083d25b21dd3`  
		Last Modified: Sat, 09 Dec 2017 07:08:57 GMT  
		Size: 28.7 MB (28661421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b724eddb49e908996ef49afab2d1831acf48a515c14bd46e883425c2d4a6f93c`  
		Last Modified: Sat, 09 Dec 2017 07:08:46 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ff49733c5622fa5cbbea15037cf8d8e813404d3a024c09b11a6f4efc86f2e1`  
		Last Modified: Sat, 09 Dec 2017 07:08:46 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755331e8c6cf9b2d56c180e42aca2d556e8e37e9027d584ceb58d42edaa8483c`  
		Last Modified: Sat, 09 Dec 2017 07:10:11 GMT  
		Size: 3.6 MB (3624710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f36091c7e587fc624a7bf4ad95f15bdda465c8dd28639b3dfaefd1c20106b5`  
		Last Modified: Sat, 09 Dec 2017 07:10:08 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5057c80de1d42c35dc7076adb8063a0361c629070d9fdfc6281a93cef3ce04c1`  
		Last Modified: Sat, 09 Dec 2017 07:10:09 GMT  
		Size: 179.8 KB (179761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbb54a5cca2c47be04db2f116cb2bd412d34a315b0d94f3b9bb4a52cb9c0e11`  
		Last Modified: Sat, 09 Dec 2017 07:10:08 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-dind` - linux; ppc64le

```console
$ docker pull docker@sha256:8a3f991e03eb7311c42981a6016766edc2777cfce0a2098f38534a5ffe226005
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33334535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b6d354199cb253cbcabe3206c0b309049161f83072d6a4603bd058a9b1104d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 25 Oct 2017 23:28:47 GMT
ADD file:e0be8616517d68cb80a2f9b74eb967cda22b9937bbcbe8b75b6153815a6f7761 in / 
# Wed, 25 Oct 2017 23:28:48 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:50 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 05:15:23 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 26 Oct 2017 05:15:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 26 Oct 2017 05:17:11 GMT
ENV DOCKER_CHANNEL=stable
# Sat, 09 Dec 2017 11:37:38 GMT
ENV DOCKER_VERSION=17.09.1-ce
# Sat, 09 Dec 2017 11:37:46 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		curl 		tar 	; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		aarch64) dockerArch='aarch64' ;; 		ppc64le) dockerArch='ppc64le' ;; 		s390x) dockerArch='s390x' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! curl -fL -o docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		apk del .fetch-deps; 		dockerd -v; 	docker -v
# Sat, 09 Dec 2017 11:37:47 GMT
COPY file:016ebcc5aefa6b28f6c484a299057d5b236e1d4f3baf44cc76eb4cd578821691 in /usr/local/bin/modprobe 
# Sat, 09 Dec 2017 11:37:49 GMT
COPY file:0d94e1cd679f133aab807891a1b00b6aef1a9f1f884108e7a17ddf50ab88f1fb in /usr/local/bin/ 
# Sat, 09 Dec 2017 11:37:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 09 Dec 2017 11:37:51 GMT
CMD ["sh"]
# Sat, 09 Dec 2017 11:38:05 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		xfsprogs 		xz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 09 Dec 2017 11:38:08 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 09 Dec 2017 11:38:09 GMT
ENV DIND_COMMIT=3b5fac462d21ca164b3778647420016315289034
# Sat, 09 Dec 2017 11:38:14 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps libressl; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind; 	apk del .fetch-deps
# Sat, 09 Dec 2017 11:38:15 GMT
COPY file:14215a2b157618f9ff66709b019144b953b95bbd7273096e970306475e524820 in /usr/local/bin/ 
# Sat, 09 Dec 2017 11:38:16 GMT
VOLUME [/var/lib/docker]
# Sat, 09 Dec 2017 11:38:17 GMT
EXPOSE 2375/tcp
# Sat, 09 Dec 2017 11:38:18 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 09 Dec 2017 11:38:20 GMT
CMD []
```

-	Layers:
	-	`sha256:1e52418956f7d2a8ea35e8e6e3318fd08e005b27457d77868c225e7433bbfa02`  
		Last Modified: Thu, 20 Jul 2017 15:12:59 GMT  
		Size: 2.0 MB (2008578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf472f4e5bb7956ac20bb343b304e1d3de1f79160c0d158cccbe25980022d50`  
		Last Modified: Wed, 25 Oct 2017 23:29:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786040648c6ce95b57cfce679096fb7515d48596fa35ebd8347645924dc7afcf`  
		Last Modified: Thu, 26 Oct 2017 05:18:55 GMT  
		Size: 354.2 KB (354237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb59a10fa001950eb807c32d69dfdb981e184862354d5a807966f342e49f5405`  
		Last Modified: Thu, 26 Oct 2017 05:18:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068c3d40648b7b480b149c37a11cb695ff06a4c2e3ec5eb6002eca9940470caa`  
		Last Modified: Sat, 09 Dec 2017 11:40:31 GMT  
		Size: 28.5 MB (28476511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9019170993a8285d7e06be3031959858b1d2a0cdad6ed9dd92095bfd145aa530`  
		Last Modified: Sat, 09 Dec 2017 11:40:23 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af084a6b9658a788e580d0d73ddfc27ce07df3edd86eae22eee0c018ba9fc77`  
		Last Modified: Sat, 09 Dec 2017 11:40:24 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498401440da790bf1bc3f68e453de047b0d9da4bd87d56e1bc081a9ed5ff2f42`  
		Last Modified: Sat, 09 Dec 2017 11:40:56 GMT  
		Size: 2.3 MB (2315590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691983bf3f2c8d8631e049305366112660f326fe11dd3ba13565feb347f8e6e0`  
		Last Modified: Sat, 09 Dec 2017 11:40:56 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37f0f927596231c7b0ef7c89253e2e7e6a01e3f97ddcc254244e44bea10d798`  
		Last Modified: Sat, 09 Dec 2017 11:40:56 GMT  
		Size: 176.2 KB (176179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44135266f871b96ecbbe8654563ccc9beb44f19355911ac0653ed1673a188e89`  
		Last Modified: Sat, 09 Dec 2017 11:40:56 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-dind` - linux; s390x

```console
$ docker pull docker@sha256:60bf0e2669cbecb2435a3f8d4b6c755d68450dee1d28007575a08ff1bba5810a
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36864551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cb7aa06e4b9dd8c8017290815660a3352f9ca53c5b563dab637697a19ef6f1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 25 Oct 2017 23:28:40 GMT
ADD file:6fbdff4b4c08600e192f5da9b67a02c58759237fb40525d70712104c80c34c48 in / 
# Wed, 25 Oct 2017 23:28:40 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:40 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 03:01:36 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 26 Oct 2017 03:01:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 26 Oct 2017 03:02:17 GMT
ENV DOCKER_CHANNEL=stable
# Sat, 09 Dec 2017 04:02:35 GMT
ENV DOCKER_VERSION=17.09.1-ce
# Sat, 09 Dec 2017 04:02:39 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		curl 		tar 	; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		aarch64) dockerArch='aarch64' ;; 		ppc64le) dockerArch='ppc64le' ;; 		s390x) dockerArch='s390x' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! curl -fL -o docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		apk del .fetch-deps; 		dockerd -v; 	docker -v
# Sat, 09 Dec 2017 04:02:40 GMT
COPY file:016ebcc5aefa6b28f6c484a299057d5b236e1d4f3baf44cc76eb4cd578821691 in /usr/local/bin/modprobe 
# Sat, 09 Dec 2017 04:02:40 GMT
COPY file:0d94e1cd679f133aab807891a1b00b6aef1a9f1f884108e7a17ddf50ab88f1fb in /usr/local/bin/ 
# Sat, 09 Dec 2017 04:02:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 09 Dec 2017 04:02:40 GMT
CMD ["sh"]
# Sat, 09 Dec 2017 04:02:56 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		xfsprogs 		xz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 09 Dec 2017 04:02:56 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 09 Dec 2017 04:02:57 GMT
ENV DIND_COMMIT=3b5fac462d21ca164b3778647420016315289034
# Sat, 09 Dec 2017 04:02:59 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps libressl; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind; 	apk del .fetch-deps
# Sat, 09 Dec 2017 04:02:59 GMT
COPY file:14215a2b157618f9ff66709b019144b953b95bbd7273096e970306475e524820 in /usr/local/bin/ 
# Sat, 09 Dec 2017 04:03:00 GMT
VOLUME [/var/lib/docker]
# Sat, 09 Dec 2017 04:03:00 GMT
EXPOSE 2375/tcp
# Sat, 09 Dec 2017 04:03:00 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 09 Dec 2017 04:03:00 GMT
CMD []
```

-	Layers:
	-	`sha256:d45fd9d3c4f188ab1f3a4bf6a9f5202b3f1577dbb998f5f28e82d192e0c1f0e7`  
		Last Modified: Sat, 17 Jun 2017 20:41:42 GMT  
		Size: 2.1 MB (2065460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5978b6b34b3e943e0fd25dfb50991c0bad82a986cfdaa91c4de756431ba679`  
		Last Modified: Wed, 25 Oct 2017 23:28:59 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c591e288aeff92334ad8b71d06647f63984dee862dde01321a4087557e0691fe`  
		Last Modified: Thu, 26 Oct 2017 03:03:38 GMT  
		Size: 352.5 KB (352514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c7a9baee1e600d6ffd18316c88768a16246fbd81d84f2f217736b364c53bf0`  
		Last Modified: Thu, 26 Oct 2017 03:03:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9528061cc8c4eb2b3de99a1ff83bbb6c466ecf1af170f4db8ad01eb0eb0c66e`  
		Last Modified: Sat, 09 Dec 2017 04:05:05 GMT  
		Size: 30.1 MB (30118644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097dc0672afa3a197279fa59d4f1b3e586c27dba86cc62dbfca4241ffac4759d`  
		Last Modified: Sat, 09 Dec 2017 04:04:56 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8680ea5a3773aca6085931ee70898ac8482f7cd4b96626323a25b98e94b000bd`  
		Last Modified: Sat, 09 Dec 2017 04:04:56 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8264f49536c3fca091723a00e869523b58a374538628ab48f97fcb554670069a`  
		Last Modified: Sat, 09 Dec 2017 04:05:30 GMT  
		Size: 4.1 MB (4144754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267ae5b0868476ceed2626b8a312a2afb7c6df18c50211cafffd06e79a90373a`  
		Last Modified: Sat, 09 Dec 2017 04:05:29 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3ff67841464baa59f0da45487476f1e380a4daab1e25a18d0bec7c7b51983c`  
		Last Modified: Sat, 09 Dec 2017 04:05:30 GMT  
		Size: 179.8 KB (179770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15daabca7eed67eef8265f58cacf6f5015ec37591a6a0ba88e67eb46d8be10eb`  
		Last Modified: Sat, 09 Dec 2017 04:05:31 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
