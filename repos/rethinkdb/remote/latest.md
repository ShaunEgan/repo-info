## `rethinkdb:latest`

```console
$ docker pull rethinkdb@sha256:0340626552c50d0852e9a31901d984c390f2a9704fbbc8ad53ebca66c261422d
```

-	Platforms:
	-	linux; amd64

### `rethinkdb:latest` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75958211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98772db29d5646f0a61c7f2b5c7ff69868531ff03ec44913a456d4d9fb756f39`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Oct 2016 01:07:59 GMT
MAINTAINER Daniel Alan Miller <dalanmiller@rethinkdb.com>
# Sat, 22 Oct 2016 01:08:00 GMT
RUN apt-key adv --keyserver pgp.mit.edu --recv-keys 1614552E5765227AEC39EFCFA7E00EF33A8F2399
# Sat, 22 Oct 2016 01:08:01 GMT
RUN echo "deb http://download.rethinkdb.com/apt jessie main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 22 Oct 2016 01:08:01 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.3.5~0jessie
# Sat, 22 Oct 2016 01:08:14 GMT
RUN apt-get update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 22 Oct 2016 01:08:14 GMT
VOLUME [/data]
# Sat, 22 Oct 2016 01:08:15 GMT
WORKDIR /data
# Sat, 22 Oct 2016 01:08:15 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 22 Oct 2016 01:08:16 GMT
EXPOSE 28015/tcp 29015/tcp 8080/tcp
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92968af165ab71a60d456ebb40c124659156768bf4f85cd394e50c07cb56c09`  
		Last Modified: Sat, 22 Oct 2016 01:08:25 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009d33162daab21f5a035889a0fbba135682116f4dcb98bf786a88d134f3e476`  
		Last Modified: Sat, 22 Oct 2016 01:08:26 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166c9b6f44287dbbbd746695c20877d5e8fcaba64d63006fe4f698053d5affa7`  
		Last Modified: Sat, 22 Oct 2016 01:08:32 GMT  
		Size: 24.6 MB (24603338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b021ff45110d1ef89e27a01a2f60f2dec0358814a785ab498d49408980b289a`  
		Last Modified: Sat, 22 Oct 2016 01:08:27 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
