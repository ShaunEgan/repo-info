## `jetty:jre7`

```console
$ docker pull jetty@sha256:a50c2225eca8629707827075c7ce1fda3d81a7a1dec14e6e1e334edfbfd39bf3
```

-	Platforms:
	-	linux; amd64

### `jetty:jre7` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158185034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:252074490a22cf73cac50061cdfbcd04c456e07b88407961dfb50b24c0776f75`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 30 Aug 2016 21:00:51 GMT
ADD file:f2453b914e7e026efd39c6321c7b14509b6d09dd3cf5567a8f6bd38466e06954 in / 
# Tue, 30 Aug 2016 21:00:52 GMT
CMD ["/bin/bash"]
# Tue, 30 Aug 2016 21:52:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Aug 2016 17:13:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Aug 2016 17:13:55 GMT
ENV LANG=C.UTF-8
# Wed, 31 Aug 2016 17:13:56 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 31 Aug 2016 17:13:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-7-openjdk-amd64/jre
# Wed, 31 Aug 2016 17:13:57 GMT
ENV JAVA_VERSION=7u111
# Wed, 31 Aug 2016 17:13:57 GMT
ENV JAVA_DEBIAN_VERSION=7u111-2.6.7-1~deb8u1
# Wed, 31 Aug 2016 17:15:00 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-7-jre-headless="$JAVA_DEBIAN_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 31 Aug 2016 20:53:59 GMT
RUN groupadd -r jetty && useradd -r -g jetty jetty
# Wed, 31 Aug 2016 20:54:00 GMT
ENV JETTY_HOME=/usr/local/jetty
# Wed, 31 Aug 2016 20:54:00 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Aug 2016 20:54:01 GMT
RUN mkdir -p "$JETTY_HOME"
# Wed, 31 Aug 2016 20:54:01 GMT
WORKDIR /usr/local/jetty
# Wed, 31 Aug 2016 20:54:01 GMT
ENV JETTY_VERSION=9.2.18.v20160721
# Wed, 31 Aug 2016 20:54:02 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-distribution/9.2.18.v20160721/jetty-distribution-9.2.18.v20160721.tar.gz
# Wed, 31 Aug 2016 20:54:02 GMT
ENV JETTY_GPG_KEYS=B59B67FD7904984367F931800818D9D68FB67BAC 	5DE533CB43DAF8BC3E372283E7AE839CD7C58886
# Wed, 31 Aug 2016 20:54:05 GMT
RUN set -xe 	&& curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz 	&& curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& for key in $JETTY_GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; done 	&& gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz 	&& rm -r "$GNUPGHOME" 	&& tar -xvf jetty.tar.gz --strip-components=1 	&& sed -i '/jetty-logging/d' etc/jetty.conf 	&& rm -fr demo-base javadoc 	&& rm jetty.tar.gz*
# Wed, 31 Aug 2016 20:54:05 GMT
ENV JETTY_BASE=/var/lib/jetty
# Wed, 31 Aug 2016 20:54:06 GMT
RUN mkdir -p "$JETTY_BASE"
# Wed, 31 Aug 2016 20:54:06 GMT
WORKDIR /var/lib/jetty
# Wed, 31 Aug 2016 20:54:09 GMT
RUN modules="$(grep -- ^--module= "$JETTY_HOME/start.ini" | cut -d= -f2 | paste -d, -s)" 	&& set -xe 	&& java -jar "$JETTY_HOME/start.jar" --add-to-startd="$modules,setuid"
# Wed, 31 Aug 2016 20:54:09 GMT
ENV TMPDIR=/tmp/jetty
# Wed, 31 Aug 2016 20:54:10 GMT
RUN set -xe 	&& mkdir -p "$TMPDIR" 	&& chown -R jetty:jetty "$TMPDIR" "$JETTY_BASE"
# Wed, 31 Aug 2016 20:54:11 GMT
COPY file:4f7da2906a90932cfb90db54a45ee08f86b17253747db62085f7512c9efd46ad in / 
# Wed, 31 Aug 2016 20:54:11 GMT
EXPOSE 8080/tcp
# Wed, 31 Aug 2016 20:54:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 31 Aug 2016 20:54:11 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:8ad8b3f87b378cfae583fef34e47a3c9203847d779961b7351cbf786af0bc09f`  
		Last Modified: Tue, 30 Aug 2016 21:02:02 GMT  
		Size: 51.4 MB (51367268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751fe39c4d348c7fc411d46929c1dac390e3d7107efc9f8f69641b50e14459f7`  
		Last Modified: Tue, 30 Aug 2016 21:59:08 GMT  
		Size: 18.5 MB (18527264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b165e84cccc10bc56e89091e37339ab98afbef36d1f06cd9c1c531af4dc18aa1`  
		Last Modified: Wed, 31 Aug 2016 17:24:31 GMT  
		Size: 566.9 KB (566898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f65ec902a1b1e7ebbd6d2f0be784334776d98e700d95657308a4e93becdf32`  
		Last Modified: Wed, 31 Aug 2016 17:24:30 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e29d14c31c0752f233600a073a4e0e439dcf16305d5fe8e081684071e6381f`  
		Last Modified: Wed, 31 Aug 2016 17:24:48 GMT  
		Size: 77.7 MB (77713068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dce28e54d1f9227089efdaba6f3265623d5fe4083e0adda89daea59cc503ab4`  
		Last Modified: Wed, 31 Aug 2016 20:54:20 GMT  
		Size: 2.1 KB (2082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112226fdbf95e35d78343aafd8f995972e393dc27a2a7d38028175653c187119`  
		Last Modified: Wed, 31 Aug 2016 20:54:20 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed96e1340437b42d8ff918e66bc23ae812e3d1b4551f3893912659c4c5b29a34`  
		Last Modified: Wed, 31 Aug 2016 20:54:18 GMT  
		Size: 10.0 MB (10004221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215e18171f5a5c5f27a0b37468109fd60b0c82346ef9188dfb16421ed25531e7`  
		Last Modified: Wed, 31 Aug 2016 20:54:17 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc2356ee4bae12e9ce0991a0f9f95f9fad7685d604b4e1283e964199cd4520f`  
		Last Modified: Wed, 31 Aug 2016 20:54:17 GMT  
		Size: 1.6 KB (1572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58921901f7be4e1febd005b95fd8e6237b1e2ba61e84ae2d2de7c39c45f5d7d0`  
		Last Modified: Wed, 31 Aug 2016 20:54:16 GMT  
		Size: 1.6 KB (1572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e44b56a5e8245925aa93a7c0552f9e2135de25dfa954922ad69347a0087f3f`  
		Last Modified: Wed, 31 Aug 2016 20:54:17 GMT  
		Size: 572.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip