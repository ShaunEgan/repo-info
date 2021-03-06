## `consul:latest`

```console
$ docker pull consul@sha256:ec93240d7f4e298094c0a301ab8d25e8f48e049602deb7f6e8de695c3d6bf4cb
```

-	Platforms:
	-	linux; amd64

### `consul:latest` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10609069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba9010ee3cc0251be45e8b55f3154eb421df841cd93a375f9f5ab334d848291`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 22:59:33 GMT
MAINTAINER James Phillips <james@hashicorp.com> (@slackpad)
# Tue, 18 Oct 2016 22:59:34 GMT
ENV CONSUL_VERSION=0.7.0
# Tue, 18 Oct 2016 22:59:34 GMT
ENV DOCKER_BASE_VERSION=0.0.4
# Tue, 18 Oct 2016 22:59:36 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 18 Oct 2016 22:59:54 GMT
RUN apk add --no-cache ca-certificates curl gnupg libcap openssl &&     gpg --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/docker-base/${DOCKER_BASE_VERSION}/docker-base_${DOCKER_BASE_VERSION}_linux_amd64.zip &&     wget https://releases.hashicorp.com/docker-base/${DOCKER_BASE_VERSION}/docker-base_${DOCKER_BASE_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/docker-base/${DOCKER_BASE_VERSION}/docker-base_${DOCKER_BASE_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify docker-base_${DOCKER_BASE_VERSION}_SHA256SUMS.sig docker-base_${DOCKER_BASE_VERSION}_SHA256SUMS &&     grep ${DOCKER_BASE_VERSION}_linux_amd64.zip docker-base_${DOCKER_BASE_VERSION}_SHA256SUMS | sha256sum -c &&     unzip docker-base_${DOCKER_BASE_VERSION}_linux_amd64.zip &&     cp bin/gosu bin/dumb-init /bin &&     wget https://releases.hashicorp.com/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_amd64.zip &&     wget https://releases.hashicorp.com/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_amd64.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_amd64.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 18 Oct 2016 22:59:55 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 18 Oct 2016 22:59:55 GMT
VOLUME [/consul/data]
# Tue, 18 Oct 2016 22:59:56 GMT
EXPOSE 8300/tcp
# Tue, 18 Oct 2016 22:59:56 GMT
EXPOSE 8301/tcp 8301/udp 8302/tcp 8302/udp
# Tue, 18 Oct 2016 22:59:57 GMT
EXPOSE 8400/tcp 8500/tcp 8600/tcp 8600/udp
# Tue, 18 Oct 2016 22:59:57 GMT
COPY file:6676f27da0116d8c6c0d4e60a1f3dd6bde44a4b14dc65edbe174cb907dc16353 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 18 Oct 2016 22:59:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Oct 2016 22:59:58 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d87316f35bf9de06908a0fe37db4f19d26c88dacfe88e4cbd2f4deb9e773d0`  
		Last Modified: Tue, 18 Oct 2016 23:00:08 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73b3349c8d07426a442db0ed3e6c2b64acf583a2251fe4665310e9e23139eac`  
		Last Modified: Tue, 18 Oct 2016 23:00:10 GMT  
		Size: 8.3 MB (8293081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79224170bcc928231e866fd9a9f24ba918a997a61bc0f52426f9024c9df5204b`  
		Last Modified: Tue, 18 Oct 2016 23:00:10 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7271d0bfc8ef385a69f7ab5e05d7ec0defb59cf360acee6a4f1e492e49f6ec`  
		Last Modified: Tue, 18 Oct 2016 23:00:07 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
