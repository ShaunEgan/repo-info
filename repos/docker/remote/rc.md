## `docker:rc`

```console
$ docker pull docker@sha256:68d9f91377e11849041fe895da601a8475f5ffd01d0b4c596386d60bf22016a4
```

-	Platforms:
	-	linux; amd64

### `docker:rc` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31975844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7159678f1d35eacd14bb42d68a9c92c9f75a23eb94156ac41add7bdcbb5e89ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 23 Sep 2016 16:29:57 GMT
ADD file:d6ee3ba7a4d59b161917082cc7242c660c61bb3f3cc1549c7e2dfff2b0de7104 in / 
# Fri, 23 Sep 2016 16:36:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		openssl
# Wed, 28 Sep 2016 20:49:07 GMT
ENV DOCKER_BUCKET=test.docker.com
# Wed, 05 Oct 2016 20:21:01 GMT
ENV DOCKER_VERSION=1.12.2-rc2
# Wed, 05 Oct 2016 20:21:01 GMT
ENV DOCKER_SHA256=dde4b9f3142a9ba38f95a58ea0005b40a3da9e8c5c8f7fe35710be3c71c6ff6b
# Wed, 05 Oct 2016 20:21:05 GMT
RUN set -x 	&& curl -fSL "https://${DOCKER_BUCKET}/builds/Linux/x86_64/docker-${DOCKER_VERSION}.tgz" -o docker.tgz 	&& echo "${DOCKER_SHA256} *docker.tgz" | sha256sum -c - 	&& tar -xzvf docker.tgz 	&& mv docker/* /usr/local/bin/ 	&& rmdir docker 	&& rm docker.tgz 	&& docker -v
# Wed, 05 Oct 2016 20:21:05 GMT
COPY file:50006c902e7677711aeffe4ab7b7042d649618b96dec760f322a8566dd83ab25 in /usr/local/bin/ 
# Wed, 05 Oct 2016 20:21:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2016 20:21:06 GMT
CMD ["sh"]
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
	-	`sha256:64debd848a6e8b0bb7df8c97f4b0fc6828e329ab6c281643cba7c67cc417dcf7`  
		Last Modified: Wed, 05 Oct 2016 20:21:54 GMT  
		Size: 28.7 MB (28747414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3563e2beb703e271ec1808a497fbb010f4d6c6bea48291566cf6b841444b4ea4`  
		Last Modified: Wed, 05 Oct 2016 20:21:42 GMT  
		Size: 465.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip