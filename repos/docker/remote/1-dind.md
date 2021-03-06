## `docker:1-dind`

```console
$ docker pull docker@sha256:8ba6e1b37a6346712f48efbaca1db050f7d5fe48f279f889200dbf341e1f9f1a
```

-	Platforms:
	-	linux; amd64

### `docker:1-dind` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34060068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5134947104f48e7f59019022166fd497c4227dbd8e634f97c0455b01eaf26705`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 23:04:45 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		openssl
# Tue, 18 Oct 2016 23:04:50 GMT
ENV DOCKER_BUCKET=get.docker.com
# Mon, 31 Oct 2016 21:46:15 GMT
ENV DOCKER_VERSION=1.12.3
# Mon, 31 Oct 2016 21:46:16 GMT
ENV DOCKER_SHA256=626601deb41d9706ac98da23f673af6c0d4631c4d194a677a9a1a07d7219fa0f
# Mon, 31 Oct 2016 21:46:19 GMT
RUN set -x 	&& curl -fSL "https://${DOCKER_BUCKET}/builds/Linux/x86_64/docker-${DOCKER_VERSION}.tgz" -o docker.tgz 	&& echo "${DOCKER_SHA256} *docker.tgz" | sha256sum -c - 	&& tar -xzvf docker.tgz 	&& mv docker/* /usr/local/bin/ 	&& rmdir docker 	&& rm docker.tgz 	&& docker -v
# Mon, 31 Oct 2016 21:46:20 GMT
COPY file:399605dc1850a60a586b5494ab538bad495fd6f94eabca0c5f8a26468ce6030f in /usr/local/bin/ 
# Mon, 31 Oct 2016 21:46:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 31 Oct 2016 21:46:21 GMT
CMD ["sh"]
# Mon, 31 Oct 2016 21:46:24 GMT
RUN apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		xfsprogs 		xz
# Mon, 31 Oct 2016 21:46:25 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 31 Oct 2016 21:46:25 GMT
ENV DIND_COMMIT=3b5fac462d21ca164b3778647420016315289034
# Mon, 31 Oct 2016 21:46:27 GMT
RUN wget "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind" -O /usr/local/bin/dind 	&& chmod +x /usr/local/bin/dind
# Mon, 31 Oct 2016 21:46:27 GMT
COPY file:0e53f84aca37cd3eaaea6a6908834cca20af731890838b17e6b13fc6f34c20b3 in /usr/local/bin/ 
# Mon, 31 Oct 2016 21:46:27 GMT
VOLUME [/var/lib/docker]
# Mon, 31 Oct 2016 21:46:28 GMT
EXPOSE 2375/tcp
# Mon, 31 Oct 2016 21:46:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 31 Oct 2016 21:46:28 GMT
CMD []
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7601c2ad1cd11213e66512af4a8f4372a4870541b8cf79a9a1058742bf65d6e7`  
		Last Modified: Tue, 18 Oct 2016 23:05:10 GMT  
		Size: 915.1 KB (915061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fa41e1947e55748e6bb64fdc8decb92de95bf1f7f69c9da3ed022983953a9f`  
		Last Modified: Mon, 31 Oct 2016 21:47:12 GMT  
		Size: 28.8 MB (28762821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee74a896d835287baba1aa769cdc88ec2b48879aabd9e1bfb3382de803495d0`  
		Last Modified: Mon, 31 Oct 2016 21:47:01 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11479d6bb0f194261893a7d056b26fccc0e01b04a48ef0fdb39b2d2ec9be9c1e`  
		Last Modified: Mon, 31 Oct 2016 21:48:06 GMT  
		Size: 2.1 MB (2065103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f107233cbdd9b6541d37d4b2647321fa1495059dc20e36658b12ee3e8b7465`  
		Last Modified: Mon, 31 Oct 2016 21:48:03 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584f95c052d8c439bae53c986077e74c8f5e3cce36a5faadcccd30aef5beebd9`  
		Last Modified: Mon, 31 Oct 2016 21:48:03 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5d0f77d68c4332363b9e1171c9a1c5ba397da553c7b26589aa378506e76d89`  
		Last Modified: Mon, 31 Oct 2016 21:48:03 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
