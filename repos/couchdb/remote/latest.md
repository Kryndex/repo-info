## `couchdb:latest`

```console
$ docker pull couchdb@sha256:206a6751dff9d32280f29798ddf73075fe2f7eca5b794e62ffeaf4921250682a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:3dc699ab70a0f00863d86bb9e340741ace7346295a9d53b7a9300a665534fcd7
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155318437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14a61c7297a58d700c46598bfdcba9fb573965fb438a4bbb59a60868e6e09adb`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:12 GMT
ADD file:1dd78a123212328bdc72ef7888024ea27fe141a72e24e0ea7c3c92b63b73d8d1 in / 
# Tue, 12 Dec 2017 01:41:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 03:58:13 GMT
MAINTAINER CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Dec 2017 03:58:14 GMT
RUN groupadd -r couchdb && useradd -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Dec 2017 03:58:51 GMT
RUN apt-get update -y && apt-get install -y --no-install-recommends     ca-certificates     curl     erlang-nox     erlang-reltool     haproxy     libicu52     libmozjs185-1.0     openssl   && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 03:58:52 GMT
ENV GOSU_VERSION=1.10
# Tue, 12 Dec 2017 03:58:52 GMT
ENV TINI_VERSION=0.16.1
# Tue, 12 Dec 2017 03:59:09 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini --version; 		apt-get purge -y --auto-remove wget
# Tue, 12 Dec 2017 03:59:09 GMT
ENV GPG_KEYS=15DD4F3B8AACA54740EB78C7B7B7C53943ECCEE1   1CFBFA43C19B6DF4A0CA3934669C02FFDF3CEBA3   25BBBAC113C1BFD5AA594A4C9F96B92930380381   4BFCA2B99BADC6F9F105BEC9C5E32E2D6B065BFB   5D680346FAA3E51B29DBCB681015F68F9DA248BC   7BCCEB868313DDA925DF1805ECA5BCB7BB9656B0   C3F4DFAEAD621E1C94523AEEC376457E61D50B88   D2B17F9DA23C0A10991AF2E3D9EE01E47852AEE4   E0AF0A194D55C84E4A19A801CDB0C0F904F4EE9B   29E4F38113DF707D722A6EF91FE9AF73118F1A7C   2EC788AE3F239FA13E82D215CDE711289384AE37
# Tue, 12 Dec 2017 03:59:17 GMT
RUN set -xe   && for key in $GPG_KEYS; do     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";   done
# Tue, 12 Dec 2017 03:59:18 GMT
ENV COUCHDB_VERSION=2.1.1
# Tue, 12 Dec 2017 04:00:07 GMT
RUN buildDeps='     apt-transport-https     gcc     g++     erlang-dev     libcurl4-openssl-dev     libicu-dev     libmozjs185-dev     make   '  && apt-get update -y -qq && apt-get install -y --no-install-recommends $buildDeps  && cd /usr/src && mkdir couchdb  && curl -fSL https://dist.apache.org/repos/dist/release/couchdb/source/$COUCHDB_VERSION/apache-couchdb-$COUCHDB_VERSION.tar.gz -o couchdb.tar.gz  && curl -fSL https://dist.apache.org/repos/dist/release/couchdb/source/$COUCHDB_VERSION/apache-couchdb-$COUCHDB_VERSION.tar.gz.asc -o couchdb.tar.gz.asc  && gpg --batch --verify couchdb.tar.gz.asc couchdb.tar.gz  && tar -xzf couchdb.tar.gz -C couchdb --strip-components=1  && cd couchdb  && ./configure --disable-docs  && make release  && mv /usr/src/couchdb/rel/couchdb /opt/  && apt-get purge -y --auto-remove $buildDeps  && rm -rf /var/lib/apt/lists/* /usr/src/couchdb*  && mkdir /opt/couchdb/data  && chown -R couchdb:couchdb /opt/couchdb
# Tue, 12 Dec 2017 04:00:09 GMT
COPY file:6e48edd87a901be3cfaa928bf5b42264b4e3173d6c817b46878bf1104dcff208 in /opt/couchdb/etc/local.d/ 
# Tue, 12 Dec 2017 04:00:10 GMT
COPY file:92f7c74ebcdab3f422f19b237777e707346b0b921cecac100009f5e1e9918e1e in /opt/couchdb/etc/ 
# Tue, 12 Dec 2017 04:00:10 GMT
COPY file:4b6c87a451132457c240370120ddfb8a03af930f0acadd3c8522f18f4c9b7398 in / 
# Tue, 12 Dec 2017 04:00:11 GMT
RUN chown -R couchdb:couchdb /opt/couchdb/etc/local.d/ /opt/couchdb/etc/vm.args
# Tue, 12 Dec 2017 04:00:11 GMT
WORKDIR /opt/couchdb
# Tue, 12 Dec 2017 04:00:12 GMT
EXPOSE 4369/tcp 5984/tcp 9100/tcp
# Tue, 12 Dec 2017 04:00:12 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Dec 2017 04:00:12 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Dec 2017 04:00:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f49cf87b52c10aa83b4f4405800527a74400fb19ea1821d209293bc4d53966aa`  
		Last Modified: Tue, 12 Dec 2017 01:47:59 GMT  
		Size: 52.6 MB (52599697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9284d607ae1f1952737bd0382f22467feaf15dafd3559158cc06b859b70bc71`  
		Last Modified: Tue, 12 Dec 2017 04:05:47 GMT  
		Size: 2.1 KB (2095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8483f21dc053a8edc8b66905180a4b12f6f6b2e6470008c41d4938b214ffd4b8`  
		Last Modified: Tue, 12 Dec 2017 04:06:04 GMT  
		Size: 84.1 MB (84067222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d505642a572cca7d72ec103c1f5d7dbf8af282cb0b9671563ad7350304893f4`  
		Last Modified: Tue, 12 Dec 2017 04:05:47 GMT  
		Size: 912.7 KB (912688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4076ba45b00c9a7318950701d681e45bd40cb1373b14d6bc6346c1651ed954`  
		Last Modified: Tue, 12 Dec 2017 04:05:46 GMT  
		Size: 527.9 KB (527925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bafa08556562b02aa26a6d9fe11cbdff1e21b120d8151cf3e58cba4897e25b`  
		Last Modified: Tue, 12 Dec 2017 04:05:46 GMT  
		Size: 17.2 MB (17205304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34152bda1b2ddbd4e5341791b78509b5acfd391c539a1e9f12fe864cf6fd2201`  
		Last Modified: Tue, 12 Dec 2017 04:05:43 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423bb4ba2bcf47fa60abb6d3c16975f6bca21c762b43733330f6f54c1386d8c0`  
		Last Modified: Tue, 12 Dec 2017 04:05:44 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a773d24865299cf5adf9de359bec4286d81b2c162bca1342aa2e978f2500c7`  
		Last Modified: Tue, 12 Dec 2017 04:05:43 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d18033b225c552c1f31f6a5c877a903d2c15708807d3dcef89cf389754fc1ae`  
		Last Modified: Tue, 12 Dec 2017 04:05:45 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
