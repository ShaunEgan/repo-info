## `couchdb:1-couchperuser`

```console
$ docker pull couchdb@sha256:218582c069f16eac84332f0f7404f9582f0acae02fdf1f49adee8f5293f40ab8
```

-	Platforms:
	-	linux; amd64

### `couchdb:1-couchperuser` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113866431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0201d8325f46ade7fce5b4d5daf53407877aa6299c9324e7d00d3b09aada47ea`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["couchdb"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 17:02:12 GMT
MAINTAINER Clemens Stolle klaemo@apache.org
# Fri, 21 Oct 2016 17:02:13 GMT
RUN groupadd -r couchdb && useradd -d /var/lib/couchdb -g couchdb couchdb
# Fri, 21 Oct 2016 17:09:39 GMT
RUN apt-get update -y && apt-get install -y --no-install-recommends     ca-certificates     curl     erlang-nox     libicu52     libmozjs185-1.0     libnspr4     libnspr4-0d   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 17:09:47 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/1.7/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/1.7/gosu-$(dpkg --print-architecture).asc"   && gpg --verify /usr/local/bin/gosu.asc   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v0.9.0/tini"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v0.9.0/tini.asc"   && gpg --verify /usr/local/bin/tini.asc   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini
# Fri, 21 Oct 2016 17:09:47 GMT
ENV GPG_KEYS=15DD4F3B8AACA54740EB78C7B7B7C53943ECCEE1   1CFBFA43C19B6DF4A0CA3934669C02FFDF3CEBA3   25BBBAC113C1BFD5AA594A4C9F96B92930380381   4BFCA2B99BADC6F9F105BEC9C5E32E2D6B065BFB   5D680346FAA3E51B29DBCB681015F68F9DA248BC   7BCCEB868313DDA925DF1805ECA5BCB7BB9656B0   C3F4DFAEAD621E1C94523AEEC376457E61D50B88   D2B17F9DA23C0A10991AF2E3D9EE01E47852AEE4   E0AF0A194D55C84E4A19A801CDB0C0F904F4EE9B
# Fri, 21 Oct 2016 17:09:56 GMT
RUN set -xe   && for key in $GPG_KEYS; do     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";   done
# Fri, 21 Oct 2016 17:09:56 GMT
ENV COUCHDB_VERSION=1.6.1
# Fri, 21 Oct 2016 17:10:55 GMT
RUN buildDeps='     gcc     g++     erlang-dev     libcurl4-openssl-dev     libicu-dev     libmozjs185-dev     libnspr4-dev     make   '   && apt-get update && apt-get install -y --no-install-recommends $buildDeps   && curl -fSL http://apache.osuosl.org/couchdb/source/$COUCHDB_VERSION/apache-couchdb-$COUCHDB_VERSION.tar.gz -o couchdb.tar.gz   && curl -fSL https://www.apache.org/dist/couchdb/source/$COUCHDB_VERSION/apache-couchdb-$COUCHDB_VERSION.tar.gz.asc -o couchdb.tar.gz.asc   && gpg --verify couchdb.tar.gz.asc   && mkdir -p /usr/src/couchdb   && tar -xzf couchdb.tar.gz -C /usr/src/couchdb --strip-components=1   && cd /usr/src/couchdb   && ./configure --with-js-lib=/usr/lib --with-js-include=/usr/include/mozjs   && make && make install   && apt-get purge -y --auto-remove $buildDeps   && rm -rf /var/lib/apt/lists/* /usr/src/couchdb /couchdb.tar.gz*   && chown -R couchdb:couchdb     /usr/local/lib/couchdb /usr/local/etc/couchdb     /usr/local/var/lib/couchdb /usr/local/var/log/couchdb /usr/local/var/run/couchdb   && chmod -R g+rw     /usr/local/lib/couchdb /usr/local/etc/couchdb     /usr/local/var/lib/couchdb /usr/local/var/log/couchdb /usr/local/var/run/couchdb   && mkdir -p /var/lib/couchdb   && sed -e 's/^bind_address = .*$/bind_address = 0.0.0.0/' -i /usr/local/etc/couchdb/default.ini   && sed -e 's!/usr/local/var/log/couchdb/couch.log$!/dev/null!' -i /usr/local/etc/couchdb/default.ini
# Fri, 21 Oct 2016 17:10:56 GMT
COPY file:9167181556794bc11f93a378f69052e0de980ac17e33be172c375a8564bbe89a in / 
# Fri, 21 Oct 2016 17:10:56 GMT
RUN chmod +x /docker-entrypoint.sh
# Fri, 21 Oct 2016 17:10:57 GMT
VOLUME [/usr/local/var/lib/couchdb]
# Fri, 21 Oct 2016 17:10:57 GMT
EXPOSE 5984/tcp
# Fri, 21 Oct 2016 17:10:57 GMT
WORKDIR /var/lib/couchdb
# Fri, 21 Oct 2016 17:10:57 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 21 Oct 2016 17:10:58 GMT
CMD ["couchdb"]
# Fri, 21 Oct 2016 17:11:56 GMT
MAINTAINER Clemens Stolle klaemo@apache.org
# Fri, 21 Oct 2016 17:11:57 GMT
ENV COUCHPERUSER_SHA=5d28db3272eea9619d4391b33aae6030f0319ecc54aa2a2f2b6c6a8d448f03f2
# Fri, 21 Oct 2016 17:12:21 GMT
RUN apt-get update && apt-get install -y rebar make  && mkdir -p /usr/local/lib/couchdb/plugins/couchperuser  && cd /usr/local/lib/couchdb/plugins  && curl -L -o couchperuser.tar.gz https://github.com/etrepum/couchperuser/archive/1.1.0.tar.gz  && echo "$COUCHPERUSER_SHA *couchperuser.tar.gz" | sha256sum -c -  && tar -xzf couchperuser.tar.gz -C couchperuser --strip-components=1  && rm couchperuser.tar.gz  && cd couchperuser  && make  && apt-get purge -y --auto-remove rebar make
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ac1c1d29ec68348fa2a569f2667f84bd8cc6f7758ac0e1e82c82c0a9100527`  
		Last Modified: Fri, 21 Oct 2016 17:11:11 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31dd814bb5e7621a96e26cb90661270f1688d503b3056592975d7e941932ced7`  
		Last Modified: Fri, 21 Oct 2016 17:11:16 GMT  
		Size: 42.7 MB (42671780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2c9b85eff0ddfbecd3a7f3a581ada60bc8c209191f92517f159ec65ac7fa92`  
		Last Modified: Fri, 21 Oct 2016 17:11:08 GMT  
		Size: 948.7 KB (948697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763d7be281defebd96aa9f92bcd1b8ce763e5e643d42062f3048d85c47e5791f`  
		Last Modified: Fri, 21 Oct 2016 17:11:08 GMT  
		Size: 631.4 KB (631407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df77e55e34f05898a0c8cb54e8d4b79238362d57f984e18157fa770d0cea119`  
		Last Modified: Fri, 21 Oct 2016 17:11:09 GMT  
		Size: 8.2 MB (8177763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66511df40a2dd088b263a744bf3c91182db2e0fa4752ff08d2c79be60ae3c562`  
		Last Modified: Fri, 21 Oct 2016 17:11:07 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66511df40a2dd088b263a744bf3c91182db2e0fa4752ff08d2c79be60ae3c562`  
		Last Modified: Fri, 21 Oct 2016 17:11:07 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b69ebef93c847176f0e5b01337777b256a6e7ff4a2d41aa1a84c3bd0a1b441f`  
		Last Modified: Fri, 21 Oct 2016 17:12:32 GMT  
		Size: 10.1 MB (10079505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
