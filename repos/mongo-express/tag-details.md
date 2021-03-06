<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mongo-express`

-	[`mongo-express:0.31.5`](#mongo-express0315)
-	[`mongo-express:0.31`](#mongo-express031)
-	[`mongo-express:latest`](#mongo-expresslatest)

## `mongo-express:0.31.5`

```console
$ docker pull mongo-express@sha256:c3cf9c1a6b3abdfddd880b5b37b3cd6803d1c7e3d48352b44d310dd9bea5ffe9
```

-	Platforms:
	-	linux; amd64

### `mongo-express:0.31.5` - linux; amd64

-	Docker Version: 1.12.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100372613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c1d887d25bbc9710531cd63c91ea8735e86dcd0a13130d8fda445d194ff809`
-	Default Command: `["tini","--","node","app"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Nov 2016 21:16:06 GMT
RUN groupadd -r node && useradd -r -g node node
# Thu, 03 Nov 2016 21:16:17 GMT
RUN set -ex   && for key in     9554F04D7259F04124DE6B476D5A82AC7E37093B     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     0034A06D9D9B0064CE8ADF6BF1747F4AD2306D93     FD3A5288F042B6850C66B31F09FE44734EB7990E     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     B9AE9905FFD7803F25714661B63B535A4C206CA9     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   ; do     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";   done
# Thu, 03 Nov 2016 21:16:18 GMT
ENV NPM_CONFIG_LOGLEVEL=info
# Thu, 03 Nov 2016 21:16:49 GMT
ENV NODE_VERSION=6.9.1
# Thu, 03 Nov 2016 21:16:59 GMT
RUN buildDeps='xz-utils'     && set -x     && apt-get update && apt-get install -y $buildDeps --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.xz"     && curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-x64.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-x64.tar.xz" -C /usr/local --strip-components=1     && rm "node-v$NODE_VERSION-linux-x64.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-get purge -y --auto-remove $buildDeps     && ln -s /usr/local/bin/node /usr/local/bin/nodejs
# Thu, 03 Nov 2016 21:16:59 GMT
CMD ["node"]
# Thu, 03 Nov 2016 22:06:44 GMT
ENV TINI_VERSION=0.9.0
# Thu, 03 Nov 2016 22:06:53 GMT
RUN set -x 	&& apt-get update && apt-get install -y ca-certificates curl 		--no-install-recommends 	&& curl -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini" -o /usr/local/bin/tini 	&& curl -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini.asc" -o /usr/local/bin/tini.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h 	&& apt-get purge --auto-remove -y ca-certificates curl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Nov 2016 22:06:53 GMT
EXPOSE 8081/tcp
# Thu, 03 Nov 2016 22:06:54 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_SERVER=mongo ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Thu, 03 Nov 2016 22:06:54 GMT
ENV MONGO_EXPRESS=0.31.5
# Thu, 03 Nov 2016 22:07:17 GMT
RUN npm install mongo-express@$MONGO_EXPRESS
# Thu, 03 Nov 2016 22:07:18 GMT
WORKDIR /node_modules/mongo-express
# Thu, 03 Nov 2016 22:07:19 GMT
RUN cp config.default.js config.js
# Thu, 03 Nov 2016 22:07:19 GMT
CMD ["tini" "--" "node" "app"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af36d2c7a1481ae5554241fcb6bc20472bf7a6b7b2be24465c76e168c278a03f`  
		Last Modified: Fri, 21 Oct 2016 16:36:48 GMT  
		Size: 18.5 MB (18528131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5412f5d9f9eb3227f777ffa61fb72f00d7505c9d757a89dc3305c2c059ac75a1`  
		Last Modified: Thu, 03 Nov 2016 21:20:17 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23444aa04998ab9d995bb2faf9a3edf240b5a2d3b81eaa4686b53eb791779e42`  
		Last Modified: Thu, 03 Nov 2016 21:20:17 GMT  
		Size: 97.2 KB (97214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3a1af9e59fa2fdb263a741d053cfb6a6020a90f58209af7168b8850fa631bc`  
		Last Modified: Thu, 03 Nov 2016 21:24:18 GMT  
		Size: 14.0 MB (14026595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbd6f6e85e42aad48522333e6b23d0bc07862c729335c05be971eea30d622a3`  
		Last Modified: Thu, 03 Nov 2016 22:07:32 GMT  
		Size: 458.5 KB (458509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b6b91c04c74a4f99cc3cf763a2c1f8f7aee1d270d4bf79e03153748b480ccf`  
		Last Modified: Thu, 03 Nov 2016 22:07:35 GMT  
		Size: 15.9 MB (15904416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1521be05164f27a06e99ad2e1aa050c22414d236ca09b95bfb5d4e7f391ea97d`  
		Last Modified: Thu, 03 Nov 2016 22:07:31 GMT  
		Size: 2.6 KB (2576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo-express:0.31`

```console
$ docker pull mongo-express@sha256:c3cf9c1a6b3abdfddd880b5b37b3cd6803d1c7e3d48352b44d310dd9bea5ffe9
```

-	Platforms:
	-	linux; amd64

### `mongo-express:0.31` - linux; amd64

-	Docker Version: 1.12.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100372613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c1d887d25bbc9710531cd63c91ea8735e86dcd0a13130d8fda445d194ff809`
-	Default Command: `["tini","--","node","app"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Nov 2016 21:16:06 GMT
RUN groupadd -r node && useradd -r -g node node
# Thu, 03 Nov 2016 21:16:17 GMT
RUN set -ex   && for key in     9554F04D7259F04124DE6B476D5A82AC7E37093B     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     0034A06D9D9B0064CE8ADF6BF1747F4AD2306D93     FD3A5288F042B6850C66B31F09FE44734EB7990E     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     B9AE9905FFD7803F25714661B63B535A4C206CA9     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   ; do     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";   done
# Thu, 03 Nov 2016 21:16:18 GMT
ENV NPM_CONFIG_LOGLEVEL=info
# Thu, 03 Nov 2016 21:16:49 GMT
ENV NODE_VERSION=6.9.1
# Thu, 03 Nov 2016 21:16:59 GMT
RUN buildDeps='xz-utils'     && set -x     && apt-get update && apt-get install -y $buildDeps --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.xz"     && curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-x64.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-x64.tar.xz" -C /usr/local --strip-components=1     && rm "node-v$NODE_VERSION-linux-x64.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-get purge -y --auto-remove $buildDeps     && ln -s /usr/local/bin/node /usr/local/bin/nodejs
# Thu, 03 Nov 2016 21:16:59 GMT
CMD ["node"]
# Thu, 03 Nov 2016 22:06:44 GMT
ENV TINI_VERSION=0.9.0
# Thu, 03 Nov 2016 22:06:53 GMT
RUN set -x 	&& apt-get update && apt-get install -y ca-certificates curl 		--no-install-recommends 	&& curl -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini" -o /usr/local/bin/tini 	&& curl -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini.asc" -o /usr/local/bin/tini.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h 	&& apt-get purge --auto-remove -y ca-certificates curl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Nov 2016 22:06:53 GMT
EXPOSE 8081/tcp
# Thu, 03 Nov 2016 22:06:54 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_SERVER=mongo ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Thu, 03 Nov 2016 22:06:54 GMT
ENV MONGO_EXPRESS=0.31.5
# Thu, 03 Nov 2016 22:07:17 GMT
RUN npm install mongo-express@$MONGO_EXPRESS
# Thu, 03 Nov 2016 22:07:18 GMT
WORKDIR /node_modules/mongo-express
# Thu, 03 Nov 2016 22:07:19 GMT
RUN cp config.default.js config.js
# Thu, 03 Nov 2016 22:07:19 GMT
CMD ["tini" "--" "node" "app"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af36d2c7a1481ae5554241fcb6bc20472bf7a6b7b2be24465c76e168c278a03f`  
		Last Modified: Fri, 21 Oct 2016 16:36:48 GMT  
		Size: 18.5 MB (18528131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5412f5d9f9eb3227f777ffa61fb72f00d7505c9d757a89dc3305c2c059ac75a1`  
		Last Modified: Thu, 03 Nov 2016 21:20:17 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23444aa04998ab9d995bb2faf9a3edf240b5a2d3b81eaa4686b53eb791779e42`  
		Last Modified: Thu, 03 Nov 2016 21:20:17 GMT  
		Size: 97.2 KB (97214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3a1af9e59fa2fdb263a741d053cfb6a6020a90f58209af7168b8850fa631bc`  
		Last Modified: Thu, 03 Nov 2016 21:24:18 GMT  
		Size: 14.0 MB (14026595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbd6f6e85e42aad48522333e6b23d0bc07862c729335c05be971eea30d622a3`  
		Last Modified: Thu, 03 Nov 2016 22:07:32 GMT  
		Size: 458.5 KB (458509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b6b91c04c74a4f99cc3cf763a2c1f8f7aee1d270d4bf79e03153748b480ccf`  
		Last Modified: Thu, 03 Nov 2016 22:07:35 GMT  
		Size: 15.9 MB (15904416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1521be05164f27a06e99ad2e1aa050c22414d236ca09b95bfb5d4e7f391ea97d`  
		Last Modified: Thu, 03 Nov 2016 22:07:31 GMT  
		Size: 2.6 KB (2576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo-express:latest`

```console
$ docker pull mongo-express@sha256:c3cf9c1a6b3abdfddd880b5b37b3cd6803d1c7e3d48352b44d310dd9bea5ffe9
```

-	Platforms:
	-	linux; amd64

### `mongo-express:latest` - linux; amd64

-	Docker Version: 1.12.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100372613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c1d887d25bbc9710531cd63c91ea8735e86dcd0a13130d8fda445d194ff809`
-	Default Command: `["tini","--","node","app"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Nov 2016 21:16:06 GMT
RUN groupadd -r node && useradd -r -g node node
# Thu, 03 Nov 2016 21:16:17 GMT
RUN set -ex   && for key in     9554F04D7259F04124DE6B476D5A82AC7E37093B     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     0034A06D9D9B0064CE8ADF6BF1747F4AD2306D93     FD3A5288F042B6850C66B31F09FE44734EB7990E     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     B9AE9905FFD7803F25714661B63B535A4C206CA9     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   ; do     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key";   done
# Thu, 03 Nov 2016 21:16:18 GMT
ENV NPM_CONFIG_LOGLEVEL=info
# Thu, 03 Nov 2016 21:16:49 GMT
ENV NODE_VERSION=6.9.1
# Thu, 03 Nov 2016 21:16:59 GMT
RUN buildDeps='xz-utils'     && set -x     && apt-get update && apt-get install -y $buildDeps --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.xz"     && curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-x64.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-x64.tar.xz" -C /usr/local --strip-components=1     && rm "node-v$NODE_VERSION-linux-x64.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-get purge -y --auto-remove $buildDeps     && ln -s /usr/local/bin/node /usr/local/bin/nodejs
# Thu, 03 Nov 2016 21:16:59 GMT
CMD ["node"]
# Thu, 03 Nov 2016 22:06:44 GMT
ENV TINI_VERSION=0.9.0
# Thu, 03 Nov 2016 22:06:53 GMT
RUN set -x 	&& apt-get update && apt-get install -y ca-certificates curl 		--no-install-recommends 	&& curl -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini" -o /usr/local/bin/tini 	&& curl -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini.asc" -o /usr/local/bin/tini.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h 	&& apt-get purge --auto-remove -y ca-certificates curl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Nov 2016 22:06:53 GMT
EXPOSE 8081/tcp
# Thu, 03 Nov 2016 22:06:54 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_SERVER=mongo ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Thu, 03 Nov 2016 22:06:54 GMT
ENV MONGO_EXPRESS=0.31.5
# Thu, 03 Nov 2016 22:07:17 GMT
RUN npm install mongo-express@$MONGO_EXPRESS
# Thu, 03 Nov 2016 22:07:18 GMT
WORKDIR /node_modules/mongo-express
# Thu, 03 Nov 2016 22:07:19 GMT
RUN cp config.default.js config.js
# Thu, 03 Nov 2016 22:07:19 GMT
CMD ["tini" "--" "node" "app"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af36d2c7a1481ae5554241fcb6bc20472bf7a6b7b2be24465c76e168c278a03f`  
		Last Modified: Fri, 21 Oct 2016 16:36:48 GMT  
		Size: 18.5 MB (18528131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5412f5d9f9eb3227f777ffa61fb72f00d7505c9d757a89dc3305c2c059ac75a1`  
		Last Modified: Thu, 03 Nov 2016 21:20:17 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23444aa04998ab9d995bb2faf9a3edf240b5a2d3b81eaa4686b53eb791779e42`  
		Last Modified: Thu, 03 Nov 2016 21:20:17 GMT  
		Size: 97.2 KB (97214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3a1af9e59fa2fdb263a741d053cfb6a6020a90f58209af7168b8850fa631bc`  
		Last Modified: Thu, 03 Nov 2016 21:24:18 GMT  
		Size: 14.0 MB (14026595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbd6f6e85e42aad48522333e6b23d0bc07862c729335c05be971eea30d622a3`  
		Last Modified: Thu, 03 Nov 2016 22:07:32 GMT  
		Size: 458.5 KB (458509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b6b91c04c74a4f99cc3cf763a2c1f8f7aee1d270d4bf79e03153748b480ccf`  
		Last Modified: Thu, 03 Nov 2016 22:07:35 GMT  
		Size: 15.9 MB (15904416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1521be05164f27a06e99ad2e1aa050c22414d236ca09b95bfb5d4e7f391ea97d`  
		Last Modified: Thu, 03 Nov 2016 22:07:31 GMT  
		Size: 2.6 KB (2576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
