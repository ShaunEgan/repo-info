<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:4.1.11`](#kibana4111)
-	[`kibana:4.1`](#kibana41)
-	[`kibana:4.2.2`](#kibana422)
-	[`kibana:4.2`](#kibana42)
-	[`kibana:4.3.3`](#kibana433)
-	[`kibana:4.3`](#kibana43)
-	[`kibana:4.4.2`](#kibana442)
-	[`kibana:4.4`](#kibana44)
-	[`kibana:4.5.4`](#kibana454)
-	[`kibana:4.5`](#kibana45)
-	[`kibana:4.6.2`](#kibana462)
-	[`kibana:4.6`](#kibana46)
-	[`kibana:4`](#kibana4)
-	[`kibana:5.0.0`](#kibana500)
-	[`kibana:5.0`](#kibana50)
-	[`kibana:5`](#kibana5)
-	[`kibana:latest`](#kibanalatest)

## `kibana:4.1.11`

```console
$ docker pull kibana@sha256:da2fc119939ef95e203838402287805b3aa847cd687d173d4136e04d6206f545
```

-	Platforms:
	-	linux; amd64

### `kibana:4.1.11` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87788529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0a4c85a8ebcca06850401b7270f25c882c6993b693b0b41905dd6dff69a86b4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:24:51 GMT
RUN apt-get update && apt-get install -y 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:24:52 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:24:57 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:24:57 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:25:00 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:26:26 GMT
ENV KIBANA_VERSION=4.1.11
# Fri, 21 Oct 2016 20:26:26 GMT
ENV KIBANA_SHA1=13655cf94f5c47e8ab4d94c8170128f63be46ad5
# Fri, 21 Oct 2016 20:26:33 GMT
RUN set -x 	&& wget -O kibana.tar.gz "https://download.elastic.co/kibana/kibana/kibana-${KIBANA_VERSION}-linux-x64.tar.gz" 	&& echo "${KIBANA_SHA1} *kibana.tar.gz" | sha1sum -c - 	&& mkdir -p /opt/kibana 	&& tar -xz --strip-components=1 -C /opt/kibana -f kibana.tar.gz 	&& chown -R kibana:kibana /opt/kibana 	&& rm kibana.tar.gz 		&& sed -ri "s!^(\#\s*)?(elasticsearch_url:).*!\2 'http://elasticsearch:9200'!" /opt/kibana/config/kibana.yml 	&& grep -q 'elasticsearch:9200' /opt/kibana/config/kibana.yml
# Fri, 21 Oct 2016 20:26:33 GMT
ENV PATH=/opt/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 20:26:34 GMT
COPY file:1ad4c14d23fc99eff1a91bced98f992e275b430cc6f63f5ad27bf5e6b929be00 in / 
# Fri, 21 Oct 2016 20:26:34 GMT
EXPOSE 5601/tcp
# Fri, 21 Oct 2016 20:26:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Oct 2016 20:26:35 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f949e3abf8f4ec8b1211b1869fe813836de1919804b13d75c4c8b2f6cda52f`  
		Last Modified: Fri, 21 Oct 2016 20:25:40 GMT  
		Size: 16.6 MB (16609616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8576c69186a82a15156cac702a0f773a50ac0c5c78bda4ba2e4c24adad3d`  
		Last Modified: Fri, 21 Oct 2016 20:25:36 GMT  
		Size: 807.9 KB (807935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc26209b04278303b61ce61c61aba5181e98d76361afe71ddbda3e88d17ce59e`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 7.1 KB (7122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5862f5b8751568dab8a93bf13908d9f0b639fd1569dcb907f362f8880adbe8b`  
		Last Modified: Fri, 21 Oct 2016 20:26:50 GMT  
		Size: 19.0 MB (19006044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b1a7ec3a10051b9357a65ebbe5087a452b1bcf126ec453873bef33d156dbc4`  
		Last Modified: Fri, 21 Oct 2016 20:26:44 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:4.1`

```console
$ docker pull kibana@sha256:da2fc119939ef95e203838402287805b3aa847cd687d173d4136e04d6206f545
```

-	Platforms:
	-	linux; amd64

### `kibana:4.1` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87788529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0a4c85a8ebcca06850401b7270f25c882c6993b693b0b41905dd6dff69a86b4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:24:51 GMT
RUN apt-get update && apt-get install -y 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:24:52 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:24:57 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:24:57 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:25:00 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:26:26 GMT
ENV KIBANA_VERSION=4.1.11
# Fri, 21 Oct 2016 20:26:26 GMT
ENV KIBANA_SHA1=13655cf94f5c47e8ab4d94c8170128f63be46ad5
# Fri, 21 Oct 2016 20:26:33 GMT
RUN set -x 	&& wget -O kibana.tar.gz "https://download.elastic.co/kibana/kibana/kibana-${KIBANA_VERSION}-linux-x64.tar.gz" 	&& echo "${KIBANA_SHA1} *kibana.tar.gz" | sha1sum -c - 	&& mkdir -p /opt/kibana 	&& tar -xz --strip-components=1 -C /opt/kibana -f kibana.tar.gz 	&& chown -R kibana:kibana /opt/kibana 	&& rm kibana.tar.gz 		&& sed -ri "s!^(\#\s*)?(elasticsearch_url:).*!\2 'http://elasticsearch:9200'!" /opt/kibana/config/kibana.yml 	&& grep -q 'elasticsearch:9200' /opt/kibana/config/kibana.yml
# Fri, 21 Oct 2016 20:26:33 GMT
ENV PATH=/opt/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 20:26:34 GMT
COPY file:1ad4c14d23fc99eff1a91bced98f992e275b430cc6f63f5ad27bf5e6b929be00 in / 
# Fri, 21 Oct 2016 20:26:34 GMT
EXPOSE 5601/tcp
# Fri, 21 Oct 2016 20:26:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Oct 2016 20:26:35 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f949e3abf8f4ec8b1211b1869fe813836de1919804b13d75c4c8b2f6cda52f`  
		Last Modified: Fri, 21 Oct 2016 20:25:40 GMT  
		Size: 16.6 MB (16609616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8576c69186a82a15156cac702a0f773a50ac0c5c78bda4ba2e4c24adad3d`  
		Last Modified: Fri, 21 Oct 2016 20:25:36 GMT  
		Size: 807.9 KB (807935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc26209b04278303b61ce61c61aba5181e98d76361afe71ddbda3e88d17ce59e`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 7.1 KB (7122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5862f5b8751568dab8a93bf13908d9f0b639fd1569dcb907f362f8880adbe8b`  
		Last Modified: Fri, 21 Oct 2016 20:26:50 GMT  
		Size: 19.0 MB (19006044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b1a7ec3a10051b9357a65ebbe5087a452b1bcf126ec453873bef33d156dbc4`  
		Last Modified: Fri, 21 Oct 2016 20:26:44 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:4.2.2`

```console
$ docker pull kibana@sha256:e8d265c1cd184ed0e58669d9bdc6a2222775334e89ce7dcbe4c4e31f1d99993b
```

-	Platforms:
	-	linux; amd64

### `kibana:4.2.2` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.3 MB (99283175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71cda438405047fcfa05b6c04c2853fcff8c8d52fd99a6bbc517c04e46748395`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:24:51 GMT
RUN apt-get update && apt-get install -y 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:24:52 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:24:57 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:24:57 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:25:00 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:27:12 GMT
ENV KIBANA_VERSION=4.2.2
# Fri, 21 Oct 2016 20:27:12 GMT
ENV KIBANA_SHA1=f0daf9cd0b949c0ec7a3be300ee876fba17d1570
# Fri, 21 Oct 2016 20:27:22 GMT
RUN set -x 	&& wget -O kibana.tar.gz "https://download.elastic.co/kibana/kibana/kibana-${KIBANA_VERSION}-linux-x64.tar.gz" 	&& echo "${KIBANA_SHA1} *kibana.tar.gz" | sha1sum -c - 	&& mkdir -p /opt/kibana 	&& tar -xz --strip-components=1 -C /opt/kibana -f kibana.tar.gz 	&& chown -R kibana:kibana /opt/kibana 	&& rm kibana.tar.gz 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /opt/kibana/config/kibana.yml 	&& grep -q 'elasticsearch:9200' /opt/kibana/config/kibana.yml
# Fri, 21 Oct 2016 20:27:23 GMT
ENV PATH=/opt/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 20:27:23 GMT
COPY file:1afe35294cf65766b0d19e7df5bfc671213b2d4cffe59decdc1cb601f7387d43 in / 
# Fri, 21 Oct 2016 20:27:24 GMT
EXPOSE 5601/tcp
# Fri, 21 Oct 2016 20:27:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Oct 2016 20:27:24 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f949e3abf8f4ec8b1211b1869fe813836de1919804b13d75c4c8b2f6cda52f`  
		Last Modified: Fri, 21 Oct 2016 20:25:40 GMT  
		Size: 16.6 MB (16609616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8576c69186a82a15156cac702a0f773a50ac0c5c78bda4ba2e4c24adad3d`  
		Last Modified: Fri, 21 Oct 2016 20:25:36 GMT  
		Size: 807.9 KB (807935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc26209b04278303b61ce61c61aba5181e98d76361afe71ddbda3e88d17ce59e`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 7.1 KB (7122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fd92f0a6adca9dc513d8293cd06d1dee74406296957088ea4f068dd39a8587`  
		Last Modified: Fri, 21 Oct 2016 20:27:45 GMT  
		Size: 30.5 MB (30500689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afde033e6ab33a42e187dd24edbcf147574357d0ca02d4e5f7eaf80ed7f8494`  
		Last Modified: Fri, 21 Oct 2016 20:27:35 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:4.2`

```console
$ docker pull kibana@sha256:e8d265c1cd184ed0e58669d9bdc6a2222775334e89ce7dcbe4c4e31f1d99993b
```

-	Platforms:
	-	linux; amd64

### `kibana:4.2` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.3 MB (99283175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71cda438405047fcfa05b6c04c2853fcff8c8d52fd99a6bbc517c04e46748395`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:24:51 GMT
RUN apt-get update && apt-get install -y 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:24:52 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:24:57 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:24:57 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:25:00 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:27:12 GMT
ENV KIBANA_VERSION=4.2.2
# Fri, 21 Oct 2016 20:27:12 GMT
ENV KIBANA_SHA1=f0daf9cd0b949c0ec7a3be300ee876fba17d1570
# Fri, 21 Oct 2016 20:27:22 GMT
RUN set -x 	&& wget -O kibana.tar.gz "https://download.elastic.co/kibana/kibana/kibana-${KIBANA_VERSION}-linux-x64.tar.gz" 	&& echo "${KIBANA_SHA1} *kibana.tar.gz" | sha1sum -c - 	&& mkdir -p /opt/kibana 	&& tar -xz --strip-components=1 -C /opt/kibana -f kibana.tar.gz 	&& chown -R kibana:kibana /opt/kibana 	&& rm kibana.tar.gz 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /opt/kibana/config/kibana.yml 	&& grep -q 'elasticsearch:9200' /opt/kibana/config/kibana.yml
# Fri, 21 Oct 2016 20:27:23 GMT
ENV PATH=/opt/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 20:27:23 GMT
COPY file:1afe35294cf65766b0d19e7df5bfc671213b2d4cffe59decdc1cb601f7387d43 in / 
# Fri, 21 Oct 2016 20:27:24 GMT
EXPOSE 5601/tcp
# Fri, 21 Oct 2016 20:27:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Oct 2016 20:27:24 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f949e3abf8f4ec8b1211b1869fe813836de1919804b13d75c4c8b2f6cda52f`  
		Last Modified: Fri, 21 Oct 2016 20:25:40 GMT  
		Size: 16.6 MB (16609616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8576c69186a82a15156cac702a0f773a50ac0c5c78bda4ba2e4c24adad3d`  
		Last Modified: Fri, 21 Oct 2016 20:25:36 GMT  
		Size: 807.9 KB (807935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc26209b04278303b61ce61c61aba5181e98d76361afe71ddbda3e88d17ce59e`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 7.1 KB (7122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fd92f0a6adca9dc513d8293cd06d1dee74406296957088ea4f068dd39a8587`  
		Last Modified: Fri, 21 Oct 2016 20:27:45 GMT  
		Size: 30.5 MB (30500689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afde033e6ab33a42e187dd24edbcf147574357d0ca02d4e5f7eaf80ed7f8494`  
		Last Modified: Fri, 21 Oct 2016 20:27:35 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:4.3.3`

```console
$ docker pull kibana@sha256:aaf328ecb99cb1633598bdc05e34fc23b6f7ba8962ec2afd90e976d6783b14b0
```

-	Platforms:
	-	linux; amd64

### `kibana:4.3.3` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101310059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce19f65e56e52f628d2674fb011198342c45db6de0a8ce356ad7bd9e19bb0300`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:24:51 GMT
RUN apt-get update && apt-get install -y 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:24:52 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:24:57 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:24:57 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:25:00 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:28:04 GMT
ENV KIBANA_VERSION=4.3.3
# Fri, 21 Oct 2016 20:28:04 GMT
ENV KIBANA_SHA1=3d3d0ae7658a3a7cd0d79e0f3c21701511604531
# Fri, 21 Oct 2016 20:28:15 GMT
RUN set -x 	&& wget -O kibana.tar.gz "https://download.elastic.co/kibana/kibana/kibana-${KIBANA_VERSION}-linux-x64.tar.gz" 	&& echo "${KIBANA_SHA1} *kibana.tar.gz" | sha1sum -c - 	&& mkdir -p /opt/kibana 	&& tar -xz --strip-components=1 -C /opt/kibana -f kibana.tar.gz 	&& chown -R kibana:kibana /opt/kibana 	&& rm kibana.tar.gz 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /opt/kibana/config/kibana.yml 	&& grep -q 'elasticsearch:9200' /opt/kibana/config/kibana.yml
# Fri, 21 Oct 2016 20:28:16 GMT
ENV PATH=/opt/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 20:28:16 GMT
COPY file:1afe35294cf65766b0d19e7df5bfc671213b2d4cffe59decdc1cb601f7387d43 in / 
# Fri, 21 Oct 2016 20:28:16 GMT
EXPOSE 5601/tcp
# Fri, 21 Oct 2016 20:28:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Oct 2016 20:28:17 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f949e3abf8f4ec8b1211b1869fe813836de1919804b13d75c4c8b2f6cda52f`  
		Last Modified: Fri, 21 Oct 2016 20:25:40 GMT  
		Size: 16.6 MB (16609616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8576c69186a82a15156cac702a0f773a50ac0c5c78bda4ba2e4c24adad3d`  
		Last Modified: Fri, 21 Oct 2016 20:25:36 GMT  
		Size: 807.9 KB (807935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc26209b04278303b61ce61c61aba5181e98d76361afe71ddbda3e88d17ce59e`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 7.1 KB (7122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79da5a341aa38a35d1ad57915b09fe556e7bbc82f599b1eaef2a3c792ce80b84`  
		Last Modified: Fri, 21 Oct 2016 20:28:38 GMT  
		Size: 32.5 MB (32527573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab47ac8bb75f16864e6d1dce548a44b35843e483143ac265fe84c473d5761177`  
		Last Modified: Fri, 21 Oct 2016 20:28:26 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:4.3`

```console
$ docker pull kibana@sha256:aaf328ecb99cb1633598bdc05e34fc23b6f7ba8962ec2afd90e976d6783b14b0
```

-	Platforms:
	-	linux; amd64

### `kibana:4.3` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101310059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce19f65e56e52f628d2674fb011198342c45db6de0a8ce356ad7bd9e19bb0300`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:24:51 GMT
RUN apt-get update && apt-get install -y 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:24:52 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:24:57 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:24:57 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:25:00 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:28:04 GMT
ENV KIBANA_VERSION=4.3.3
# Fri, 21 Oct 2016 20:28:04 GMT
ENV KIBANA_SHA1=3d3d0ae7658a3a7cd0d79e0f3c21701511604531
# Fri, 21 Oct 2016 20:28:15 GMT
RUN set -x 	&& wget -O kibana.tar.gz "https://download.elastic.co/kibana/kibana/kibana-${KIBANA_VERSION}-linux-x64.tar.gz" 	&& echo "${KIBANA_SHA1} *kibana.tar.gz" | sha1sum -c - 	&& mkdir -p /opt/kibana 	&& tar -xz --strip-components=1 -C /opt/kibana -f kibana.tar.gz 	&& chown -R kibana:kibana /opt/kibana 	&& rm kibana.tar.gz 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /opt/kibana/config/kibana.yml 	&& grep -q 'elasticsearch:9200' /opt/kibana/config/kibana.yml
# Fri, 21 Oct 2016 20:28:16 GMT
ENV PATH=/opt/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 20:28:16 GMT
COPY file:1afe35294cf65766b0d19e7df5bfc671213b2d4cffe59decdc1cb601f7387d43 in / 
# Fri, 21 Oct 2016 20:28:16 GMT
EXPOSE 5601/tcp
# Fri, 21 Oct 2016 20:28:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Oct 2016 20:28:17 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f949e3abf8f4ec8b1211b1869fe813836de1919804b13d75c4c8b2f6cda52f`  
		Last Modified: Fri, 21 Oct 2016 20:25:40 GMT  
		Size: 16.6 MB (16609616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8576c69186a82a15156cac702a0f773a50ac0c5c78bda4ba2e4c24adad3d`  
		Last Modified: Fri, 21 Oct 2016 20:25:36 GMT  
		Size: 807.9 KB (807935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc26209b04278303b61ce61c61aba5181e98d76361afe71ddbda3e88d17ce59e`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 7.1 KB (7122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79da5a341aa38a35d1ad57915b09fe556e7bbc82f599b1eaef2a3c792ce80b84`  
		Last Modified: Fri, 21 Oct 2016 20:28:38 GMT  
		Size: 32.5 MB (32527573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab47ac8bb75f16864e6d1dce548a44b35843e483143ac265fe84c473d5761177`  
		Last Modified: Fri, 21 Oct 2016 20:28:26 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:4.4.2`

```console
$ docker pull kibana@sha256:1a4978f31e9b655c27de21b3de672825ce8eab573dc93bb119441c89bbac8817
```

-	Platforms:
	-	linux; amd64

### `kibana:4.4.2` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101831419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdad9ec5f2367629ab900fa7b8878a2de0c558b7099d8237a0bb9adf64bacfc9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:24:51 GMT
RUN apt-get update && apt-get install -y 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:24:52 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:24:57 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:24:57 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:25:00 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:25:02 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 46095ACC8548582C1A2699A9D27D666CD88E42B4
# Fri, 21 Oct 2016 20:28:56 GMT
ENV KIBANA_MAJOR=4.4
# Fri, 21 Oct 2016 20:28:57 GMT
ENV KIBANA_VERSION=4.4.2
# Fri, 21 Oct 2016 20:28:58 GMT
RUN echo "deb http://packages.elastic.co/kibana/${KIBANA_MAJOR}/debian stable main" > /etc/apt/sources.list.d/kibana.list
# Fri, 21 Oct 2016 20:29:14 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends kibana=$KIBANA_VERSION 	&& chown -R kibana:kibana /opt/kibana 	&& rm -rf /var/lib/apt/lists/* 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /opt/kibana/config/kibana.yml 	&& grep -q 'elasticsearch:9200' /opt/kibana/config/kibana.yml
# Fri, 21 Oct 2016 20:29:15 GMT
ENV PATH=/opt/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 20:29:16 GMT
COPY file:1afe35294cf65766b0d19e7df5bfc671213b2d4cffe59decdc1cb601f7387d43 in / 
# Fri, 21 Oct 2016 20:29:16 GMT
EXPOSE 5601/tcp
# Fri, 21 Oct 2016 20:29:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Oct 2016 20:29:17 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f949e3abf8f4ec8b1211b1869fe813836de1919804b13d75c4c8b2f6cda52f`  
		Last Modified: Fri, 21 Oct 2016 20:25:40 GMT  
		Size: 16.6 MB (16609616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8576c69186a82a15156cac702a0f773a50ac0c5c78bda4ba2e4c24adad3d`  
		Last Modified: Fri, 21 Oct 2016 20:25:36 GMT  
		Size: 807.9 KB (807935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc26209b04278303b61ce61c61aba5181e98d76361afe71ddbda3e88d17ce59e`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 7.1 KB (7122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab742c8240cb823a6e4750d2a2dbd3ce7f559dfadf08df8b75d197d99bc731bb`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534b371ef7dd80a164b4c01e3ba8689e1d38c747f79cff23f7d34263585e0b82`  
		Last Modified: Fri, 21 Oct 2016 20:29:26 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6700f8c4f7be33370f2c93d52da31dd882787d5d34e57f84f1d816bf83952f`  
		Last Modified: Fri, 21 Oct 2016 20:29:38 GMT  
		Size: 33.0 MB (33047268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8877ea671155d953a6a8ed97255861e902dadff5ae8f9c7812c4a2eecd2db85`  
		Last Modified: Fri, 21 Oct 2016 20:29:26 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:4.4`

```console
$ docker pull kibana@sha256:1a4978f31e9b655c27de21b3de672825ce8eab573dc93bb119441c89bbac8817
```

-	Platforms:
	-	linux; amd64

### `kibana:4.4` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101831419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdad9ec5f2367629ab900fa7b8878a2de0c558b7099d8237a0bb9adf64bacfc9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:24:51 GMT
RUN apt-get update && apt-get install -y 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:24:52 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:24:57 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:24:57 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:25:00 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:25:02 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 46095ACC8548582C1A2699A9D27D666CD88E42B4
# Fri, 21 Oct 2016 20:28:56 GMT
ENV KIBANA_MAJOR=4.4
# Fri, 21 Oct 2016 20:28:57 GMT
ENV KIBANA_VERSION=4.4.2
# Fri, 21 Oct 2016 20:28:58 GMT
RUN echo "deb http://packages.elastic.co/kibana/${KIBANA_MAJOR}/debian stable main" > /etc/apt/sources.list.d/kibana.list
# Fri, 21 Oct 2016 20:29:14 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends kibana=$KIBANA_VERSION 	&& chown -R kibana:kibana /opt/kibana 	&& rm -rf /var/lib/apt/lists/* 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /opt/kibana/config/kibana.yml 	&& grep -q 'elasticsearch:9200' /opt/kibana/config/kibana.yml
# Fri, 21 Oct 2016 20:29:15 GMT
ENV PATH=/opt/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 20:29:16 GMT
COPY file:1afe35294cf65766b0d19e7df5bfc671213b2d4cffe59decdc1cb601f7387d43 in / 
# Fri, 21 Oct 2016 20:29:16 GMT
EXPOSE 5601/tcp
# Fri, 21 Oct 2016 20:29:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Oct 2016 20:29:17 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f949e3abf8f4ec8b1211b1869fe813836de1919804b13d75c4c8b2f6cda52f`  
		Last Modified: Fri, 21 Oct 2016 20:25:40 GMT  
		Size: 16.6 MB (16609616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8576c69186a82a15156cac702a0f773a50ac0c5c78bda4ba2e4c24adad3d`  
		Last Modified: Fri, 21 Oct 2016 20:25:36 GMT  
		Size: 807.9 KB (807935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc26209b04278303b61ce61c61aba5181e98d76361afe71ddbda3e88d17ce59e`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 7.1 KB (7122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab742c8240cb823a6e4750d2a2dbd3ce7f559dfadf08df8b75d197d99bc731bb`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534b371ef7dd80a164b4c01e3ba8689e1d38c747f79cff23f7d34263585e0b82`  
		Last Modified: Fri, 21 Oct 2016 20:29:26 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6700f8c4f7be33370f2c93d52da31dd882787d5d34e57f84f1d816bf83952f`  
		Last Modified: Fri, 21 Oct 2016 20:29:38 GMT  
		Size: 33.0 MB (33047268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8877ea671155d953a6a8ed97255861e902dadff5ae8f9c7812c4a2eecd2db85`  
		Last Modified: Fri, 21 Oct 2016 20:29:26 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:4.5.4`

```console
$ docker pull kibana@sha256:90f7c1ad24dc5a5b7b7e24bc09a8d902f7acc646beb1f611eacb7ddb58bdab45
```

-	Platforms:
	-	linux; amd64

### `kibana:4.5.4` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102236215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b303aeb5bba32079b59bdaa98882564e0a7976aca836a5631022757899066a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:24:51 GMT
RUN apt-get update && apt-get install -y 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:24:52 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:24:57 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:24:57 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:25:00 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:25:02 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 46095ACC8548582C1A2699A9D27D666CD88E42B4
# Fri, 21 Oct 2016 20:29:57 GMT
ENV KIBANA_MAJOR=4.5
# Fri, 21 Oct 2016 20:29:58 GMT
ENV KIBANA_VERSION=4.5.4
# Fri, 21 Oct 2016 20:29:59 GMT
RUN echo "deb http://packages.elastic.co/kibana/${KIBANA_MAJOR}/debian stable main" > /etc/apt/sources.list.d/kibana.list
# Fri, 21 Oct 2016 20:30:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends kibana=$KIBANA_VERSION 	&& chown -R kibana:kibana /opt/kibana 	&& rm -rf /var/lib/apt/lists/* 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /opt/kibana/config/kibana.yml 	&& grep -q 'elasticsearch:9200' /opt/kibana/config/kibana.yml
# Fri, 21 Oct 2016 20:30:16 GMT
ENV PATH=/opt/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 20:30:17 GMT
COPY file:1afe35294cf65766b0d19e7df5bfc671213b2d4cffe59decdc1cb601f7387d43 in / 
# Fri, 21 Oct 2016 20:30:17 GMT
EXPOSE 5601/tcp
# Fri, 21 Oct 2016 20:30:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Oct 2016 20:30:18 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f949e3abf8f4ec8b1211b1869fe813836de1919804b13d75c4c8b2f6cda52f`  
		Last Modified: Fri, 21 Oct 2016 20:25:40 GMT  
		Size: 16.6 MB (16609616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8576c69186a82a15156cac702a0f773a50ac0c5c78bda4ba2e4c24adad3d`  
		Last Modified: Fri, 21 Oct 2016 20:25:36 GMT  
		Size: 807.9 KB (807935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc26209b04278303b61ce61c61aba5181e98d76361afe71ddbda3e88d17ce59e`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 7.1 KB (7122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab742c8240cb823a6e4750d2a2dbd3ce7f559dfadf08df8b75d197d99bc731bb`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca14bf0bfc016676b78cb99bf7af19de74dbb50bce6d4b5d589455e71f1fcc7`  
		Last Modified: Fri, 21 Oct 2016 20:30:27 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881f85f692596f4a8883cce7d80398ba5836a53285943917128bd5791c33f946`  
		Last Modified: Fri, 21 Oct 2016 20:30:38 GMT  
		Size: 33.5 MB (33452064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1098b9e643699b0048a3dd77b7aa2bd8461adacdd0a948a150dfc5460efcbcd4`  
		Last Modified: Fri, 21 Oct 2016 20:30:27 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:4.5`

```console
$ docker pull kibana@sha256:90f7c1ad24dc5a5b7b7e24bc09a8d902f7acc646beb1f611eacb7ddb58bdab45
```

-	Platforms:
	-	linux; amd64

### `kibana:4.5` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102236215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b303aeb5bba32079b59bdaa98882564e0a7976aca836a5631022757899066a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:24:51 GMT
RUN apt-get update && apt-get install -y 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:24:52 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:24:57 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:24:57 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:25:00 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:25:02 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 46095ACC8548582C1A2699A9D27D666CD88E42B4
# Fri, 21 Oct 2016 20:29:57 GMT
ENV KIBANA_MAJOR=4.5
# Fri, 21 Oct 2016 20:29:58 GMT
ENV KIBANA_VERSION=4.5.4
# Fri, 21 Oct 2016 20:29:59 GMT
RUN echo "deb http://packages.elastic.co/kibana/${KIBANA_MAJOR}/debian stable main" > /etc/apt/sources.list.d/kibana.list
# Fri, 21 Oct 2016 20:30:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends kibana=$KIBANA_VERSION 	&& chown -R kibana:kibana /opt/kibana 	&& rm -rf /var/lib/apt/lists/* 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /opt/kibana/config/kibana.yml 	&& grep -q 'elasticsearch:9200' /opt/kibana/config/kibana.yml
# Fri, 21 Oct 2016 20:30:16 GMT
ENV PATH=/opt/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 20:30:17 GMT
COPY file:1afe35294cf65766b0d19e7df5bfc671213b2d4cffe59decdc1cb601f7387d43 in / 
# Fri, 21 Oct 2016 20:30:17 GMT
EXPOSE 5601/tcp
# Fri, 21 Oct 2016 20:30:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Oct 2016 20:30:18 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f949e3abf8f4ec8b1211b1869fe813836de1919804b13d75c4c8b2f6cda52f`  
		Last Modified: Fri, 21 Oct 2016 20:25:40 GMT  
		Size: 16.6 MB (16609616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8576c69186a82a15156cac702a0f773a50ac0c5c78bda4ba2e4c24adad3d`  
		Last Modified: Fri, 21 Oct 2016 20:25:36 GMT  
		Size: 807.9 KB (807935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc26209b04278303b61ce61c61aba5181e98d76361afe71ddbda3e88d17ce59e`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 7.1 KB (7122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab742c8240cb823a6e4750d2a2dbd3ce7f559dfadf08df8b75d197d99bc731bb`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca14bf0bfc016676b78cb99bf7af19de74dbb50bce6d4b5d589455e71f1fcc7`  
		Last Modified: Fri, 21 Oct 2016 20:30:27 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881f85f692596f4a8883cce7d80398ba5836a53285943917128bd5791c33f946`  
		Last Modified: Fri, 21 Oct 2016 20:30:38 GMT  
		Size: 33.5 MB (33452064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1098b9e643699b0048a3dd77b7aa2bd8461adacdd0a948a150dfc5460efcbcd4`  
		Last Modified: Fri, 21 Oct 2016 20:30:27 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:4.6.2`

```console
$ docker pull kibana@sha256:d76d3d72a02dfed60b3c02475501b176178aee9e42fb22f63064eed6ef23ad98
```

-	Platforms:
	-	linux; amd64

### `kibana:4.6.2` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103070100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:547e03cb364b324e35b933ccddc0f58cc409545fd6b82d28c0341b5bd571bd1f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:24:51 GMT
RUN apt-get update && apt-get install -y 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:24:52 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:24:57 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:24:57 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:25:00 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:25:02 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 46095ACC8548582C1A2699A9D27D666CD88E42B4
# Fri, 21 Oct 2016 20:25:02 GMT
ENV KIBANA_MAJOR=4.6
# Mon, 24 Oct 2016 18:57:34 GMT
ENV KIBANA_VERSION=4.6.2
# Mon, 24 Oct 2016 18:57:34 GMT
RUN echo "deb http://packages.elastic.co/kibana/${KIBANA_MAJOR}/debian stable main" > /etc/apt/sources.list.d/kibana.list
# Mon, 24 Oct 2016 18:57:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends kibana=$KIBANA_VERSION 	&& chown -R kibana:kibana /opt/kibana 	&& rm -rf /var/lib/apt/lists/* 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /opt/kibana/config/kibana.yml 	&& grep -q 'elasticsearch:9200' /opt/kibana/config/kibana.yml
# Mon, 24 Oct 2016 18:57:53 GMT
ENV PATH=/opt/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Oct 2016 18:57:53 GMT
COPY file:1afe35294cf65766b0d19e7df5bfc671213b2d4cffe59decdc1cb601f7387d43 in / 
# Mon, 24 Oct 2016 18:57:54 GMT
EXPOSE 5601/tcp
# Mon, 24 Oct 2016 18:57:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 24 Oct 2016 18:57:54 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f949e3abf8f4ec8b1211b1869fe813836de1919804b13d75c4c8b2f6cda52f`  
		Last Modified: Fri, 21 Oct 2016 20:25:40 GMT  
		Size: 16.6 MB (16609616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8576c69186a82a15156cac702a0f773a50ac0c5c78bda4ba2e4c24adad3d`  
		Last Modified: Fri, 21 Oct 2016 20:25:36 GMT  
		Size: 807.9 KB (807935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc26209b04278303b61ce61c61aba5181e98d76361afe71ddbda3e88d17ce59e`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 7.1 KB (7122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab742c8240cb823a6e4750d2a2dbd3ce7f559dfadf08df8b75d197d99bc731bb`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e4024e7395542e90ca9757d389c0f19cde97620290674d66ee7e25bfb3200c`  
		Last Modified: Mon, 24 Oct 2016 19:00:10 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ce6adf34f5c16f021c118151a2d2ad2904a76fa26cf512561e7d0a83dc0bf`  
		Last Modified: Mon, 24 Oct 2016 19:00:18 GMT  
		Size: 34.3 MB (34285946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ef3273f68483e15347793e58b9365ba218e54282c7f31e31231cef2c8d81ba`  
		Last Modified: Mon, 24 Oct 2016 19:00:06 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:4.6`

```console
$ docker pull kibana@sha256:d76d3d72a02dfed60b3c02475501b176178aee9e42fb22f63064eed6ef23ad98
```

-	Platforms:
	-	linux; amd64

### `kibana:4.6` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103070100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:547e03cb364b324e35b933ccddc0f58cc409545fd6b82d28c0341b5bd571bd1f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:24:51 GMT
RUN apt-get update && apt-get install -y 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:24:52 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:24:57 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:24:57 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:25:00 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:25:02 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 46095ACC8548582C1A2699A9D27D666CD88E42B4
# Fri, 21 Oct 2016 20:25:02 GMT
ENV KIBANA_MAJOR=4.6
# Mon, 24 Oct 2016 18:57:34 GMT
ENV KIBANA_VERSION=4.6.2
# Mon, 24 Oct 2016 18:57:34 GMT
RUN echo "deb http://packages.elastic.co/kibana/${KIBANA_MAJOR}/debian stable main" > /etc/apt/sources.list.d/kibana.list
# Mon, 24 Oct 2016 18:57:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends kibana=$KIBANA_VERSION 	&& chown -R kibana:kibana /opt/kibana 	&& rm -rf /var/lib/apt/lists/* 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /opt/kibana/config/kibana.yml 	&& grep -q 'elasticsearch:9200' /opt/kibana/config/kibana.yml
# Mon, 24 Oct 2016 18:57:53 GMT
ENV PATH=/opt/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Oct 2016 18:57:53 GMT
COPY file:1afe35294cf65766b0d19e7df5bfc671213b2d4cffe59decdc1cb601f7387d43 in / 
# Mon, 24 Oct 2016 18:57:54 GMT
EXPOSE 5601/tcp
# Mon, 24 Oct 2016 18:57:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 24 Oct 2016 18:57:54 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f949e3abf8f4ec8b1211b1869fe813836de1919804b13d75c4c8b2f6cda52f`  
		Last Modified: Fri, 21 Oct 2016 20:25:40 GMT  
		Size: 16.6 MB (16609616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8576c69186a82a15156cac702a0f773a50ac0c5c78bda4ba2e4c24adad3d`  
		Last Modified: Fri, 21 Oct 2016 20:25:36 GMT  
		Size: 807.9 KB (807935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc26209b04278303b61ce61c61aba5181e98d76361afe71ddbda3e88d17ce59e`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 7.1 KB (7122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab742c8240cb823a6e4750d2a2dbd3ce7f559dfadf08df8b75d197d99bc731bb`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e4024e7395542e90ca9757d389c0f19cde97620290674d66ee7e25bfb3200c`  
		Last Modified: Mon, 24 Oct 2016 19:00:10 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ce6adf34f5c16f021c118151a2d2ad2904a76fa26cf512561e7d0a83dc0bf`  
		Last Modified: Mon, 24 Oct 2016 19:00:18 GMT  
		Size: 34.3 MB (34285946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ef3273f68483e15347793e58b9365ba218e54282c7f31e31231cef2c8d81ba`  
		Last Modified: Mon, 24 Oct 2016 19:00:06 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:4`

```console
$ docker pull kibana@sha256:d76d3d72a02dfed60b3c02475501b176178aee9e42fb22f63064eed6ef23ad98
```

-	Platforms:
	-	linux; amd64

### `kibana:4` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103070100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:547e03cb364b324e35b933ccddc0f58cc409545fd6b82d28c0341b5bd571bd1f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:24:51 GMT
RUN apt-get update && apt-get install -y 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:24:52 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:24:57 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:24:57 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:25:00 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:25:02 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 46095ACC8548582C1A2699A9D27D666CD88E42B4
# Fri, 21 Oct 2016 20:25:02 GMT
ENV KIBANA_MAJOR=4.6
# Mon, 24 Oct 2016 18:57:34 GMT
ENV KIBANA_VERSION=4.6.2
# Mon, 24 Oct 2016 18:57:34 GMT
RUN echo "deb http://packages.elastic.co/kibana/${KIBANA_MAJOR}/debian stable main" > /etc/apt/sources.list.d/kibana.list
# Mon, 24 Oct 2016 18:57:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends kibana=$KIBANA_VERSION 	&& chown -R kibana:kibana /opt/kibana 	&& rm -rf /var/lib/apt/lists/* 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /opt/kibana/config/kibana.yml 	&& grep -q 'elasticsearch:9200' /opt/kibana/config/kibana.yml
# Mon, 24 Oct 2016 18:57:53 GMT
ENV PATH=/opt/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Oct 2016 18:57:53 GMT
COPY file:1afe35294cf65766b0d19e7df5bfc671213b2d4cffe59decdc1cb601f7387d43 in / 
# Mon, 24 Oct 2016 18:57:54 GMT
EXPOSE 5601/tcp
# Mon, 24 Oct 2016 18:57:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 24 Oct 2016 18:57:54 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f949e3abf8f4ec8b1211b1869fe813836de1919804b13d75c4c8b2f6cda52f`  
		Last Modified: Fri, 21 Oct 2016 20:25:40 GMT  
		Size: 16.6 MB (16609616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714b8576c69186a82a15156cac702a0f773a50ac0c5c78bda4ba2e4c24adad3d`  
		Last Modified: Fri, 21 Oct 2016 20:25:36 GMT  
		Size: 807.9 KB (807935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc26209b04278303b61ce61c61aba5181e98d76361afe71ddbda3e88d17ce59e`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 7.1 KB (7122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab742c8240cb823a6e4750d2a2dbd3ce7f559dfadf08df8b75d197d99bc731bb`  
		Last Modified: Fri, 21 Oct 2016 20:25:33 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e4024e7395542e90ca9757d389c0f19cde97620290674d66ee7e25bfb3200c`  
		Last Modified: Mon, 24 Oct 2016 19:00:10 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ce6adf34f5c16f021c118151a2d2ad2904a76fa26cf512561e7d0a83dc0bf`  
		Last Modified: Mon, 24 Oct 2016 19:00:18 GMT  
		Size: 34.3 MB (34285946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ef3273f68483e15347793e58b9365ba218e54282c7f31e31231cef2c8d81ba`  
		Last Modified: Mon, 24 Oct 2016 19:00:06 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:5.0.0`

```console
$ docker pull kibana@sha256:b18e8e03193b56c2c10e9530d281f47151c59d85576294dc8d559de92d1bb83c
```

-	Platforms:
	-	linux; amd64

### `kibana:5.0.0` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111001826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57381b34e3ea8bc58c7d7051ce27ed25e1e9ff1072f499b143e96509d4f5b4a8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:31:11 GMT
RUN apt-get update && apt-get install -y 		apt-transport-https 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:31:11 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:31:23 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:31:23 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:31:26 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:31:28 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 46095ACC8548582C1A2699A9D27D666CD88E42B4
# Fri, 21 Oct 2016 20:31:28 GMT
ENV KIBANA_MAJOR=5.0
# Wed, 26 Oct 2016 20:30:40 GMT
ENV KIBANA_VERSION=5.0.0
# Wed, 26 Oct 2016 20:30:41 GMT
RUN echo 'deb https://artifacts.elastic.co/packages/5.x/apt stable main' > /etc/apt/sources.list.d/kibana.list
# Wed, 26 Oct 2016 20:30:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends kibana=$KIBANA_VERSION 	&& rm -rf /var/lib/apt/lists/* 		&& sed -ri "s!^(\#\s*)?(server\.host:).*!\2 '0.0.0.0'!" /etc/kibana/kibana.yml 	&& grep -q "^server\.host: '0.0.0.0'\$" /etc/kibana/kibana.yml 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /etc/kibana/kibana.yml 	&& grep -q "^elasticsearch\.url: 'http://elasticsearch:9200'\$" /etc/kibana/kibana.yml
# Wed, 26 Oct 2016 20:31:00 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2016 20:31:00 GMT
COPY file:9a3ed3a1655d5afa631fded5211f1c33f5f49f1d1e0e0d9a031c9e8601111f05 in / 
# Wed, 26 Oct 2016 20:31:01 GMT
EXPOSE 5601/tcp
# Wed, 26 Oct 2016 20:31:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Oct 2016 20:31:01 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce46c41cb89fa517ea63261714602a80f830a3c2593a97aaed7bb763db48926`  
		Last Modified: Fri, 21 Oct 2016 20:32:08 GMT  
		Size: 18.5 MB (18456229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799f25bf4f577d35af4ed511b435a6a4a08a7add762bf7456bfbffc9d0f18118`  
		Last Modified: Fri, 21 Oct 2016 20:32:02 GMT  
		Size: 807.9 KB (807934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1609dd0feef4c73990b78d6d3d85d9a73653f6987363011fdd1e683178622366`  
		Last Modified: Fri, 21 Oct 2016 20:32:00 GMT  
		Size: 7.1 KB (7124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a672c9fed7375479d7729d96dfc64cd4cb46998d71746f0a7f8c99f294e94b`  
		Last Modified: Fri, 21 Oct 2016 20:32:01 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2346b42f8dbc927218ba0eb27082267dc20dbb9ab6b06bf6131a8b659907534`  
		Last Modified: Wed, 26 Oct 2016 20:33:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5465ede92a4675d4d0626fa3e85af213ee10f5542b5a6e80fcef1ae1a24f55d2`  
		Last Modified: Wed, 26 Oct 2016 20:33:57 GMT  
		Size: 40.4 MB (40371063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede2426cbc83fb3abd0bf57950483414cd82c10e50268ad7bed3eace13b32fef`  
		Last Modified: Wed, 26 Oct 2016 20:33:43 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:5.0`

```console
$ docker pull kibana@sha256:b18e8e03193b56c2c10e9530d281f47151c59d85576294dc8d559de92d1bb83c
```

-	Platforms:
	-	linux; amd64

### `kibana:5.0` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111001826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57381b34e3ea8bc58c7d7051ce27ed25e1e9ff1072f499b143e96509d4f5b4a8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:31:11 GMT
RUN apt-get update && apt-get install -y 		apt-transport-https 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:31:11 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:31:23 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:31:23 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:31:26 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:31:28 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 46095ACC8548582C1A2699A9D27D666CD88E42B4
# Fri, 21 Oct 2016 20:31:28 GMT
ENV KIBANA_MAJOR=5.0
# Wed, 26 Oct 2016 20:30:40 GMT
ENV KIBANA_VERSION=5.0.0
# Wed, 26 Oct 2016 20:30:41 GMT
RUN echo 'deb https://artifacts.elastic.co/packages/5.x/apt stable main' > /etc/apt/sources.list.d/kibana.list
# Wed, 26 Oct 2016 20:30:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends kibana=$KIBANA_VERSION 	&& rm -rf /var/lib/apt/lists/* 		&& sed -ri "s!^(\#\s*)?(server\.host:).*!\2 '0.0.0.0'!" /etc/kibana/kibana.yml 	&& grep -q "^server\.host: '0.0.0.0'\$" /etc/kibana/kibana.yml 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /etc/kibana/kibana.yml 	&& grep -q "^elasticsearch\.url: 'http://elasticsearch:9200'\$" /etc/kibana/kibana.yml
# Wed, 26 Oct 2016 20:31:00 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2016 20:31:00 GMT
COPY file:9a3ed3a1655d5afa631fded5211f1c33f5f49f1d1e0e0d9a031c9e8601111f05 in / 
# Wed, 26 Oct 2016 20:31:01 GMT
EXPOSE 5601/tcp
# Wed, 26 Oct 2016 20:31:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Oct 2016 20:31:01 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce46c41cb89fa517ea63261714602a80f830a3c2593a97aaed7bb763db48926`  
		Last Modified: Fri, 21 Oct 2016 20:32:08 GMT  
		Size: 18.5 MB (18456229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799f25bf4f577d35af4ed511b435a6a4a08a7add762bf7456bfbffc9d0f18118`  
		Last Modified: Fri, 21 Oct 2016 20:32:02 GMT  
		Size: 807.9 KB (807934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1609dd0feef4c73990b78d6d3d85d9a73653f6987363011fdd1e683178622366`  
		Last Modified: Fri, 21 Oct 2016 20:32:00 GMT  
		Size: 7.1 KB (7124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a672c9fed7375479d7729d96dfc64cd4cb46998d71746f0a7f8c99f294e94b`  
		Last Modified: Fri, 21 Oct 2016 20:32:01 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2346b42f8dbc927218ba0eb27082267dc20dbb9ab6b06bf6131a8b659907534`  
		Last Modified: Wed, 26 Oct 2016 20:33:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5465ede92a4675d4d0626fa3e85af213ee10f5542b5a6e80fcef1ae1a24f55d2`  
		Last Modified: Wed, 26 Oct 2016 20:33:57 GMT  
		Size: 40.4 MB (40371063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede2426cbc83fb3abd0bf57950483414cd82c10e50268ad7bed3eace13b32fef`  
		Last Modified: Wed, 26 Oct 2016 20:33:43 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:5`

```console
$ docker pull kibana@sha256:b18e8e03193b56c2c10e9530d281f47151c59d85576294dc8d559de92d1bb83c
```

-	Platforms:
	-	linux; amd64

### `kibana:5` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111001826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57381b34e3ea8bc58c7d7051ce27ed25e1e9ff1072f499b143e96509d4f5b4a8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:31:11 GMT
RUN apt-get update && apt-get install -y 		apt-transport-https 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:31:11 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:31:23 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:31:23 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:31:26 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:31:28 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 46095ACC8548582C1A2699A9D27D666CD88E42B4
# Fri, 21 Oct 2016 20:31:28 GMT
ENV KIBANA_MAJOR=5.0
# Wed, 26 Oct 2016 20:30:40 GMT
ENV KIBANA_VERSION=5.0.0
# Wed, 26 Oct 2016 20:30:41 GMT
RUN echo 'deb https://artifacts.elastic.co/packages/5.x/apt stable main' > /etc/apt/sources.list.d/kibana.list
# Wed, 26 Oct 2016 20:30:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends kibana=$KIBANA_VERSION 	&& rm -rf /var/lib/apt/lists/* 		&& sed -ri "s!^(\#\s*)?(server\.host:).*!\2 '0.0.0.0'!" /etc/kibana/kibana.yml 	&& grep -q "^server\.host: '0.0.0.0'\$" /etc/kibana/kibana.yml 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /etc/kibana/kibana.yml 	&& grep -q "^elasticsearch\.url: 'http://elasticsearch:9200'\$" /etc/kibana/kibana.yml
# Wed, 26 Oct 2016 20:31:00 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2016 20:31:00 GMT
COPY file:9a3ed3a1655d5afa631fded5211f1c33f5f49f1d1e0e0d9a031c9e8601111f05 in / 
# Wed, 26 Oct 2016 20:31:01 GMT
EXPOSE 5601/tcp
# Wed, 26 Oct 2016 20:31:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Oct 2016 20:31:01 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce46c41cb89fa517ea63261714602a80f830a3c2593a97aaed7bb763db48926`  
		Last Modified: Fri, 21 Oct 2016 20:32:08 GMT  
		Size: 18.5 MB (18456229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799f25bf4f577d35af4ed511b435a6a4a08a7add762bf7456bfbffc9d0f18118`  
		Last Modified: Fri, 21 Oct 2016 20:32:02 GMT  
		Size: 807.9 KB (807934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1609dd0feef4c73990b78d6d3d85d9a73653f6987363011fdd1e683178622366`  
		Last Modified: Fri, 21 Oct 2016 20:32:00 GMT  
		Size: 7.1 KB (7124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a672c9fed7375479d7729d96dfc64cd4cb46998d71746f0a7f8c99f294e94b`  
		Last Modified: Fri, 21 Oct 2016 20:32:01 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2346b42f8dbc927218ba0eb27082267dc20dbb9ab6b06bf6131a8b659907534`  
		Last Modified: Wed, 26 Oct 2016 20:33:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5465ede92a4675d4d0626fa3e85af213ee10f5542b5a6e80fcef1ae1a24f55d2`  
		Last Modified: Wed, 26 Oct 2016 20:33:57 GMT  
		Size: 40.4 MB (40371063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede2426cbc83fb3abd0bf57950483414cd82c10e50268ad7bed3eace13b32fef`  
		Last Modified: Wed, 26 Oct 2016 20:33:43 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:latest`

```console
$ docker pull kibana@sha256:b18e8e03193b56c2c10e9530d281f47151c59d85576294dc8d559de92d1bb83c
```

-	Platforms:
	-	linux; amd64

### `kibana:latest` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111001826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57381b34e3ea8bc58c7d7051ce27ed25e1e9ff1072f499b143e96509d4f5b4a8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kibana"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 20:24:38 GMT
RUN groupadd -r kibana && useradd -r -m -g kibana kibana
# Fri, 21 Oct 2016 20:31:11 GMT
RUN apt-get update && apt-get install -y 		apt-transport-https 		ca-certificates 		wget 	--no-install-recommends && rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:31:11 GMT
ENV GOSU_VERSION=1.7
# Fri, 21 Oct 2016 20:31:23 GMT
RUN set -x 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true
# Fri, 21 Oct 2016 20:31:23 GMT
ENV TINI_VERSION=v0.9.0
# Fri, 21 Oct 2016 20:31:26 GMT
RUN set -x 	&& wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini" 	&& wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/$TINI_VERSION/tini.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5 	&& gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini 	&& rm -r "$GNUPGHOME" /usr/local/bin/tini.asc 	&& chmod +x /usr/local/bin/tini 	&& tini -h
# Fri, 21 Oct 2016 20:31:28 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 46095ACC8548582C1A2699A9D27D666CD88E42B4
# Fri, 21 Oct 2016 20:31:28 GMT
ENV KIBANA_MAJOR=5.0
# Wed, 26 Oct 2016 20:30:40 GMT
ENV KIBANA_VERSION=5.0.0
# Wed, 26 Oct 2016 20:30:41 GMT
RUN echo 'deb https://artifacts.elastic.co/packages/5.x/apt stable main' > /etc/apt/sources.list.d/kibana.list
# Wed, 26 Oct 2016 20:30:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends kibana=$KIBANA_VERSION 	&& rm -rf /var/lib/apt/lists/* 		&& sed -ri "s!^(\#\s*)?(server\.host:).*!\2 '0.0.0.0'!" /etc/kibana/kibana.yml 	&& grep -q "^server\.host: '0.0.0.0'\$" /etc/kibana/kibana.yml 		&& sed -ri "s!^(\#\s*)?(elasticsearch\.url:).*!\2 'http://elasticsearch:9200'!" /etc/kibana/kibana.yml 	&& grep -q "^elasticsearch\.url: 'http://elasticsearch:9200'\$" /etc/kibana/kibana.yml
# Wed, 26 Oct 2016 20:31:00 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2016 20:31:00 GMT
COPY file:9a3ed3a1655d5afa631fded5211f1c33f5f49f1d1e0e0d9a031c9e8601111f05 in / 
# Wed, 26 Oct 2016 20:31:01 GMT
EXPOSE 5601/tcp
# Wed, 26 Oct 2016 20:31:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Oct 2016 20:31:01 GMT
CMD ["kibana"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592250a6a44e451dc6758866fd7297c68832c948512fcde20e436abc26b97d0a`  
		Last Modified: Fri, 21 Oct 2016 20:25:35 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce46c41cb89fa517ea63261714602a80f830a3c2593a97aaed7bb763db48926`  
		Last Modified: Fri, 21 Oct 2016 20:32:08 GMT  
		Size: 18.5 MB (18456229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799f25bf4f577d35af4ed511b435a6a4a08a7add762bf7456bfbffc9d0f18118`  
		Last Modified: Fri, 21 Oct 2016 20:32:02 GMT  
		Size: 807.9 KB (807934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1609dd0feef4c73990b78d6d3d85d9a73653f6987363011fdd1e683178622366`  
		Last Modified: Fri, 21 Oct 2016 20:32:00 GMT  
		Size: 7.1 KB (7124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a672c9fed7375479d7729d96dfc64cd4cb46998d71746f0a7f8c99f294e94b`  
		Last Modified: Fri, 21 Oct 2016 20:32:01 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2346b42f8dbc927218ba0eb27082267dc20dbb9ab6b06bf6131a8b659907534`  
		Last Modified: Wed, 26 Oct 2016 20:33:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5465ede92a4675d4d0626fa3e85af213ee10f5542b5a6e80fcef1ae1a24f55d2`  
		Last Modified: Wed, 26 Oct 2016 20:33:57 GMT  
		Size: 40.4 MB (40371063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede2426cbc83fb3abd0bf57950483414cd82c10e50268ad7bed3eace13b32fef`  
		Last Modified: Wed, 26 Oct 2016 20:33:43 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
