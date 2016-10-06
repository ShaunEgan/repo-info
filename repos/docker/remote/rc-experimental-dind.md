## `docker:rc-experimental-dind`

```console
$ docker pull docker@sha256:10da5d1c1245e47f9407ce0ad4af6b10bfd5e04c24d67c6d7b052b3b45ac9e6d
```

-	Platforms:
	-	linux; amd64

### `docker:rc-experimental-dind` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34183493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbf441400eea7ce17c3994d01941d37177607c43cabb1054e38650d3dbc3500c`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 23 Sep 2016 16:29:57 GMT
ADD file:d6ee3ba7a4d59b161917082cc7242c660c61bb3f3cc1549c7e2dfff2b0de7104 in / 
# Fri, 23 Sep 2016 16:36:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		openssl
# Fri, 23 Sep 2016 16:38:38 GMT
ENV DOCKER_BUCKET=experimental.docker.com
# Wed, 05 Oct 2016 20:21:15 GMT
ENV DOCKER_VERSION=1.12.2-rc2
# Wed, 05 Oct 2016 20:21:16 GMT
ENV DOCKER_SHA256=61758c2d92d8e4a3c39ad8c0766c4ae2de76da8814d7986efdb9483ba35d934e
# Wed, 05 Oct 2016 20:21:23 GMT
RUN set -x 	&& curl -fSL "https://${DOCKER_BUCKET}/builds/Linux/x86_64/docker-${DOCKER_VERSION}.tgz" -o docker.tgz 	&& echo "${DOCKER_SHA256} *docker.tgz" | sha256sum -c - 	&& tar -xzvf docker.tgz 	&& mv docker/* /usr/local/bin/ 	&& rmdir docker 	&& rm docker.tgz 	&& docker -v
# Wed, 05 Oct 2016 20:21:23 GMT
COPY file:50006c902e7677711aeffe4ab7b7042d649618b96dec760f322a8566dd83ab25 in /usr/local/bin/ 
# Wed, 05 Oct 2016 20:21:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2016 20:21:24 GMT
CMD ["sh"]
# Wed, 05 Oct 2016 20:21:27 GMT
RUN apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		xfsprogs 		xz
# Wed, 05 Oct 2016 20:21:28 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 05 Oct 2016 20:21:28 GMT
ENV DIND_COMMIT=3b5fac462d21ca164b3778647420016315289034
# Wed, 05 Oct 2016 20:21:29 GMT
RUN wget "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind" -O /usr/local/bin/dind 	&& chmod +x /usr/local/bin/dind
# Wed, 05 Oct 2016 20:21:29 GMT
COPY file:a00ae81495fdf69e63bb25e3b665aa29cb53cfe5788e6134adfc0f35caff6295 in /usr/local/bin/ 
# Wed, 05 Oct 2016 20:21:29 GMT
VOLUME [/var/lib/docker]
# Wed, 05 Oct 2016 20:21:30 GMT
EXPOSE 2375/tcp
# Wed, 05 Oct 2016 20:21:30 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 05 Oct 2016 20:21:30 GMT
CMD []
```

-	Layers:
	-	`sha256:c0cb142e43453ebb1f82b905aa472e6e66017efd43872135bc5372e4fac04031`  
		Last Modified: Fri, 23 Sep 2016 16:30:54 GMT  
		Size: 2.3 MB (2312930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6fe447e877c6fb78f7040d59f81a9aaac5be90ed3f7396a6dfd9aaa3467d29`  
		Last Modified: Fri, 23 Sep 2016 16:37:07 GMT  
		Size: 915.0 KB (915035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fc6cf58f61b7586eb5fecc8653183645164dbd9a8fa04b60362dc74a7fb6ff`  
		Last Modified: Wed, 05 Oct 2016 20:23:56 GMT  
		Size: 28.9 MB (28886446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5565862d4f659d1b49d3c7202b080a10be7ee53a240766ca3674c15caab4cbaa`  
		Last Modified: Wed, 05 Oct 2016 20:23:46 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb30c8d8bd864e4195b12f8cb821da9b09565d9dc34427c395c055db7c2b564f`  
		Last Modified: Wed, 05 Oct 2016 20:24:36 GMT  
		Size: 2.1 MB (2065038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07a0ddb174f5a52748e9088eb8b90bbf0ace79e7519391b0114bfba2d49c4c9`  
		Last Modified: Wed, 05 Oct 2016 20:24:36 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830d8dd2a5ed69bff591e06f8a5bc13f2a5acb790eb5dfcf593840f58cb66f81`  
		Last Modified: Wed, 05 Oct 2016 20:24:36 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e8381963a81a52a1a4fb4d996a772e1f42c1ae206734154eb0ebfead4e3a88`  
		Last Modified: Wed, 05 Oct 2016 20:24:35 GMT  
		Size: 439.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip