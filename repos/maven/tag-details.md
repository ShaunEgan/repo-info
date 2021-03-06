<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `maven`

-	[`maven:3.3.9-jdk-7`](#maven339-jdk-7)
-	[`maven:3.3-jdk-7`](#maven33-jdk-7)
-	[`maven:3-jdk-7`](#maven3-jdk-7)
-	[`maven:3.3.9-jdk-7-onbuild`](#maven339-jdk-7-onbuild)
-	[`maven:3.3-jdk-7-onbuild`](#maven33-jdk-7-onbuild)
-	[`maven:3-jdk-7-onbuild`](#maven3-jdk-7-onbuild)
-	[`maven:3.3.9-jdk-7-alpine`](#maven339-jdk-7-alpine)
-	[`maven:3.3-jdk-7-alpine`](#maven33-jdk-7-alpine)
-	[`maven:3-jdk-7-alpine`](#maven3-jdk-7-alpine)
-	[`maven:3.3.9-jdk-7-onbuild-alpine`](#maven339-jdk-7-onbuild-alpine)
-	[`maven:3.3-jdk-7-onbuild-alpine`](#maven33-jdk-7-onbuild-alpine)
-	[`maven:3-jdk-7-onbuild-alpine`](#maven3-jdk-7-onbuild-alpine)
-	[`maven:3.3.9-jdk-8`](#maven339-jdk-8)
-	[`maven:3.3.9`](#maven339)
-	[`maven:3.3-jdk-8`](#maven33-jdk-8)
-	[`maven:3.3`](#maven33)
-	[`maven:3-jdk-8`](#maven3-jdk-8)
-	[`maven:3`](#maven3)
-	[`maven:latest`](#mavenlatest)
-	[`maven:3.3.9-jdk-8-onbuild`](#maven339-jdk-8-onbuild)
-	[`maven:3.3.9-onbuild`](#maven339-onbuild)
-	[`maven:3.3-jdk-8-onbuild`](#maven33-jdk-8-onbuild)
-	[`maven:3.3-onbuild`](#maven33-onbuild)
-	[`maven:3-jdk-8-onbuild`](#maven3-jdk-8-onbuild)
-	[`maven:3-onbuild`](#maven3-onbuild)
-	[`maven:onbuild`](#mavenonbuild)
-	[`maven:3.3.9-jdk-8-alpine`](#maven339-jdk-8-alpine)
-	[`maven:3.3.9-alpine`](#maven339-alpine)
-	[`maven:3.3-jdk-8-alpine`](#maven33-jdk-8-alpine)
-	[`maven:3.3-alpine`](#maven33-alpine)
-	[`maven:3-jdk-8-alpine`](#maven3-jdk-8-alpine)
-	[`maven:3-alpine`](#maven3-alpine)
-	[`maven:alpine`](#mavenalpine)
-	[`maven:3.3.9-jdk-8-onbuild-alpine`](#maven339-jdk-8-onbuild-alpine)
-	[`maven:3.3.9-onbuild-alpine`](#maven339-onbuild-alpine)
-	[`maven:3.3-jdk-8-onbuild-alpine`](#maven33-jdk-8-onbuild-alpine)
-	[`maven:3.3-onbuild-alpine`](#maven33-onbuild-alpine)
-	[`maven:3-jdk-8-onbuild-alpine`](#maven3-jdk-8-onbuild-alpine)
-	[`maven:3-onbuild-alpine`](#maven3-onbuild-alpine)
-	[`maven:onbuild-alpine`](#mavenonbuild-alpine)
-	[`maven:3.3.9-jdk-9`](#maven339-jdk-9)
-	[`maven:3.3-jdk-9`](#maven33-jdk-9)
-	[`maven:3-jdk-9`](#maven3-jdk-9)
-	[`maven:3.3.9-jdk-9-onbuild`](#maven339-jdk-9-onbuild)
-	[`maven:3.3-jdk-9-onbuild`](#maven33-jdk-9-onbuild)
-	[`maven:3-jdk-9-onbuild`](#maven3-jdk-9-onbuild)

## `maven:3.3.9-jdk-7`

```console
$ docker pull maven@sha256:c5ee7303f6df0f4b723cf7b1199af9d3e8df5c3c25a4b7404ce09f64a4b26853
```

-	Platforms:
	-	linux; amd64

### `maven:3.3.9-jdk-7` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261216661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a6a9dbee6574e71cd3b94828f91e15b751da318acb046b50a2c3a59f708d589`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2016 20:07:29 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-7-openjdk-amd64
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_VERSION=7u111
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_DEBIAN_VERSION=7u111-2.6.7-1~deb8u1
# Fri, 21 Oct 2016 20:08:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-7-jdk="$JAVA_DEBIAN_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sat, 22 Oct 2016 06:58:19 GMT
ARG MAVEN_VERSION=3.3.9
# Sat, 22 Oct 2016 06:58:19 GMT
ARG USER_HOME_DIR=/root
# Sat, 22 Oct 2016 06:58:21 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 22 Oct 2016 06:58:21 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 22 Oct 2016 06:58:22 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 22 Oct 2016 06:58:22 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 22 Oct 2016 06:58:23 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Sat, 22 Oct 2016 06:58:23 GMT
VOLUME [/root/.m2]
# Sat, 22 Oct 2016 06:58:24 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 22 Oct 2016 06:58:24 GMT
CMD ["mvn"]
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38af4ea2aca2dd9fdaa2d741cf500f2bef515d779d6aa7bf31894774ffda697`  
		Last Modified: Fri, 21 Oct 2016 20:08:26 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31eee7b5a62519285e299108528b0cbf68a03995b9a6da049d7a9283707615e`  
		Last Modified: Fri, 21 Oct 2016 20:08:53 GMT  
		Size: 139.6 MB (139641458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72d97f0bcb304dcdf07e1dda800e3c4703c5cd6393189f42a6321f847db9782`  
		Last Modified: Sat, 22 Oct 2016 06:58:36 GMT  
		Size: 8.6 MB (8598849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ff66b2c778cf79b7818e49ab7c174366f35ef915ff46301a63d95ab0256142`  
		Last Modified: Sat, 22 Oct 2016 06:58:34 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80b16ca10122efa382531be1f764c5fa93bb7440556180dcf4de878fd094b4f`  
		Last Modified: Sat, 22 Oct 2016 06:58:34 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3-jdk-7`

```console
$ docker pull maven@sha256:c5ee7303f6df0f4b723cf7b1199af9d3e8df5c3c25a4b7404ce09f64a4b26853
```

-	Platforms:
	-	linux; amd64

### `maven:3.3-jdk-7` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261216661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a6a9dbee6574e71cd3b94828f91e15b751da318acb046b50a2c3a59f708d589`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2016 20:07:29 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-7-openjdk-amd64
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_VERSION=7u111
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_DEBIAN_VERSION=7u111-2.6.7-1~deb8u1
# Fri, 21 Oct 2016 20:08:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-7-jdk="$JAVA_DEBIAN_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sat, 22 Oct 2016 06:58:19 GMT
ARG MAVEN_VERSION=3.3.9
# Sat, 22 Oct 2016 06:58:19 GMT
ARG USER_HOME_DIR=/root
# Sat, 22 Oct 2016 06:58:21 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 22 Oct 2016 06:58:21 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 22 Oct 2016 06:58:22 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 22 Oct 2016 06:58:22 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 22 Oct 2016 06:58:23 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Sat, 22 Oct 2016 06:58:23 GMT
VOLUME [/root/.m2]
# Sat, 22 Oct 2016 06:58:24 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 22 Oct 2016 06:58:24 GMT
CMD ["mvn"]
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38af4ea2aca2dd9fdaa2d741cf500f2bef515d779d6aa7bf31894774ffda697`  
		Last Modified: Fri, 21 Oct 2016 20:08:26 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31eee7b5a62519285e299108528b0cbf68a03995b9a6da049d7a9283707615e`  
		Last Modified: Fri, 21 Oct 2016 20:08:53 GMT  
		Size: 139.6 MB (139641458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72d97f0bcb304dcdf07e1dda800e3c4703c5cd6393189f42a6321f847db9782`  
		Last Modified: Sat, 22 Oct 2016 06:58:36 GMT  
		Size: 8.6 MB (8598849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ff66b2c778cf79b7818e49ab7c174366f35ef915ff46301a63d95ab0256142`  
		Last Modified: Sat, 22 Oct 2016 06:58:34 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80b16ca10122efa382531be1f764c5fa93bb7440556180dcf4de878fd094b4f`  
		Last Modified: Sat, 22 Oct 2016 06:58:34 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3-jdk-7`

```console
$ docker pull maven@sha256:c5ee7303f6df0f4b723cf7b1199af9d3e8df5c3c25a4b7404ce09f64a4b26853
```

-	Platforms:
	-	linux; amd64

### `maven:3-jdk-7` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261216661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a6a9dbee6574e71cd3b94828f91e15b751da318acb046b50a2c3a59f708d589`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2016 20:07:29 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-7-openjdk-amd64
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_VERSION=7u111
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_DEBIAN_VERSION=7u111-2.6.7-1~deb8u1
# Fri, 21 Oct 2016 20:08:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-7-jdk="$JAVA_DEBIAN_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sat, 22 Oct 2016 06:58:19 GMT
ARG MAVEN_VERSION=3.3.9
# Sat, 22 Oct 2016 06:58:19 GMT
ARG USER_HOME_DIR=/root
# Sat, 22 Oct 2016 06:58:21 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 22 Oct 2016 06:58:21 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 22 Oct 2016 06:58:22 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 22 Oct 2016 06:58:22 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 22 Oct 2016 06:58:23 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Sat, 22 Oct 2016 06:58:23 GMT
VOLUME [/root/.m2]
# Sat, 22 Oct 2016 06:58:24 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 22 Oct 2016 06:58:24 GMT
CMD ["mvn"]
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38af4ea2aca2dd9fdaa2d741cf500f2bef515d779d6aa7bf31894774ffda697`  
		Last Modified: Fri, 21 Oct 2016 20:08:26 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31eee7b5a62519285e299108528b0cbf68a03995b9a6da049d7a9283707615e`  
		Last Modified: Fri, 21 Oct 2016 20:08:53 GMT  
		Size: 139.6 MB (139641458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72d97f0bcb304dcdf07e1dda800e3c4703c5cd6393189f42a6321f847db9782`  
		Last Modified: Sat, 22 Oct 2016 06:58:36 GMT  
		Size: 8.6 MB (8598849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ff66b2c778cf79b7818e49ab7c174366f35ef915ff46301a63d95ab0256142`  
		Last Modified: Sat, 22 Oct 2016 06:58:34 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80b16ca10122efa382531be1f764c5fa93bb7440556180dcf4de878fd094b4f`  
		Last Modified: Sat, 22 Oct 2016 06:58:34 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3.9-jdk-7-onbuild`

```console
$ docker pull maven@sha256:8e1abd0619aefc42fb3500aeb9447fe23478e8bdeced7638d9a1ca464b8828ea
```

-	Platforms:
	-	linux; amd64

### `maven:3.3.9-jdk-7-onbuild` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261216819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102e0b5a4ffa90ec086868fb6fa0d105f15b5044b2e074bd7f22e1d2dac17d19`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2016 20:07:29 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-7-openjdk-amd64
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_VERSION=7u111
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_DEBIAN_VERSION=7u111-2.6.7-1~deb8u1
# Fri, 21 Oct 2016 20:08:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-7-jdk="$JAVA_DEBIAN_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sat, 22 Oct 2016 06:58:19 GMT
ARG MAVEN_VERSION=3.3.9
# Sat, 22 Oct 2016 06:58:19 GMT
ARG USER_HOME_DIR=/root
# Sat, 22 Oct 2016 06:58:21 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 22 Oct 2016 06:58:21 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 22 Oct 2016 06:58:22 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 22 Oct 2016 06:58:22 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 22 Oct 2016 06:58:23 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Sat, 22 Oct 2016 06:58:23 GMT
VOLUME [/root/.m2]
# Sat, 22 Oct 2016 06:58:24 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 22 Oct 2016 06:58:24 GMT
CMD ["mvn"]
# Sat, 22 Oct 2016 06:59:06 GMT
RUN mkdir -p /usr/src/app
# Sat, 22 Oct 2016 06:59:06 GMT
WORKDIR /usr/src/app
# Sat, 22 Oct 2016 06:59:07 GMT
ONBUILD ADD . /usr/src/app
# Sat, 22 Oct 2016 06:59:07 GMT
ONBUILD RUN mvn install
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38af4ea2aca2dd9fdaa2d741cf500f2bef515d779d6aa7bf31894774ffda697`  
		Last Modified: Fri, 21 Oct 2016 20:08:26 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31eee7b5a62519285e299108528b0cbf68a03995b9a6da049d7a9283707615e`  
		Last Modified: Fri, 21 Oct 2016 20:08:53 GMT  
		Size: 139.6 MB (139641458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72d97f0bcb304dcdf07e1dda800e3c4703c5cd6393189f42a6321f847db9782`  
		Last Modified: Sat, 22 Oct 2016 06:58:36 GMT  
		Size: 8.6 MB (8598849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ff66b2c778cf79b7818e49ab7c174366f35ef915ff46301a63d95ab0256142`  
		Last Modified: Sat, 22 Oct 2016 06:58:34 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80b16ca10122efa382531be1f764c5fa93bb7440556180dcf4de878fd094b4f`  
		Last Modified: Sat, 22 Oct 2016 06:58:34 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676a0eb7d8d8f464e5c9647023e3850919c84f6f30539e8fef82b88de87f991a`  
		Last Modified: Sat, 22 Oct 2016 06:59:17 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3-jdk-7-onbuild`

```console
$ docker pull maven@sha256:8e1abd0619aefc42fb3500aeb9447fe23478e8bdeced7638d9a1ca464b8828ea
```

-	Platforms:
	-	linux; amd64

### `maven:3.3-jdk-7-onbuild` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261216819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102e0b5a4ffa90ec086868fb6fa0d105f15b5044b2e074bd7f22e1d2dac17d19`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2016 20:07:29 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-7-openjdk-amd64
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_VERSION=7u111
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_DEBIAN_VERSION=7u111-2.6.7-1~deb8u1
# Fri, 21 Oct 2016 20:08:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-7-jdk="$JAVA_DEBIAN_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sat, 22 Oct 2016 06:58:19 GMT
ARG MAVEN_VERSION=3.3.9
# Sat, 22 Oct 2016 06:58:19 GMT
ARG USER_HOME_DIR=/root
# Sat, 22 Oct 2016 06:58:21 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 22 Oct 2016 06:58:21 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 22 Oct 2016 06:58:22 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 22 Oct 2016 06:58:22 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 22 Oct 2016 06:58:23 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Sat, 22 Oct 2016 06:58:23 GMT
VOLUME [/root/.m2]
# Sat, 22 Oct 2016 06:58:24 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 22 Oct 2016 06:58:24 GMT
CMD ["mvn"]
# Sat, 22 Oct 2016 06:59:06 GMT
RUN mkdir -p /usr/src/app
# Sat, 22 Oct 2016 06:59:06 GMT
WORKDIR /usr/src/app
# Sat, 22 Oct 2016 06:59:07 GMT
ONBUILD ADD . /usr/src/app
# Sat, 22 Oct 2016 06:59:07 GMT
ONBUILD RUN mvn install
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38af4ea2aca2dd9fdaa2d741cf500f2bef515d779d6aa7bf31894774ffda697`  
		Last Modified: Fri, 21 Oct 2016 20:08:26 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31eee7b5a62519285e299108528b0cbf68a03995b9a6da049d7a9283707615e`  
		Last Modified: Fri, 21 Oct 2016 20:08:53 GMT  
		Size: 139.6 MB (139641458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72d97f0bcb304dcdf07e1dda800e3c4703c5cd6393189f42a6321f847db9782`  
		Last Modified: Sat, 22 Oct 2016 06:58:36 GMT  
		Size: 8.6 MB (8598849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ff66b2c778cf79b7818e49ab7c174366f35ef915ff46301a63d95ab0256142`  
		Last Modified: Sat, 22 Oct 2016 06:58:34 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80b16ca10122efa382531be1f764c5fa93bb7440556180dcf4de878fd094b4f`  
		Last Modified: Sat, 22 Oct 2016 06:58:34 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676a0eb7d8d8f464e5c9647023e3850919c84f6f30539e8fef82b88de87f991a`  
		Last Modified: Sat, 22 Oct 2016 06:59:17 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3-jdk-7-onbuild`

```console
$ docker pull maven@sha256:8e1abd0619aefc42fb3500aeb9447fe23478e8bdeced7638d9a1ca464b8828ea
```

-	Platforms:
	-	linux; amd64

### `maven:3-jdk-7-onbuild` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261216819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102e0b5a4ffa90ec086868fb6fa0d105f15b5044b2e074bd7f22e1d2dac17d19`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2016 20:07:29 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-7-openjdk-amd64
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_VERSION=7u111
# Fri, 21 Oct 2016 20:07:30 GMT
ENV JAVA_DEBIAN_VERSION=7u111-2.6.7-1~deb8u1
# Fri, 21 Oct 2016 20:08:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-7-jdk="$JAVA_DEBIAN_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sat, 22 Oct 2016 06:58:19 GMT
ARG MAVEN_VERSION=3.3.9
# Sat, 22 Oct 2016 06:58:19 GMT
ARG USER_HOME_DIR=/root
# Sat, 22 Oct 2016 06:58:21 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 22 Oct 2016 06:58:21 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 22 Oct 2016 06:58:22 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 22 Oct 2016 06:58:22 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 22 Oct 2016 06:58:23 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Sat, 22 Oct 2016 06:58:23 GMT
VOLUME [/root/.m2]
# Sat, 22 Oct 2016 06:58:24 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 22 Oct 2016 06:58:24 GMT
CMD ["mvn"]
# Sat, 22 Oct 2016 06:59:06 GMT
RUN mkdir -p /usr/src/app
# Sat, 22 Oct 2016 06:59:06 GMT
WORKDIR /usr/src/app
# Sat, 22 Oct 2016 06:59:07 GMT
ONBUILD ADD . /usr/src/app
# Sat, 22 Oct 2016 06:59:07 GMT
ONBUILD RUN mvn install
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38af4ea2aca2dd9fdaa2d741cf500f2bef515d779d6aa7bf31894774ffda697`  
		Last Modified: Fri, 21 Oct 2016 20:08:26 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31eee7b5a62519285e299108528b0cbf68a03995b9a6da049d7a9283707615e`  
		Last Modified: Fri, 21 Oct 2016 20:08:53 GMT  
		Size: 139.6 MB (139641458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72d97f0bcb304dcdf07e1dda800e3c4703c5cd6393189f42a6321f847db9782`  
		Last Modified: Sat, 22 Oct 2016 06:58:36 GMT  
		Size: 8.6 MB (8598849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ff66b2c778cf79b7818e49ab7c174366f35ef915ff46301a63d95ab0256142`  
		Last Modified: Sat, 22 Oct 2016 06:58:34 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80b16ca10122efa382531be1f764c5fa93bb7440556180dcf4de878fd094b4f`  
		Last Modified: Sat, 22 Oct 2016 06:58:34 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676a0eb7d8d8f464e5c9647023e3850919c84f6f30539e8fef82b88de87f991a`  
		Last Modified: Sat, 22 Oct 2016 06:59:17 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3.9-jdk-7-alpine`

```console
$ docker pull maven@sha256:b1b2431649f8ff42ff95e17a1646d0428fbcfa00956fed652110c8efeae93e14
```

-	Platforms:
	-	linux; amd64

### `maven:3.3.9-jdk-7-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.2 MB (88193521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08db7b90e3f2f037a278299fce9513df286fbbd76282322be9ebae16fb2d319a`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:39:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.7-openjdk
# Tue, 18 Oct 2016 20:39:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.7-openjdk/jre/bin:/usr/lib/jvm/java-1.7-openjdk/bin
# Wed, 19 Oct 2016 22:02:07 GMT
ENV JAVA_VERSION=7u111
# Wed, 19 Oct 2016 22:02:07 GMT
ENV JAVA_ALPINE_VERSION=7.111.2.6.7-r2
# Wed, 19 Oct 2016 22:02:17 GMT
RUN set -x 	&& apk add --no-cache 		openjdk7="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 20 Oct 2016 00:55:24 GMT
RUN apk add --no-cache curl tar bash
# Thu, 20 Oct 2016 00:55:24 GMT
ARG MAVEN_VERSION=3.3.9
# Thu, 20 Oct 2016 00:55:25 GMT
ARG USER_HOME_DIR=/root
# Thu, 20 Oct 2016 00:55:26 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 20 Oct 2016 00:55:26 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 20 Oct 2016 00:55:27 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 20 Oct 2016 00:55:27 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 20 Oct 2016 00:55:28 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Thu, 20 Oct 2016 00:55:28 GMT
VOLUME [/root/.m2]
# Thu, 20 Oct 2016 00:55:29 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 20 Oct 2016 00:55:29 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e87eeb13ad9ed22981f9c0b7753f79568a84073d032ad7ac2310f0b494bfa1a`  
		Last Modified: Wed, 19 Oct 2016 22:06:24 GMT  
		Size: 75.5 MB (75549480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732c0fe2ddbc61e0483324efd0d4de1618742bc31745ae7bcd198c53ebe80b3e`  
		Last Modified: Thu, 20 Oct 2016 00:55:40 GMT  
		Size: 1.7 MB (1730974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c554515083d008a13d6a788009632fea3861de2a0a3fd506e28e5465ad8c910`  
		Last Modified: Thu, 20 Oct 2016 00:55:40 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517c1119d772706ad7049b420e73bae6a0b249bdb5d08d55f58f979fb5b80b90`  
		Last Modified: Thu, 20 Oct 2016 00:55:38 GMT  
		Size: 686.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c415d1171cba9e5ddfa7e2905d47d597d49b7145f638d45ddefd8905ea601dc3`  
		Last Modified: Thu, 20 Oct 2016 00:55:39 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3-jdk-7-alpine`

```console
$ docker pull maven@sha256:b1b2431649f8ff42ff95e17a1646d0428fbcfa00956fed652110c8efeae93e14
```

-	Platforms:
	-	linux; amd64

### `maven:3.3-jdk-7-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.2 MB (88193521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08db7b90e3f2f037a278299fce9513df286fbbd76282322be9ebae16fb2d319a`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:39:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.7-openjdk
# Tue, 18 Oct 2016 20:39:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.7-openjdk/jre/bin:/usr/lib/jvm/java-1.7-openjdk/bin
# Wed, 19 Oct 2016 22:02:07 GMT
ENV JAVA_VERSION=7u111
# Wed, 19 Oct 2016 22:02:07 GMT
ENV JAVA_ALPINE_VERSION=7.111.2.6.7-r2
# Wed, 19 Oct 2016 22:02:17 GMT
RUN set -x 	&& apk add --no-cache 		openjdk7="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 20 Oct 2016 00:55:24 GMT
RUN apk add --no-cache curl tar bash
# Thu, 20 Oct 2016 00:55:24 GMT
ARG MAVEN_VERSION=3.3.9
# Thu, 20 Oct 2016 00:55:25 GMT
ARG USER_HOME_DIR=/root
# Thu, 20 Oct 2016 00:55:26 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 20 Oct 2016 00:55:26 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 20 Oct 2016 00:55:27 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 20 Oct 2016 00:55:27 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 20 Oct 2016 00:55:28 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Thu, 20 Oct 2016 00:55:28 GMT
VOLUME [/root/.m2]
# Thu, 20 Oct 2016 00:55:29 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 20 Oct 2016 00:55:29 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e87eeb13ad9ed22981f9c0b7753f79568a84073d032ad7ac2310f0b494bfa1a`  
		Last Modified: Wed, 19 Oct 2016 22:06:24 GMT  
		Size: 75.5 MB (75549480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732c0fe2ddbc61e0483324efd0d4de1618742bc31745ae7bcd198c53ebe80b3e`  
		Last Modified: Thu, 20 Oct 2016 00:55:40 GMT  
		Size: 1.7 MB (1730974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c554515083d008a13d6a788009632fea3861de2a0a3fd506e28e5465ad8c910`  
		Last Modified: Thu, 20 Oct 2016 00:55:40 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517c1119d772706ad7049b420e73bae6a0b249bdb5d08d55f58f979fb5b80b90`  
		Last Modified: Thu, 20 Oct 2016 00:55:38 GMT  
		Size: 686.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c415d1171cba9e5ddfa7e2905d47d597d49b7145f638d45ddefd8905ea601dc3`  
		Last Modified: Thu, 20 Oct 2016 00:55:39 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3-jdk-7-alpine`

```console
$ docker pull maven@sha256:b1b2431649f8ff42ff95e17a1646d0428fbcfa00956fed652110c8efeae93e14
```

-	Platforms:
	-	linux; amd64

### `maven:3-jdk-7-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.2 MB (88193521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08db7b90e3f2f037a278299fce9513df286fbbd76282322be9ebae16fb2d319a`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:39:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.7-openjdk
# Tue, 18 Oct 2016 20:39:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.7-openjdk/jre/bin:/usr/lib/jvm/java-1.7-openjdk/bin
# Wed, 19 Oct 2016 22:02:07 GMT
ENV JAVA_VERSION=7u111
# Wed, 19 Oct 2016 22:02:07 GMT
ENV JAVA_ALPINE_VERSION=7.111.2.6.7-r2
# Wed, 19 Oct 2016 22:02:17 GMT
RUN set -x 	&& apk add --no-cache 		openjdk7="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 20 Oct 2016 00:55:24 GMT
RUN apk add --no-cache curl tar bash
# Thu, 20 Oct 2016 00:55:24 GMT
ARG MAVEN_VERSION=3.3.9
# Thu, 20 Oct 2016 00:55:25 GMT
ARG USER_HOME_DIR=/root
# Thu, 20 Oct 2016 00:55:26 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 20 Oct 2016 00:55:26 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 20 Oct 2016 00:55:27 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 20 Oct 2016 00:55:27 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 20 Oct 2016 00:55:28 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Thu, 20 Oct 2016 00:55:28 GMT
VOLUME [/root/.m2]
# Thu, 20 Oct 2016 00:55:29 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 20 Oct 2016 00:55:29 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e87eeb13ad9ed22981f9c0b7753f79568a84073d032ad7ac2310f0b494bfa1a`  
		Last Modified: Wed, 19 Oct 2016 22:06:24 GMT  
		Size: 75.5 MB (75549480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732c0fe2ddbc61e0483324efd0d4de1618742bc31745ae7bcd198c53ebe80b3e`  
		Last Modified: Thu, 20 Oct 2016 00:55:40 GMT  
		Size: 1.7 MB (1730974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c554515083d008a13d6a788009632fea3861de2a0a3fd506e28e5465ad8c910`  
		Last Modified: Thu, 20 Oct 2016 00:55:40 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517c1119d772706ad7049b420e73bae6a0b249bdb5d08d55f58f979fb5b80b90`  
		Last Modified: Thu, 20 Oct 2016 00:55:38 GMT  
		Size: 686.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c415d1171cba9e5ddfa7e2905d47d597d49b7145f638d45ddefd8905ea601dc3`  
		Last Modified: Thu, 20 Oct 2016 00:55:39 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3.9-jdk-7-onbuild-alpine`

```console
$ docker pull maven@sha256:64d7bae17c74b6d088db30ce66c45164e35f0113f93be40757d0379aaa07b4b1
```

-	Platforms:
	-	linux; amd64

### `maven:3.3.9-jdk-7-onbuild-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.2 MB (88193678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40f03731dd99c6c6b166af94f4113b423d34f4168ce62315c65d6340ad3adfc`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:39:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.7-openjdk
# Tue, 18 Oct 2016 20:39:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.7-openjdk/jre/bin:/usr/lib/jvm/java-1.7-openjdk/bin
# Wed, 19 Oct 2016 22:02:07 GMT
ENV JAVA_VERSION=7u111
# Wed, 19 Oct 2016 22:02:07 GMT
ENV JAVA_ALPINE_VERSION=7.111.2.6.7-r2
# Wed, 19 Oct 2016 22:02:17 GMT
RUN set -x 	&& apk add --no-cache 		openjdk7="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 20 Oct 2016 00:55:24 GMT
RUN apk add --no-cache curl tar bash
# Thu, 20 Oct 2016 00:55:24 GMT
ARG MAVEN_VERSION=3.3.9
# Thu, 20 Oct 2016 00:55:25 GMT
ARG USER_HOME_DIR=/root
# Thu, 20 Oct 2016 00:55:26 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 20 Oct 2016 00:55:26 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 20 Oct 2016 00:55:27 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 20 Oct 2016 00:55:27 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 20 Oct 2016 00:55:28 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Thu, 20 Oct 2016 00:55:28 GMT
VOLUME [/root/.m2]
# Thu, 20 Oct 2016 00:55:29 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 20 Oct 2016 00:55:29 GMT
CMD ["mvn"]
# Thu, 20 Oct 2016 00:56:40 GMT
RUN mkdir -p /usr/src/app
# Thu, 20 Oct 2016 00:56:41 GMT
WORKDIR /usr/src/app
# Thu, 20 Oct 2016 00:56:41 GMT
ONBUILD ADD . /usr/src/app
# Thu, 20 Oct 2016 00:56:41 GMT
ONBUILD RUN mvn install
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e87eeb13ad9ed22981f9c0b7753f79568a84073d032ad7ac2310f0b494bfa1a`  
		Last Modified: Wed, 19 Oct 2016 22:06:24 GMT  
		Size: 75.5 MB (75549480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732c0fe2ddbc61e0483324efd0d4de1618742bc31745ae7bcd198c53ebe80b3e`  
		Last Modified: Thu, 20 Oct 2016 00:55:40 GMT  
		Size: 1.7 MB (1730974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c554515083d008a13d6a788009632fea3861de2a0a3fd506e28e5465ad8c910`  
		Last Modified: Thu, 20 Oct 2016 00:55:40 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517c1119d772706ad7049b420e73bae6a0b249bdb5d08d55f58f979fb5b80b90`  
		Last Modified: Thu, 20 Oct 2016 00:55:38 GMT  
		Size: 686.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c415d1171cba9e5ddfa7e2905d47d597d49b7145f638d45ddefd8905ea601dc3`  
		Last Modified: Thu, 20 Oct 2016 00:55:39 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d11c7260eb5dd976e238636215cd86dd597c02b62e1a0b7b7721751da647db4`  
		Last Modified: Thu, 20 Oct 2016 00:56:51 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3-jdk-7-onbuild-alpine`

```console
$ docker pull maven@sha256:64d7bae17c74b6d088db30ce66c45164e35f0113f93be40757d0379aaa07b4b1
```

-	Platforms:
	-	linux; amd64

### `maven:3.3-jdk-7-onbuild-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.2 MB (88193678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40f03731dd99c6c6b166af94f4113b423d34f4168ce62315c65d6340ad3adfc`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:39:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.7-openjdk
# Tue, 18 Oct 2016 20:39:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.7-openjdk/jre/bin:/usr/lib/jvm/java-1.7-openjdk/bin
# Wed, 19 Oct 2016 22:02:07 GMT
ENV JAVA_VERSION=7u111
# Wed, 19 Oct 2016 22:02:07 GMT
ENV JAVA_ALPINE_VERSION=7.111.2.6.7-r2
# Wed, 19 Oct 2016 22:02:17 GMT
RUN set -x 	&& apk add --no-cache 		openjdk7="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 20 Oct 2016 00:55:24 GMT
RUN apk add --no-cache curl tar bash
# Thu, 20 Oct 2016 00:55:24 GMT
ARG MAVEN_VERSION=3.3.9
# Thu, 20 Oct 2016 00:55:25 GMT
ARG USER_HOME_DIR=/root
# Thu, 20 Oct 2016 00:55:26 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 20 Oct 2016 00:55:26 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 20 Oct 2016 00:55:27 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 20 Oct 2016 00:55:27 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 20 Oct 2016 00:55:28 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Thu, 20 Oct 2016 00:55:28 GMT
VOLUME [/root/.m2]
# Thu, 20 Oct 2016 00:55:29 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 20 Oct 2016 00:55:29 GMT
CMD ["mvn"]
# Thu, 20 Oct 2016 00:56:40 GMT
RUN mkdir -p /usr/src/app
# Thu, 20 Oct 2016 00:56:41 GMT
WORKDIR /usr/src/app
# Thu, 20 Oct 2016 00:56:41 GMT
ONBUILD ADD . /usr/src/app
# Thu, 20 Oct 2016 00:56:41 GMT
ONBUILD RUN mvn install
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e87eeb13ad9ed22981f9c0b7753f79568a84073d032ad7ac2310f0b494bfa1a`  
		Last Modified: Wed, 19 Oct 2016 22:06:24 GMT  
		Size: 75.5 MB (75549480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732c0fe2ddbc61e0483324efd0d4de1618742bc31745ae7bcd198c53ebe80b3e`  
		Last Modified: Thu, 20 Oct 2016 00:55:40 GMT  
		Size: 1.7 MB (1730974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c554515083d008a13d6a788009632fea3861de2a0a3fd506e28e5465ad8c910`  
		Last Modified: Thu, 20 Oct 2016 00:55:40 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517c1119d772706ad7049b420e73bae6a0b249bdb5d08d55f58f979fb5b80b90`  
		Last Modified: Thu, 20 Oct 2016 00:55:38 GMT  
		Size: 686.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c415d1171cba9e5ddfa7e2905d47d597d49b7145f638d45ddefd8905ea601dc3`  
		Last Modified: Thu, 20 Oct 2016 00:55:39 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d11c7260eb5dd976e238636215cd86dd597c02b62e1a0b7b7721751da647db4`  
		Last Modified: Thu, 20 Oct 2016 00:56:51 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3-jdk-7-onbuild-alpine`

```console
$ docker pull maven@sha256:64d7bae17c74b6d088db30ce66c45164e35f0113f93be40757d0379aaa07b4b1
```

-	Platforms:
	-	linux; amd64

### `maven:3-jdk-7-onbuild-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.2 MB (88193678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40f03731dd99c6c6b166af94f4113b423d34f4168ce62315c65d6340ad3adfc`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:39:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.7-openjdk
# Tue, 18 Oct 2016 20:39:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.7-openjdk/jre/bin:/usr/lib/jvm/java-1.7-openjdk/bin
# Wed, 19 Oct 2016 22:02:07 GMT
ENV JAVA_VERSION=7u111
# Wed, 19 Oct 2016 22:02:07 GMT
ENV JAVA_ALPINE_VERSION=7.111.2.6.7-r2
# Wed, 19 Oct 2016 22:02:17 GMT
RUN set -x 	&& apk add --no-cache 		openjdk7="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 20 Oct 2016 00:55:24 GMT
RUN apk add --no-cache curl tar bash
# Thu, 20 Oct 2016 00:55:24 GMT
ARG MAVEN_VERSION=3.3.9
# Thu, 20 Oct 2016 00:55:25 GMT
ARG USER_HOME_DIR=/root
# Thu, 20 Oct 2016 00:55:26 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 20 Oct 2016 00:55:26 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 20 Oct 2016 00:55:27 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 20 Oct 2016 00:55:27 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 20 Oct 2016 00:55:28 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Thu, 20 Oct 2016 00:55:28 GMT
VOLUME [/root/.m2]
# Thu, 20 Oct 2016 00:55:29 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 20 Oct 2016 00:55:29 GMT
CMD ["mvn"]
# Thu, 20 Oct 2016 00:56:40 GMT
RUN mkdir -p /usr/src/app
# Thu, 20 Oct 2016 00:56:41 GMT
WORKDIR /usr/src/app
# Thu, 20 Oct 2016 00:56:41 GMT
ONBUILD ADD . /usr/src/app
# Thu, 20 Oct 2016 00:56:41 GMT
ONBUILD RUN mvn install
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e87eeb13ad9ed22981f9c0b7753f79568a84073d032ad7ac2310f0b494bfa1a`  
		Last Modified: Wed, 19 Oct 2016 22:06:24 GMT  
		Size: 75.5 MB (75549480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732c0fe2ddbc61e0483324efd0d4de1618742bc31745ae7bcd198c53ebe80b3e`  
		Last Modified: Thu, 20 Oct 2016 00:55:40 GMT  
		Size: 1.7 MB (1730974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c554515083d008a13d6a788009632fea3861de2a0a3fd506e28e5465ad8c910`  
		Last Modified: Thu, 20 Oct 2016 00:55:40 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517c1119d772706ad7049b420e73bae6a0b249bdb5d08d55f58f979fb5b80b90`  
		Last Modified: Thu, 20 Oct 2016 00:55:38 GMT  
		Size: 686.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c415d1171cba9e5ddfa7e2905d47d597d49b7145f638d45ddefd8905ea601dc3`  
		Last Modified: Thu, 20 Oct 2016 00:55:39 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d11c7260eb5dd976e238636215cd86dd597c02b62e1a0b7b7721751da647db4`  
		Last Modified: Thu, 20 Oct 2016 00:56:51 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3.9-jdk-8`

```console
$ docker pull maven@sha256:be5b9ccd2c36fe278f9684a93f728e4a42edd0aa0f00ae33e53ab2e75b0f09b1
```

-	Platforms:
	-	linux; amd64

### `maven:3.3.9-jdk-8` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251963805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59411589096b49aae6e8d1012fcb30146de18e0e7b59713b03c0efa02de27e7d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:53:47 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:53:48 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:53:49 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:53:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:54:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jdk="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:00 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 20:57:48 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 20:57:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 20:57:51 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 20:57:52 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 20:57:53 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 20:57:53 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 20:57:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 20:57:54 GMT
CMD ["mvn"]
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c6fc3e9968f5b8fb198a1ea206d24c695ca2ba720f3c60465eb766378eb661`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa8d5153bb17cb57f744591779c9cae37e3ce60ef7f251a06de8a52b4a5dc4`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc8d0fffcad18701b038c987358882834e50c5f8880d80e596b1b53a10452b`  
		Last Modified: Tue, 01 Nov 2016 05:35:36 GMT  
		Size: 130.1 MB (130104197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266a2a7ecbe81ae03360bc3e8bf9300175665db11e6d02fa7be79d485b530e`  
		Last Modified: Tue, 01 Nov 2016 05:34:58 GMT  
		Size: 284.2 KB (284198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e47e58a1da1cab2883e7bd00f19d95c09a7d0259e395de0f693f876c016ce6b`  
		Last Modified: Tue, 01 Nov 2016 20:58:08 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195755e92dd5148b2406cadaa8faba615b59375d5ce8e0101125ae5f7a9c875b`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780defcebf1af6f69fb32b4b775410ef0b3a533d7206d0802fb47992e6939246`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3.9`

```console
$ docker pull maven@sha256:be5b9ccd2c36fe278f9684a93f728e4a42edd0aa0f00ae33e53ab2e75b0f09b1
```

-	Platforms:
	-	linux; amd64

### `maven:3.3.9` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251963805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59411589096b49aae6e8d1012fcb30146de18e0e7b59713b03c0efa02de27e7d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:53:47 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:53:48 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:53:49 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:53:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:54:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jdk="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:00 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 20:57:48 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 20:57:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 20:57:51 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 20:57:52 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 20:57:53 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 20:57:53 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 20:57:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 20:57:54 GMT
CMD ["mvn"]
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c6fc3e9968f5b8fb198a1ea206d24c695ca2ba720f3c60465eb766378eb661`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa8d5153bb17cb57f744591779c9cae37e3ce60ef7f251a06de8a52b4a5dc4`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc8d0fffcad18701b038c987358882834e50c5f8880d80e596b1b53a10452b`  
		Last Modified: Tue, 01 Nov 2016 05:35:36 GMT  
		Size: 130.1 MB (130104197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266a2a7ecbe81ae03360bc3e8bf9300175665db11e6d02fa7be79d485b530e`  
		Last Modified: Tue, 01 Nov 2016 05:34:58 GMT  
		Size: 284.2 KB (284198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e47e58a1da1cab2883e7bd00f19d95c09a7d0259e395de0f693f876c016ce6b`  
		Last Modified: Tue, 01 Nov 2016 20:58:08 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195755e92dd5148b2406cadaa8faba615b59375d5ce8e0101125ae5f7a9c875b`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780defcebf1af6f69fb32b4b775410ef0b3a533d7206d0802fb47992e6939246`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3-jdk-8`

```console
$ docker pull maven@sha256:be5b9ccd2c36fe278f9684a93f728e4a42edd0aa0f00ae33e53ab2e75b0f09b1
```

-	Platforms:
	-	linux; amd64

### `maven:3.3-jdk-8` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251963805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59411589096b49aae6e8d1012fcb30146de18e0e7b59713b03c0efa02de27e7d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:53:47 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:53:48 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:53:49 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:53:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:54:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jdk="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:00 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 20:57:48 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 20:57:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 20:57:51 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 20:57:52 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 20:57:53 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 20:57:53 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 20:57:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 20:57:54 GMT
CMD ["mvn"]
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c6fc3e9968f5b8fb198a1ea206d24c695ca2ba720f3c60465eb766378eb661`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa8d5153bb17cb57f744591779c9cae37e3ce60ef7f251a06de8a52b4a5dc4`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc8d0fffcad18701b038c987358882834e50c5f8880d80e596b1b53a10452b`  
		Last Modified: Tue, 01 Nov 2016 05:35:36 GMT  
		Size: 130.1 MB (130104197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266a2a7ecbe81ae03360bc3e8bf9300175665db11e6d02fa7be79d485b530e`  
		Last Modified: Tue, 01 Nov 2016 05:34:58 GMT  
		Size: 284.2 KB (284198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e47e58a1da1cab2883e7bd00f19d95c09a7d0259e395de0f693f876c016ce6b`  
		Last Modified: Tue, 01 Nov 2016 20:58:08 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195755e92dd5148b2406cadaa8faba615b59375d5ce8e0101125ae5f7a9c875b`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780defcebf1af6f69fb32b4b775410ef0b3a533d7206d0802fb47992e6939246`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3`

```console
$ docker pull maven@sha256:be5b9ccd2c36fe278f9684a93f728e4a42edd0aa0f00ae33e53ab2e75b0f09b1
```

-	Platforms:
	-	linux; amd64

### `maven:3.3` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251963805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59411589096b49aae6e8d1012fcb30146de18e0e7b59713b03c0efa02de27e7d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:53:47 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:53:48 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:53:49 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:53:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:54:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jdk="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:00 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 20:57:48 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 20:57:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 20:57:51 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 20:57:52 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 20:57:53 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 20:57:53 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 20:57:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 20:57:54 GMT
CMD ["mvn"]
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c6fc3e9968f5b8fb198a1ea206d24c695ca2ba720f3c60465eb766378eb661`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa8d5153bb17cb57f744591779c9cae37e3ce60ef7f251a06de8a52b4a5dc4`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc8d0fffcad18701b038c987358882834e50c5f8880d80e596b1b53a10452b`  
		Last Modified: Tue, 01 Nov 2016 05:35:36 GMT  
		Size: 130.1 MB (130104197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266a2a7ecbe81ae03360bc3e8bf9300175665db11e6d02fa7be79d485b530e`  
		Last Modified: Tue, 01 Nov 2016 05:34:58 GMT  
		Size: 284.2 KB (284198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e47e58a1da1cab2883e7bd00f19d95c09a7d0259e395de0f693f876c016ce6b`  
		Last Modified: Tue, 01 Nov 2016 20:58:08 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195755e92dd5148b2406cadaa8faba615b59375d5ce8e0101125ae5f7a9c875b`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780defcebf1af6f69fb32b4b775410ef0b3a533d7206d0802fb47992e6939246`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3-jdk-8`

```console
$ docker pull maven@sha256:be5b9ccd2c36fe278f9684a93f728e4a42edd0aa0f00ae33e53ab2e75b0f09b1
```

-	Platforms:
	-	linux; amd64

### `maven:3-jdk-8` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251963805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59411589096b49aae6e8d1012fcb30146de18e0e7b59713b03c0efa02de27e7d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:53:47 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:53:48 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:53:49 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:53:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:54:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jdk="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:00 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 20:57:48 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 20:57:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 20:57:51 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 20:57:52 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 20:57:53 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 20:57:53 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 20:57:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 20:57:54 GMT
CMD ["mvn"]
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c6fc3e9968f5b8fb198a1ea206d24c695ca2ba720f3c60465eb766378eb661`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa8d5153bb17cb57f744591779c9cae37e3ce60ef7f251a06de8a52b4a5dc4`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc8d0fffcad18701b038c987358882834e50c5f8880d80e596b1b53a10452b`  
		Last Modified: Tue, 01 Nov 2016 05:35:36 GMT  
		Size: 130.1 MB (130104197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266a2a7ecbe81ae03360bc3e8bf9300175665db11e6d02fa7be79d485b530e`  
		Last Modified: Tue, 01 Nov 2016 05:34:58 GMT  
		Size: 284.2 KB (284198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e47e58a1da1cab2883e7bd00f19d95c09a7d0259e395de0f693f876c016ce6b`  
		Last Modified: Tue, 01 Nov 2016 20:58:08 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195755e92dd5148b2406cadaa8faba615b59375d5ce8e0101125ae5f7a9c875b`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780defcebf1af6f69fb32b4b775410ef0b3a533d7206d0802fb47992e6939246`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3`

```console
$ docker pull maven@sha256:be5b9ccd2c36fe278f9684a93f728e4a42edd0aa0f00ae33e53ab2e75b0f09b1
```

-	Platforms:
	-	linux; amd64

### `maven:3` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251963805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59411589096b49aae6e8d1012fcb30146de18e0e7b59713b03c0efa02de27e7d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:53:47 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:53:48 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:53:49 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:53:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:54:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jdk="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:00 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 20:57:48 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 20:57:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 20:57:51 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 20:57:52 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 20:57:53 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 20:57:53 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 20:57:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 20:57:54 GMT
CMD ["mvn"]
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c6fc3e9968f5b8fb198a1ea206d24c695ca2ba720f3c60465eb766378eb661`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa8d5153bb17cb57f744591779c9cae37e3ce60ef7f251a06de8a52b4a5dc4`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc8d0fffcad18701b038c987358882834e50c5f8880d80e596b1b53a10452b`  
		Last Modified: Tue, 01 Nov 2016 05:35:36 GMT  
		Size: 130.1 MB (130104197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266a2a7ecbe81ae03360bc3e8bf9300175665db11e6d02fa7be79d485b530e`  
		Last Modified: Tue, 01 Nov 2016 05:34:58 GMT  
		Size: 284.2 KB (284198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e47e58a1da1cab2883e7bd00f19d95c09a7d0259e395de0f693f876c016ce6b`  
		Last Modified: Tue, 01 Nov 2016 20:58:08 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195755e92dd5148b2406cadaa8faba615b59375d5ce8e0101125ae5f7a9c875b`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780defcebf1af6f69fb32b4b775410ef0b3a533d7206d0802fb47992e6939246`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:latest`

```console
$ docker pull maven@sha256:be5b9ccd2c36fe278f9684a93f728e4a42edd0aa0f00ae33e53ab2e75b0f09b1
```

-	Platforms:
	-	linux; amd64

### `maven:latest` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251963805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59411589096b49aae6e8d1012fcb30146de18e0e7b59713b03c0efa02de27e7d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:53:47 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:53:48 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:53:49 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:53:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:54:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jdk="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:00 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 20:57:48 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 20:57:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 20:57:51 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 20:57:52 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 20:57:53 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 20:57:53 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 20:57:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 20:57:54 GMT
CMD ["mvn"]
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c6fc3e9968f5b8fb198a1ea206d24c695ca2ba720f3c60465eb766378eb661`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa8d5153bb17cb57f744591779c9cae37e3ce60ef7f251a06de8a52b4a5dc4`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc8d0fffcad18701b038c987358882834e50c5f8880d80e596b1b53a10452b`  
		Last Modified: Tue, 01 Nov 2016 05:35:36 GMT  
		Size: 130.1 MB (130104197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266a2a7ecbe81ae03360bc3e8bf9300175665db11e6d02fa7be79d485b530e`  
		Last Modified: Tue, 01 Nov 2016 05:34:58 GMT  
		Size: 284.2 KB (284198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e47e58a1da1cab2883e7bd00f19d95c09a7d0259e395de0f693f876c016ce6b`  
		Last Modified: Tue, 01 Nov 2016 20:58:08 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195755e92dd5148b2406cadaa8faba615b59375d5ce8e0101125ae5f7a9c875b`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780defcebf1af6f69fb32b4b775410ef0b3a533d7206d0802fb47992e6939246`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3.9-jdk-8-onbuild`

```console
$ docker pull maven@sha256:651183b4b67ea32ca4931944fa714e9dcaf52409a221b0551c87d38cf723ef39
```

-	Platforms:
	-	linux; amd64

### `maven:3.3.9-jdk-8-onbuild` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251963962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849fb4dad2fc29ef0f3d83ca7119766c4bfe945f8f085677430d12b28b76aac3`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:53:47 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:53:48 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:53:49 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:53:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:54:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jdk="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:00 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 20:57:48 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 20:57:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 20:57:51 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 20:57:52 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 20:57:53 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 20:57:53 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 20:57:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 20:57:54 GMT
CMD ["mvn"]
# Tue, 01 Nov 2016 21:03:24 GMT
RUN mkdir -p /usr/src/app
# Tue, 01 Nov 2016 21:03:24 GMT
WORKDIR /usr/src/app
# Tue, 01 Nov 2016 21:03:25 GMT
ONBUILD ADD . /usr/src/app
# Tue, 01 Nov 2016 21:03:25 GMT
ONBUILD RUN mvn install
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c6fc3e9968f5b8fb198a1ea206d24c695ca2ba720f3c60465eb766378eb661`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa8d5153bb17cb57f744591779c9cae37e3ce60ef7f251a06de8a52b4a5dc4`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc8d0fffcad18701b038c987358882834e50c5f8880d80e596b1b53a10452b`  
		Last Modified: Tue, 01 Nov 2016 05:35:36 GMT  
		Size: 130.1 MB (130104197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266a2a7ecbe81ae03360bc3e8bf9300175665db11e6d02fa7be79d485b530e`  
		Last Modified: Tue, 01 Nov 2016 05:34:58 GMT  
		Size: 284.2 KB (284198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e47e58a1da1cab2883e7bd00f19d95c09a7d0259e395de0f693f876c016ce6b`  
		Last Modified: Tue, 01 Nov 2016 20:58:08 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195755e92dd5148b2406cadaa8faba615b59375d5ce8e0101125ae5f7a9c875b`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780defcebf1af6f69fb32b4b775410ef0b3a533d7206d0802fb47992e6939246`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43613224a1ef011b49fa7d0d93a0922bc1f8441b463b59e8cfb1467ab36d72b8`  
		Last Modified: Tue, 01 Nov 2016 21:03:36 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3.9-onbuild`

```console
$ docker pull maven@sha256:651183b4b67ea32ca4931944fa714e9dcaf52409a221b0551c87d38cf723ef39
```

-	Platforms:
	-	linux; amd64

### `maven:3.3.9-onbuild` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251963962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849fb4dad2fc29ef0f3d83ca7119766c4bfe945f8f085677430d12b28b76aac3`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:53:47 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:53:48 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:53:49 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:53:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:54:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jdk="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:00 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 20:57:48 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 20:57:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 20:57:51 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 20:57:52 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 20:57:53 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 20:57:53 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 20:57:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 20:57:54 GMT
CMD ["mvn"]
# Tue, 01 Nov 2016 21:03:24 GMT
RUN mkdir -p /usr/src/app
# Tue, 01 Nov 2016 21:03:24 GMT
WORKDIR /usr/src/app
# Tue, 01 Nov 2016 21:03:25 GMT
ONBUILD ADD . /usr/src/app
# Tue, 01 Nov 2016 21:03:25 GMT
ONBUILD RUN mvn install
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c6fc3e9968f5b8fb198a1ea206d24c695ca2ba720f3c60465eb766378eb661`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa8d5153bb17cb57f744591779c9cae37e3ce60ef7f251a06de8a52b4a5dc4`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc8d0fffcad18701b038c987358882834e50c5f8880d80e596b1b53a10452b`  
		Last Modified: Tue, 01 Nov 2016 05:35:36 GMT  
		Size: 130.1 MB (130104197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266a2a7ecbe81ae03360bc3e8bf9300175665db11e6d02fa7be79d485b530e`  
		Last Modified: Tue, 01 Nov 2016 05:34:58 GMT  
		Size: 284.2 KB (284198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e47e58a1da1cab2883e7bd00f19d95c09a7d0259e395de0f693f876c016ce6b`  
		Last Modified: Tue, 01 Nov 2016 20:58:08 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195755e92dd5148b2406cadaa8faba615b59375d5ce8e0101125ae5f7a9c875b`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780defcebf1af6f69fb32b4b775410ef0b3a533d7206d0802fb47992e6939246`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43613224a1ef011b49fa7d0d93a0922bc1f8441b463b59e8cfb1467ab36d72b8`  
		Last Modified: Tue, 01 Nov 2016 21:03:36 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3-jdk-8-onbuild`

```console
$ docker pull maven@sha256:651183b4b67ea32ca4931944fa714e9dcaf52409a221b0551c87d38cf723ef39
```

-	Platforms:
	-	linux; amd64

### `maven:3.3-jdk-8-onbuild` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251963962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849fb4dad2fc29ef0f3d83ca7119766c4bfe945f8f085677430d12b28b76aac3`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:53:47 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:53:48 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:53:49 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:53:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:54:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jdk="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:00 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 20:57:48 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 20:57:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 20:57:51 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 20:57:52 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 20:57:53 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 20:57:53 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 20:57:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 20:57:54 GMT
CMD ["mvn"]
# Tue, 01 Nov 2016 21:03:24 GMT
RUN mkdir -p /usr/src/app
# Tue, 01 Nov 2016 21:03:24 GMT
WORKDIR /usr/src/app
# Tue, 01 Nov 2016 21:03:25 GMT
ONBUILD ADD . /usr/src/app
# Tue, 01 Nov 2016 21:03:25 GMT
ONBUILD RUN mvn install
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c6fc3e9968f5b8fb198a1ea206d24c695ca2ba720f3c60465eb766378eb661`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa8d5153bb17cb57f744591779c9cae37e3ce60ef7f251a06de8a52b4a5dc4`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc8d0fffcad18701b038c987358882834e50c5f8880d80e596b1b53a10452b`  
		Last Modified: Tue, 01 Nov 2016 05:35:36 GMT  
		Size: 130.1 MB (130104197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266a2a7ecbe81ae03360bc3e8bf9300175665db11e6d02fa7be79d485b530e`  
		Last Modified: Tue, 01 Nov 2016 05:34:58 GMT  
		Size: 284.2 KB (284198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e47e58a1da1cab2883e7bd00f19d95c09a7d0259e395de0f693f876c016ce6b`  
		Last Modified: Tue, 01 Nov 2016 20:58:08 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195755e92dd5148b2406cadaa8faba615b59375d5ce8e0101125ae5f7a9c875b`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780defcebf1af6f69fb32b4b775410ef0b3a533d7206d0802fb47992e6939246`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43613224a1ef011b49fa7d0d93a0922bc1f8441b463b59e8cfb1467ab36d72b8`  
		Last Modified: Tue, 01 Nov 2016 21:03:36 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3-onbuild`

```console
$ docker pull maven@sha256:651183b4b67ea32ca4931944fa714e9dcaf52409a221b0551c87d38cf723ef39
```

-	Platforms:
	-	linux; amd64

### `maven:3.3-onbuild` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251963962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849fb4dad2fc29ef0f3d83ca7119766c4bfe945f8f085677430d12b28b76aac3`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:53:47 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:53:48 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:53:49 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:53:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:54:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jdk="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:00 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 20:57:48 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 20:57:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 20:57:51 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 20:57:52 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 20:57:53 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 20:57:53 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 20:57:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 20:57:54 GMT
CMD ["mvn"]
# Tue, 01 Nov 2016 21:03:24 GMT
RUN mkdir -p /usr/src/app
# Tue, 01 Nov 2016 21:03:24 GMT
WORKDIR /usr/src/app
# Tue, 01 Nov 2016 21:03:25 GMT
ONBUILD ADD . /usr/src/app
# Tue, 01 Nov 2016 21:03:25 GMT
ONBUILD RUN mvn install
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c6fc3e9968f5b8fb198a1ea206d24c695ca2ba720f3c60465eb766378eb661`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa8d5153bb17cb57f744591779c9cae37e3ce60ef7f251a06de8a52b4a5dc4`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc8d0fffcad18701b038c987358882834e50c5f8880d80e596b1b53a10452b`  
		Last Modified: Tue, 01 Nov 2016 05:35:36 GMT  
		Size: 130.1 MB (130104197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266a2a7ecbe81ae03360bc3e8bf9300175665db11e6d02fa7be79d485b530e`  
		Last Modified: Tue, 01 Nov 2016 05:34:58 GMT  
		Size: 284.2 KB (284198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e47e58a1da1cab2883e7bd00f19d95c09a7d0259e395de0f693f876c016ce6b`  
		Last Modified: Tue, 01 Nov 2016 20:58:08 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195755e92dd5148b2406cadaa8faba615b59375d5ce8e0101125ae5f7a9c875b`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780defcebf1af6f69fb32b4b775410ef0b3a533d7206d0802fb47992e6939246`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43613224a1ef011b49fa7d0d93a0922bc1f8441b463b59e8cfb1467ab36d72b8`  
		Last Modified: Tue, 01 Nov 2016 21:03:36 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3-jdk-8-onbuild`

```console
$ docker pull maven@sha256:651183b4b67ea32ca4931944fa714e9dcaf52409a221b0551c87d38cf723ef39
```

-	Platforms:
	-	linux; amd64

### `maven:3-jdk-8-onbuild` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251963962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849fb4dad2fc29ef0f3d83ca7119766c4bfe945f8f085677430d12b28b76aac3`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:53:47 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:53:48 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:53:49 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:53:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:54:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jdk="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:00 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 20:57:48 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 20:57:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 20:57:51 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 20:57:52 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 20:57:53 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 20:57:53 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 20:57:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 20:57:54 GMT
CMD ["mvn"]
# Tue, 01 Nov 2016 21:03:24 GMT
RUN mkdir -p /usr/src/app
# Tue, 01 Nov 2016 21:03:24 GMT
WORKDIR /usr/src/app
# Tue, 01 Nov 2016 21:03:25 GMT
ONBUILD ADD . /usr/src/app
# Tue, 01 Nov 2016 21:03:25 GMT
ONBUILD RUN mvn install
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c6fc3e9968f5b8fb198a1ea206d24c695ca2ba720f3c60465eb766378eb661`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa8d5153bb17cb57f744591779c9cae37e3ce60ef7f251a06de8a52b4a5dc4`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc8d0fffcad18701b038c987358882834e50c5f8880d80e596b1b53a10452b`  
		Last Modified: Tue, 01 Nov 2016 05:35:36 GMT  
		Size: 130.1 MB (130104197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266a2a7ecbe81ae03360bc3e8bf9300175665db11e6d02fa7be79d485b530e`  
		Last Modified: Tue, 01 Nov 2016 05:34:58 GMT  
		Size: 284.2 KB (284198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e47e58a1da1cab2883e7bd00f19d95c09a7d0259e395de0f693f876c016ce6b`  
		Last Modified: Tue, 01 Nov 2016 20:58:08 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195755e92dd5148b2406cadaa8faba615b59375d5ce8e0101125ae5f7a9c875b`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780defcebf1af6f69fb32b4b775410ef0b3a533d7206d0802fb47992e6939246`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43613224a1ef011b49fa7d0d93a0922bc1f8441b463b59e8cfb1467ab36d72b8`  
		Last Modified: Tue, 01 Nov 2016 21:03:36 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3-onbuild`

```console
$ docker pull maven@sha256:651183b4b67ea32ca4931944fa714e9dcaf52409a221b0551c87d38cf723ef39
```

-	Platforms:
	-	linux; amd64

### `maven:3-onbuild` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251963962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849fb4dad2fc29ef0f3d83ca7119766c4bfe945f8f085677430d12b28b76aac3`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:53:47 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:53:48 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:53:49 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:53:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:54:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jdk="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:00 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 20:57:48 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 20:57:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 20:57:51 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 20:57:52 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 20:57:53 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 20:57:53 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 20:57:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 20:57:54 GMT
CMD ["mvn"]
# Tue, 01 Nov 2016 21:03:24 GMT
RUN mkdir -p /usr/src/app
# Tue, 01 Nov 2016 21:03:24 GMT
WORKDIR /usr/src/app
# Tue, 01 Nov 2016 21:03:25 GMT
ONBUILD ADD . /usr/src/app
# Tue, 01 Nov 2016 21:03:25 GMT
ONBUILD RUN mvn install
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c6fc3e9968f5b8fb198a1ea206d24c695ca2ba720f3c60465eb766378eb661`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa8d5153bb17cb57f744591779c9cae37e3ce60ef7f251a06de8a52b4a5dc4`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc8d0fffcad18701b038c987358882834e50c5f8880d80e596b1b53a10452b`  
		Last Modified: Tue, 01 Nov 2016 05:35:36 GMT  
		Size: 130.1 MB (130104197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266a2a7ecbe81ae03360bc3e8bf9300175665db11e6d02fa7be79d485b530e`  
		Last Modified: Tue, 01 Nov 2016 05:34:58 GMT  
		Size: 284.2 KB (284198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e47e58a1da1cab2883e7bd00f19d95c09a7d0259e395de0f693f876c016ce6b`  
		Last Modified: Tue, 01 Nov 2016 20:58:08 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195755e92dd5148b2406cadaa8faba615b59375d5ce8e0101125ae5f7a9c875b`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780defcebf1af6f69fb32b4b775410ef0b3a533d7206d0802fb47992e6939246`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43613224a1ef011b49fa7d0d93a0922bc1f8441b463b59e8cfb1467ab36d72b8`  
		Last Modified: Tue, 01 Nov 2016 21:03:36 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:onbuild`

```console
$ docker pull maven@sha256:651183b4b67ea32ca4931944fa714e9dcaf52409a221b0551c87d38cf723ef39
```

-	Platforms:
	-	linux; amd64

### `maven:onbuild` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251963962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849fb4dad2fc29ef0f3d83ca7119766c4bfe945f8f085677430d12b28b76aac3`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:53:47 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:53:48 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
# Mon, 31 Oct 2016 21:53:48 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:53:49 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:53:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:54:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jdk="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:00 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 20:57:48 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 20:57:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 20:57:51 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 20:57:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 20:57:52 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 20:57:53 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 20:57:53 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 20:57:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 20:57:54 GMT
CMD ["mvn"]
# Tue, 01 Nov 2016 21:03:24 GMT
RUN mkdir -p /usr/src/app
# Tue, 01 Nov 2016 21:03:24 GMT
WORKDIR /usr/src/app
# Tue, 01 Nov 2016 21:03:25 GMT
ONBUILD ADD . /usr/src/app
# Tue, 01 Nov 2016 21:03:25 GMT
ONBUILD RUN mvn install
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
	-	`sha256:143e9d501644c63b3e69d854e8b4c238797cdf3fc87fd79a686c1262fe61e9b5`  
		Last Modified: Fri, 21 Oct 2016 16:37:53 GMT  
		Size: 42.5 MB (42500812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc4cdbc8d81addf57f4475aafb4d7c14f8b33b1f81338f292d019b52dab828d`  
		Last Modified: Fri, 21 Oct 2016 20:08:28 GMT  
		Size: 593.0 KB (593002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c6fc3e9968f5b8fb198a1ea206d24c695ca2ba720f3c60465eb766378eb661`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa8d5153bb17cb57f744591779c9cae37e3ce60ef7f251a06de8a52b4a5dc4`  
		Last Modified: Tue, 01 Nov 2016 05:34:59 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc8d0fffcad18701b038c987358882834e50c5f8880d80e596b1b53a10452b`  
		Last Modified: Tue, 01 Nov 2016 05:35:36 GMT  
		Size: 130.1 MB (130104197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266a2a7ecbe81ae03360bc3e8bf9300175665db11e6d02fa7be79d485b530e`  
		Last Modified: Tue, 01 Nov 2016 05:34:58 GMT  
		Size: 284.2 KB (284198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e47e58a1da1cab2883e7bd00f19d95c09a7d0259e395de0f693f876c016ce6b`  
		Last Modified: Tue, 01 Nov 2016 20:58:08 GMT  
		Size: 8.6 MB (8598845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195755e92dd5148b2406cadaa8faba615b59375d5ce8e0101125ae5f7a9c875b`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780defcebf1af6f69fb32b4b775410ef0b3a533d7206d0802fb47992e6939246`  
		Last Modified: Tue, 01 Nov 2016 20:58:05 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43613224a1ef011b49fa7d0d93a0922bc1f8441b463b59e8cfb1467ab36d72b8`  
		Last Modified: Tue, 01 Nov 2016 21:03:36 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3.9-jdk-8-alpine`

```console
$ docker pull maven@sha256:62df41e9b418088f2e451609e51380effe41d2f399ae27625f2af84075559d79
```

-	Platforms:
	-	linux; amd64

### `maven:3.3.9-jdk-8-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61928045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4bea601e3d6c930e376475a05738188aa71425a1c8b5e0ca62ff1de9a361500`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:40:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Tue, 18 Oct 2016 20:40:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_VERSION=8u92
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 18 Oct 2016 20:40:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 19 Oct 2016 00:48:37 GMT
RUN apk add --no-cache curl tar bash
# Wed, 19 Oct 2016 00:48:37 GMT
ARG MAVEN_VERSION=3.3.9
# Wed, 19 Oct 2016 00:48:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2016 00:48:39 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2016 00:48:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2016 00:48:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2016 00:48:40 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2016 00:48:41 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 19 Oct 2016 00:48:41 GMT
VOLUME [/root/.m2]
# Wed, 19 Oct 2016 00:48:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2016 00:48:42 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d438913956e1ea2320b12f24358a2b0822a0b3a09aa59d082151759f24486d3`  
		Last Modified: Tue, 18 Oct 2016 20:50:55 GMT  
		Size: 49.3 MB (49327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b8049e40c747a1505c45ac9f52a1cba347b5b4852313173bd431d4b2eb92f`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 1.7 MB (1687191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8aff7e3e994164b7b75ea1e50cd391f0410610c1825619de764b467a3236e1`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 8.6 MB (8598850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546df286a8fce20689ba8271fea14df15e256549ee6c46a38115bd429b7e2782`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc4a15abdcccff3982f30eae2edad980b00ba95b6625baff5e51cfa9bfd06`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3.9-alpine`

```console
$ docker pull maven@sha256:62df41e9b418088f2e451609e51380effe41d2f399ae27625f2af84075559d79
```

-	Platforms:
	-	linux; amd64

### `maven:3.3.9-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61928045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4bea601e3d6c930e376475a05738188aa71425a1c8b5e0ca62ff1de9a361500`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:40:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Tue, 18 Oct 2016 20:40:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_VERSION=8u92
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 18 Oct 2016 20:40:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 19 Oct 2016 00:48:37 GMT
RUN apk add --no-cache curl tar bash
# Wed, 19 Oct 2016 00:48:37 GMT
ARG MAVEN_VERSION=3.3.9
# Wed, 19 Oct 2016 00:48:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2016 00:48:39 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2016 00:48:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2016 00:48:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2016 00:48:40 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2016 00:48:41 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 19 Oct 2016 00:48:41 GMT
VOLUME [/root/.m2]
# Wed, 19 Oct 2016 00:48:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2016 00:48:42 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d438913956e1ea2320b12f24358a2b0822a0b3a09aa59d082151759f24486d3`  
		Last Modified: Tue, 18 Oct 2016 20:50:55 GMT  
		Size: 49.3 MB (49327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b8049e40c747a1505c45ac9f52a1cba347b5b4852313173bd431d4b2eb92f`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 1.7 MB (1687191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8aff7e3e994164b7b75ea1e50cd391f0410610c1825619de764b467a3236e1`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 8.6 MB (8598850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546df286a8fce20689ba8271fea14df15e256549ee6c46a38115bd429b7e2782`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc4a15abdcccff3982f30eae2edad980b00ba95b6625baff5e51cfa9bfd06`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3-jdk-8-alpine`

```console
$ docker pull maven@sha256:62df41e9b418088f2e451609e51380effe41d2f399ae27625f2af84075559d79
```

-	Platforms:
	-	linux; amd64

### `maven:3.3-jdk-8-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61928045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4bea601e3d6c930e376475a05738188aa71425a1c8b5e0ca62ff1de9a361500`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:40:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Tue, 18 Oct 2016 20:40:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_VERSION=8u92
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 18 Oct 2016 20:40:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 19 Oct 2016 00:48:37 GMT
RUN apk add --no-cache curl tar bash
# Wed, 19 Oct 2016 00:48:37 GMT
ARG MAVEN_VERSION=3.3.9
# Wed, 19 Oct 2016 00:48:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2016 00:48:39 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2016 00:48:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2016 00:48:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2016 00:48:40 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2016 00:48:41 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 19 Oct 2016 00:48:41 GMT
VOLUME [/root/.m2]
# Wed, 19 Oct 2016 00:48:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2016 00:48:42 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d438913956e1ea2320b12f24358a2b0822a0b3a09aa59d082151759f24486d3`  
		Last Modified: Tue, 18 Oct 2016 20:50:55 GMT  
		Size: 49.3 MB (49327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b8049e40c747a1505c45ac9f52a1cba347b5b4852313173bd431d4b2eb92f`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 1.7 MB (1687191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8aff7e3e994164b7b75ea1e50cd391f0410610c1825619de764b467a3236e1`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 8.6 MB (8598850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546df286a8fce20689ba8271fea14df15e256549ee6c46a38115bd429b7e2782`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc4a15abdcccff3982f30eae2edad980b00ba95b6625baff5e51cfa9bfd06`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3-alpine`

```console
$ docker pull maven@sha256:62df41e9b418088f2e451609e51380effe41d2f399ae27625f2af84075559d79
```

-	Platforms:
	-	linux; amd64

### `maven:3.3-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61928045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4bea601e3d6c930e376475a05738188aa71425a1c8b5e0ca62ff1de9a361500`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:40:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Tue, 18 Oct 2016 20:40:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_VERSION=8u92
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 18 Oct 2016 20:40:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 19 Oct 2016 00:48:37 GMT
RUN apk add --no-cache curl tar bash
# Wed, 19 Oct 2016 00:48:37 GMT
ARG MAVEN_VERSION=3.3.9
# Wed, 19 Oct 2016 00:48:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2016 00:48:39 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2016 00:48:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2016 00:48:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2016 00:48:40 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2016 00:48:41 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 19 Oct 2016 00:48:41 GMT
VOLUME [/root/.m2]
# Wed, 19 Oct 2016 00:48:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2016 00:48:42 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d438913956e1ea2320b12f24358a2b0822a0b3a09aa59d082151759f24486d3`  
		Last Modified: Tue, 18 Oct 2016 20:50:55 GMT  
		Size: 49.3 MB (49327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b8049e40c747a1505c45ac9f52a1cba347b5b4852313173bd431d4b2eb92f`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 1.7 MB (1687191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8aff7e3e994164b7b75ea1e50cd391f0410610c1825619de764b467a3236e1`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 8.6 MB (8598850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546df286a8fce20689ba8271fea14df15e256549ee6c46a38115bd429b7e2782`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc4a15abdcccff3982f30eae2edad980b00ba95b6625baff5e51cfa9bfd06`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3-jdk-8-alpine`

```console
$ docker pull maven@sha256:62df41e9b418088f2e451609e51380effe41d2f399ae27625f2af84075559d79
```

-	Platforms:
	-	linux; amd64

### `maven:3-jdk-8-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61928045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4bea601e3d6c930e376475a05738188aa71425a1c8b5e0ca62ff1de9a361500`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:40:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Tue, 18 Oct 2016 20:40:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_VERSION=8u92
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 18 Oct 2016 20:40:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 19 Oct 2016 00:48:37 GMT
RUN apk add --no-cache curl tar bash
# Wed, 19 Oct 2016 00:48:37 GMT
ARG MAVEN_VERSION=3.3.9
# Wed, 19 Oct 2016 00:48:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2016 00:48:39 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2016 00:48:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2016 00:48:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2016 00:48:40 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2016 00:48:41 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 19 Oct 2016 00:48:41 GMT
VOLUME [/root/.m2]
# Wed, 19 Oct 2016 00:48:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2016 00:48:42 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d438913956e1ea2320b12f24358a2b0822a0b3a09aa59d082151759f24486d3`  
		Last Modified: Tue, 18 Oct 2016 20:50:55 GMT  
		Size: 49.3 MB (49327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b8049e40c747a1505c45ac9f52a1cba347b5b4852313173bd431d4b2eb92f`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 1.7 MB (1687191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8aff7e3e994164b7b75ea1e50cd391f0410610c1825619de764b467a3236e1`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 8.6 MB (8598850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546df286a8fce20689ba8271fea14df15e256549ee6c46a38115bd429b7e2782`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc4a15abdcccff3982f30eae2edad980b00ba95b6625baff5e51cfa9bfd06`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3-alpine`

```console
$ docker pull maven@sha256:62df41e9b418088f2e451609e51380effe41d2f399ae27625f2af84075559d79
```

-	Platforms:
	-	linux; amd64

### `maven:3-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61928045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4bea601e3d6c930e376475a05738188aa71425a1c8b5e0ca62ff1de9a361500`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:40:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Tue, 18 Oct 2016 20:40:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_VERSION=8u92
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 18 Oct 2016 20:40:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 19 Oct 2016 00:48:37 GMT
RUN apk add --no-cache curl tar bash
# Wed, 19 Oct 2016 00:48:37 GMT
ARG MAVEN_VERSION=3.3.9
# Wed, 19 Oct 2016 00:48:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2016 00:48:39 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2016 00:48:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2016 00:48:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2016 00:48:40 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2016 00:48:41 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 19 Oct 2016 00:48:41 GMT
VOLUME [/root/.m2]
# Wed, 19 Oct 2016 00:48:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2016 00:48:42 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d438913956e1ea2320b12f24358a2b0822a0b3a09aa59d082151759f24486d3`  
		Last Modified: Tue, 18 Oct 2016 20:50:55 GMT  
		Size: 49.3 MB (49327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b8049e40c747a1505c45ac9f52a1cba347b5b4852313173bd431d4b2eb92f`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 1.7 MB (1687191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8aff7e3e994164b7b75ea1e50cd391f0410610c1825619de764b467a3236e1`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 8.6 MB (8598850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546df286a8fce20689ba8271fea14df15e256549ee6c46a38115bd429b7e2782`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc4a15abdcccff3982f30eae2edad980b00ba95b6625baff5e51cfa9bfd06`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:alpine`

```console
$ docker pull maven@sha256:62df41e9b418088f2e451609e51380effe41d2f399ae27625f2af84075559d79
```

-	Platforms:
	-	linux; amd64

### `maven:alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61928045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4bea601e3d6c930e376475a05738188aa71425a1c8b5e0ca62ff1de9a361500`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:40:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Tue, 18 Oct 2016 20:40:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_VERSION=8u92
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 18 Oct 2016 20:40:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 19 Oct 2016 00:48:37 GMT
RUN apk add --no-cache curl tar bash
# Wed, 19 Oct 2016 00:48:37 GMT
ARG MAVEN_VERSION=3.3.9
# Wed, 19 Oct 2016 00:48:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2016 00:48:39 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2016 00:48:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2016 00:48:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2016 00:48:40 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2016 00:48:41 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 19 Oct 2016 00:48:41 GMT
VOLUME [/root/.m2]
# Wed, 19 Oct 2016 00:48:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2016 00:48:42 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d438913956e1ea2320b12f24358a2b0822a0b3a09aa59d082151759f24486d3`  
		Last Modified: Tue, 18 Oct 2016 20:50:55 GMT  
		Size: 49.3 MB (49327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b8049e40c747a1505c45ac9f52a1cba347b5b4852313173bd431d4b2eb92f`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 1.7 MB (1687191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8aff7e3e994164b7b75ea1e50cd391f0410610c1825619de764b467a3236e1`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 8.6 MB (8598850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546df286a8fce20689ba8271fea14df15e256549ee6c46a38115bd429b7e2782`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc4a15abdcccff3982f30eae2edad980b00ba95b6625baff5e51cfa9bfd06`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3.9-jdk-8-onbuild-alpine`

```console
$ docker pull maven@sha256:58498551028491dc40182d421a0500d31f6b5ad5f2beb0117bc8d72620f60f5c
```

-	Platforms:
	-	linux; amd64

### `maven:3.3.9-jdk-8-onbuild-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61928202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907ecf7899ad4b22a2cfd208eb4ae7b269369551eeab9c010b02b3761efc8b2d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:40:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Tue, 18 Oct 2016 20:40:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_VERSION=8u92
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 18 Oct 2016 20:40:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 19 Oct 2016 00:48:37 GMT
RUN apk add --no-cache curl tar bash
# Wed, 19 Oct 2016 00:48:37 GMT
ARG MAVEN_VERSION=3.3.9
# Wed, 19 Oct 2016 00:48:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2016 00:48:39 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2016 00:48:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2016 00:48:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2016 00:48:40 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2016 00:48:41 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 19 Oct 2016 00:48:41 GMT
VOLUME [/root/.m2]
# Wed, 19 Oct 2016 00:48:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2016 00:48:42 GMT
CMD ["mvn"]
# Wed, 19 Oct 2016 00:51:32 GMT
RUN mkdir -p /usr/src/app
# Wed, 19 Oct 2016 00:51:32 GMT
WORKDIR /usr/src/app
# Wed, 19 Oct 2016 00:51:33 GMT
ONBUILD ADD . /usr/src/app
# Wed, 19 Oct 2016 00:51:33 GMT
ONBUILD RUN mvn install
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d438913956e1ea2320b12f24358a2b0822a0b3a09aa59d082151759f24486d3`  
		Last Modified: Tue, 18 Oct 2016 20:50:55 GMT  
		Size: 49.3 MB (49327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b8049e40c747a1505c45ac9f52a1cba347b5b4852313173bd431d4b2eb92f`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 1.7 MB (1687191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8aff7e3e994164b7b75ea1e50cd391f0410610c1825619de764b467a3236e1`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 8.6 MB (8598850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546df286a8fce20689ba8271fea14df15e256549ee6c46a38115bd429b7e2782`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc4a15abdcccff3982f30eae2edad980b00ba95b6625baff5e51cfa9bfd06`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeca2b024b2850d4fd27ecb654983132029e99c122a9f01f0c549d4f473f139f`  
		Last Modified: Wed, 19 Oct 2016 00:51:43 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3.9-onbuild-alpine`

```console
$ docker pull maven@sha256:58498551028491dc40182d421a0500d31f6b5ad5f2beb0117bc8d72620f60f5c
```

-	Platforms:
	-	linux; amd64

### `maven:3.3.9-onbuild-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61928202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907ecf7899ad4b22a2cfd208eb4ae7b269369551eeab9c010b02b3761efc8b2d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:40:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Tue, 18 Oct 2016 20:40:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_VERSION=8u92
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 18 Oct 2016 20:40:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 19 Oct 2016 00:48:37 GMT
RUN apk add --no-cache curl tar bash
# Wed, 19 Oct 2016 00:48:37 GMT
ARG MAVEN_VERSION=3.3.9
# Wed, 19 Oct 2016 00:48:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2016 00:48:39 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2016 00:48:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2016 00:48:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2016 00:48:40 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2016 00:48:41 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 19 Oct 2016 00:48:41 GMT
VOLUME [/root/.m2]
# Wed, 19 Oct 2016 00:48:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2016 00:48:42 GMT
CMD ["mvn"]
# Wed, 19 Oct 2016 00:51:32 GMT
RUN mkdir -p /usr/src/app
# Wed, 19 Oct 2016 00:51:32 GMT
WORKDIR /usr/src/app
# Wed, 19 Oct 2016 00:51:33 GMT
ONBUILD ADD . /usr/src/app
# Wed, 19 Oct 2016 00:51:33 GMT
ONBUILD RUN mvn install
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d438913956e1ea2320b12f24358a2b0822a0b3a09aa59d082151759f24486d3`  
		Last Modified: Tue, 18 Oct 2016 20:50:55 GMT  
		Size: 49.3 MB (49327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b8049e40c747a1505c45ac9f52a1cba347b5b4852313173bd431d4b2eb92f`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 1.7 MB (1687191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8aff7e3e994164b7b75ea1e50cd391f0410610c1825619de764b467a3236e1`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 8.6 MB (8598850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546df286a8fce20689ba8271fea14df15e256549ee6c46a38115bd429b7e2782`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc4a15abdcccff3982f30eae2edad980b00ba95b6625baff5e51cfa9bfd06`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeca2b024b2850d4fd27ecb654983132029e99c122a9f01f0c549d4f473f139f`  
		Last Modified: Wed, 19 Oct 2016 00:51:43 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3-jdk-8-onbuild-alpine`

```console
$ docker pull maven@sha256:58498551028491dc40182d421a0500d31f6b5ad5f2beb0117bc8d72620f60f5c
```

-	Platforms:
	-	linux; amd64

### `maven:3.3-jdk-8-onbuild-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61928202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907ecf7899ad4b22a2cfd208eb4ae7b269369551eeab9c010b02b3761efc8b2d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:40:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Tue, 18 Oct 2016 20:40:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_VERSION=8u92
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 18 Oct 2016 20:40:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 19 Oct 2016 00:48:37 GMT
RUN apk add --no-cache curl tar bash
# Wed, 19 Oct 2016 00:48:37 GMT
ARG MAVEN_VERSION=3.3.9
# Wed, 19 Oct 2016 00:48:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2016 00:48:39 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2016 00:48:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2016 00:48:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2016 00:48:40 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2016 00:48:41 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 19 Oct 2016 00:48:41 GMT
VOLUME [/root/.m2]
# Wed, 19 Oct 2016 00:48:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2016 00:48:42 GMT
CMD ["mvn"]
# Wed, 19 Oct 2016 00:51:32 GMT
RUN mkdir -p /usr/src/app
# Wed, 19 Oct 2016 00:51:32 GMT
WORKDIR /usr/src/app
# Wed, 19 Oct 2016 00:51:33 GMT
ONBUILD ADD . /usr/src/app
# Wed, 19 Oct 2016 00:51:33 GMT
ONBUILD RUN mvn install
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d438913956e1ea2320b12f24358a2b0822a0b3a09aa59d082151759f24486d3`  
		Last Modified: Tue, 18 Oct 2016 20:50:55 GMT  
		Size: 49.3 MB (49327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b8049e40c747a1505c45ac9f52a1cba347b5b4852313173bd431d4b2eb92f`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 1.7 MB (1687191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8aff7e3e994164b7b75ea1e50cd391f0410610c1825619de764b467a3236e1`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 8.6 MB (8598850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546df286a8fce20689ba8271fea14df15e256549ee6c46a38115bd429b7e2782`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc4a15abdcccff3982f30eae2edad980b00ba95b6625baff5e51cfa9bfd06`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeca2b024b2850d4fd27ecb654983132029e99c122a9f01f0c549d4f473f139f`  
		Last Modified: Wed, 19 Oct 2016 00:51:43 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3-onbuild-alpine`

```console
$ docker pull maven@sha256:58498551028491dc40182d421a0500d31f6b5ad5f2beb0117bc8d72620f60f5c
```

-	Platforms:
	-	linux; amd64

### `maven:3.3-onbuild-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61928202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907ecf7899ad4b22a2cfd208eb4ae7b269369551eeab9c010b02b3761efc8b2d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:40:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Tue, 18 Oct 2016 20:40:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_VERSION=8u92
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 18 Oct 2016 20:40:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 19 Oct 2016 00:48:37 GMT
RUN apk add --no-cache curl tar bash
# Wed, 19 Oct 2016 00:48:37 GMT
ARG MAVEN_VERSION=3.3.9
# Wed, 19 Oct 2016 00:48:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2016 00:48:39 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2016 00:48:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2016 00:48:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2016 00:48:40 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2016 00:48:41 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 19 Oct 2016 00:48:41 GMT
VOLUME [/root/.m2]
# Wed, 19 Oct 2016 00:48:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2016 00:48:42 GMT
CMD ["mvn"]
# Wed, 19 Oct 2016 00:51:32 GMT
RUN mkdir -p /usr/src/app
# Wed, 19 Oct 2016 00:51:32 GMT
WORKDIR /usr/src/app
# Wed, 19 Oct 2016 00:51:33 GMT
ONBUILD ADD . /usr/src/app
# Wed, 19 Oct 2016 00:51:33 GMT
ONBUILD RUN mvn install
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d438913956e1ea2320b12f24358a2b0822a0b3a09aa59d082151759f24486d3`  
		Last Modified: Tue, 18 Oct 2016 20:50:55 GMT  
		Size: 49.3 MB (49327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b8049e40c747a1505c45ac9f52a1cba347b5b4852313173bd431d4b2eb92f`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 1.7 MB (1687191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8aff7e3e994164b7b75ea1e50cd391f0410610c1825619de764b467a3236e1`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 8.6 MB (8598850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546df286a8fce20689ba8271fea14df15e256549ee6c46a38115bd429b7e2782`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc4a15abdcccff3982f30eae2edad980b00ba95b6625baff5e51cfa9bfd06`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeca2b024b2850d4fd27ecb654983132029e99c122a9f01f0c549d4f473f139f`  
		Last Modified: Wed, 19 Oct 2016 00:51:43 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3-jdk-8-onbuild-alpine`

```console
$ docker pull maven@sha256:58498551028491dc40182d421a0500d31f6b5ad5f2beb0117bc8d72620f60f5c
```

-	Platforms:
	-	linux; amd64

### `maven:3-jdk-8-onbuild-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61928202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907ecf7899ad4b22a2cfd208eb4ae7b269369551eeab9c010b02b3761efc8b2d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:40:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Tue, 18 Oct 2016 20:40:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_VERSION=8u92
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 18 Oct 2016 20:40:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 19 Oct 2016 00:48:37 GMT
RUN apk add --no-cache curl tar bash
# Wed, 19 Oct 2016 00:48:37 GMT
ARG MAVEN_VERSION=3.3.9
# Wed, 19 Oct 2016 00:48:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2016 00:48:39 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2016 00:48:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2016 00:48:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2016 00:48:40 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2016 00:48:41 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 19 Oct 2016 00:48:41 GMT
VOLUME [/root/.m2]
# Wed, 19 Oct 2016 00:48:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2016 00:48:42 GMT
CMD ["mvn"]
# Wed, 19 Oct 2016 00:51:32 GMT
RUN mkdir -p /usr/src/app
# Wed, 19 Oct 2016 00:51:32 GMT
WORKDIR /usr/src/app
# Wed, 19 Oct 2016 00:51:33 GMT
ONBUILD ADD . /usr/src/app
# Wed, 19 Oct 2016 00:51:33 GMT
ONBUILD RUN mvn install
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d438913956e1ea2320b12f24358a2b0822a0b3a09aa59d082151759f24486d3`  
		Last Modified: Tue, 18 Oct 2016 20:50:55 GMT  
		Size: 49.3 MB (49327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b8049e40c747a1505c45ac9f52a1cba347b5b4852313173bd431d4b2eb92f`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 1.7 MB (1687191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8aff7e3e994164b7b75ea1e50cd391f0410610c1825619de764b467a3236e1`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 8.6 MB (8598850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546df286a8fce20689ba8271fea14df15e256549ee6c46a38115bd429b7e2782`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc4a15abdcccff3982f30eae2edad980b00ba95b6625baff5e51cfa9bfd06`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeca2b024b2850d4fd27ecb654983132029e99c122a9f01f0c549d4f473f139f`  
		Last Modified: Wed, 19 Oct 2016 00:51:43 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3-onbuild-alpine`

```console
$ docker pull maven@sha256:58498551028491dc40182d421a0500d31f6b5ad5f2beb0117bc8d72620f60f5c
```

-	Platforms:
	-	linux; amd64

### `maven:3-onbuild-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61928202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907ecf7899ad4b22a2cfd208eb4ae7b269369551eeab9c010b02b3761efc8b2d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:40:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Tue, 18 Oct 2016 20:40:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_VERSION=8u92
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 18 Oct 2016 20:40:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 19 Oct 2016 00:48:37 GMT
RUN apk add --no-cache curl tar bash
# Wed, 19 Oct 2016 00:48:37 GMT
ARG MAVEN_VERSION=3.3.9
# Wed, 19 Oct 2016 00:48:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2016 00:48:39 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2016 00:48:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2016 00:48:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2016 00:48:40 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2016 00:48:41 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 19 Oct 2016 00:48:41 GMT
VOLUME [/root/.m2]
# Wed, 19 Oct 2016 00:48:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2016 00:48:42 GMT
CMD ["mvn"]
# Wed, 19 Oct 2016 00:51:32 GMT
RUN mkdir -p /usr/src/app
# Wed, 19 Oct 2016 00:51:32 GMT
WORKDIR /usr/src/app
# Wed, 19 Oct 2016 00:51:33 GMT
ONBUILD ADD . /usr/src/app
# Wed, 19 Oct 2016 00:51:33 GMT
ONBUILD RUN mvn install
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d438913956e1ea2320b12f24358a2b0822a0b3a09aa59d082151759f24486d3`  
		Last Modified: Tue, 18 Oct 2016 20:50:55 GMT  
		Size: 49.3 MB (49327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b8049e40c747a1505c45ac9f52a1cba347b5b4852313173bd431d4b2eb92f`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 1.7 MB (1687191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8aff7e3e994164b7b75ea1e50cd391f0410610c1825619de764b467a3236e1`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 8.6 MB (8598850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546df286a8fce20689ba8271fea14df15e256549ee6c46a38115bd429b7e2782`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc4a15abdcccff3982f30eae2edad980b00ba95b6625baff5e51cfa9bfd06`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeca2b024b2850d4fd27ecb654983132029e99c122a9f01f0c549d4f473f139f`  
		Last Modified: Wed, 19 Oct 2016 00:51:43 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:onbuild-alpine`

```console
$ docker pull maven@sha256:58498551028491dc40182d421a0500d31f6b5ad5f2beb0117bc8d72620f60f5c
```

-	Platforms:
	-	linux; amd64

### `maven:onbuild-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61928202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907ecf7899ad4b22a2cfd208eb4ae7b269369551eeab9c010b02b3761efc8b2d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:39:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2016 20:39:58 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Oct 2016 20:40:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Tue, 18 Oct 2016 20:40:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_VERSION=8u92
# Tue, 18 Oct 2016 20:40:26 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 18 Oct 2016 20:40:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 19 Oct 2016 00:48:37 GMT
RUN apk add --no-cache curl tar bash
# Wed, 19 Oct 2016 00:48:37 GMT
ARG MAVEN_VERSION=3.3.9
# Wed, 19 Oct 2016 00:48:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2016 00:48:39 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2016 00:48:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2016 00:48:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2016 00:48:40 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2016 00:48:41 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 19 Oct 2016 00:48:41 GMT
VOLUME [/root/.m2]
# Wed, 19 Oct 2016 00:48:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2016 00:48:42 GMT
CMD ["mvn"]
# Wed, 19 Oct 2016 00:51:32 GMT
RUN mkdir -p /usr/src/app
# Wed, 19 Oct 2016 00:51:32 GMT
WORKDIR /usr/src/app
# Wed, 19 Oct 2016 00:51:33 GMT
ONBUILD ADD . /usr/src/app
# Wed, 19 Oct 2016 00:51:33 GMT
ONBUILD RUN mvn install
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb77eb56b4c44907a822ccdf607323c1f42fd024b7db6be146dd049d95f305`  
		Last Modified: Tue, 18 Oct 2016 20:45:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d438913956e1ea2320b12f24358a2b0822a0b3a09aa59d082151759f24486d3`  
		Last Modified: Tue, 18 Oct 2016 20:50:55 GMT  
		Size: 49.3 MB (49327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b8049e40c747a1505c45ac9f52a1cba347b5b4852313173bd431d4b2eb92f`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 1.7 MB (1687191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8aff7e3e994164b7b75ea1e50cd391f0410610c1825619de764b467a3236e1`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 8.6 MB (8598850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546df286a8fce20689ba8271fea14df15e256549ee6c46a38115bd429b7e2782`  
		Last Modified: Wed, 19 Oct 2016 00:48:52 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadc4a15abdcccff3982f30eae2edad980b00ba95b6625baff5e51cfa9bfd06`  
		Last Modified: Wed, 19 Oct 2016 00:48:53 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeca2b024b2850d4fd27ecb654983132029e99c122a9f01f0c549d4f473f139f`  
		Last Modified: Wed, 19 Oct 2016 00:51:43 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3.9-jdk-9`

```console
$ docker pull maven@sha256:3a23f78ce97aabf62bcd0d642c570ab58b8b332094f632c2a44e98e02c215371
```

-	Platforms:
	-	linux; amd64

### `maven:3.3.9-jdk-9` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.1 MB (252134352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1410423cb508c4c25c4e2788b10de9b7d3db6e579f1b00738a8b502dcfba690`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 17 Oct 2016 21:26:09 GMT
ADD file:7a91bb1a28e088d8d427022bb612873476ea54ec75cb559e5943b771d7412386 in / 
# Mon, 17 Oct 2016 21:26:10 GMT
CMD ["/bin/bash"]
# Mon, 17 Oct 2016 23:39:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Mon, 17 Oct 2016 23:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Oct 2016 20:40:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:55:25 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
# Mon, 31 Oct 2016 21:55:26 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:55:27 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:55:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-9-openjdk-amd64
# Tue, 01 Nov 2016 17:32:07 GMT
ENV JAVA_VERSION=9~b142
# Tue, 01 Nov 2016 17:32:07 GMT
ENV JAVA_DEBIAN_VERSION=9~b142-1
# Tue, 01 Nov 2016 17:33:02 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-9-jdk-headless="$JAVA_DEBIAN_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 01 Nov 2016 21:09:43 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 21:09:43 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 21:09:46 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 21:09:46 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 21:09:47 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 21:09:47 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 21:09:48 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 21:09:48 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 21:09:49 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 21:09:49 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:279daf9814f4ba6feba147fd51356389273017b7d4a057e5a7cf724467c2fbcd`  
		Last Modified: Mon, 17 Oct 2016 21:26:30 GMT  
		Size: 43.2 MB (43195045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee53d9e55ce8c4310eed9df888489b1e79dc22764f3c442d8e767d0f4218b57`  
		Last Modified: Mon, 17 Oct 2016 23:40:01 GMT  
		Size: 20.6 MB (20581005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1bde82dbdb2519006f9578e8408db12a546bf1b5ae03940b08f3f20ca8b3dc`  
		Last Modified: Mon, 17 Oct 2016 23:41:03 GMT  
		Size: 48.3 MB (48288494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af9bebd3ac92605303612e9f49a36146006a2e79a5854e87e6027cc653ba2f`  
		Last Modified: Tue, 18 Oct 2016 20:54:37 GMT  
		Size: 635.2 KB (635211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a8b3d97f9ec158a76cc7a9b135022d2879c8bad50545e8489b035c5ec117bb`  
		Last Modified: Tue, 01 Nov 2016 17:47:25 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf2e5d403074cda795f6dbb5eb780c54d1228c4721baecc38d81207f376f75b`  
		Last Modified: Tue, 01 Nov 2016 17:47:25 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d7b126890936d56eda9052eb4d78f32533381bc4bea0b621ddbbd9cd9ffff9`  
		Last Modified: Tue, 01 Nov 2016 17:47:47 GMT  
		Size: 130.8 MB (130834247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e1a5ba0ef9b1c4cce3beb8bd69da4910d14329b133eff8a907157d53b82031`  
		Last Modified: Tue, 01 Nov 2016 21:10:02 GMT  
		Size: 8.6 MB (8598855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a600c2f6671c0be801df4b944103f1fae7f6262ff6cb6c5abc916b2b584984`  
		Last Modified: Tue, 01 Nov 2016 21:10:00 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f7204b7980e92509a4511f548b3d6d6e51d8ce18275231a061b4d1dc9b1547`  
		Last Modified: Tue, 01 Nov 2016 21:10:00 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3-jdk-9`

```console
$ docker pull maven@sha256:3a23f78ce97aabf62bcd0d642c570ab58b8b332094f632c2a44e98e02c215371
```

-	Platforms:
	-	linux; amd64

### `maven:3.3-jdk-9` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.1 MB (252134352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1410423cb508c4c25c4e2788b10de9b7d3db6e579f1b00738a8b502dcfba690`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 17 Oct 2016 21:26:09 GMT
ADD file:7a91bb1a28e088d8d427022bb612873476ea54ec75cb559e5943b771d7412386 in / 
# Mon, 17 Oct 2016 21:26:10 GMT
CMD ["/bin/bash"]
# Mon, 17 Oct 2016 23:39:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Mon, 17 Oct 2016 23:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Oct 2016 20:40:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:55:25 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
# Mon, 31 Oct 2016 21:55:26 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:55:27 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:55:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-9-openjdk-amd64
# Tue, 01 Nov 2016 17:32:07 GMT
ENV JAVA_VERSION=9~b142
# Tue, 01 Nov 2016 17:32:07 GMT
ENV JAVA_DEBIAN_VERSION=9~b142-1
# Tue, 01 Nov 2016 17:33:02 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-9-jdk-headless="$JAVA_DEBIAN_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 01 Nov 2016 21:09:43 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 21:09:43 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 21:09:46 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 21:09:46 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 21:09:47 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 21:09:47 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 21:09:48 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 21:09:48 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 21:09:49 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 21:09:49 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:279daf9814f4ba6feba147fd51356389273017b7d4a057e5a7cf724467c2fbcd`  
		Last Modified: Mon, 17 Oct 2016 21:26:30 GMT  
		Size: 43.2 MB (43195045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee53d9e55ce8c4310eed9df888489b1e79dc22764f3c442d8e767d0f4218b57`  
		Last Modified: Mon, 17 Oct 2016 23:40:01 GMT  
		Size: 20.6 MB (20581005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1bde82dbdb2519006f9578e8408db12a546bf1b5ae03940b08f3f20ca8b3dc`  
		Last Modified: Mon, 17 Oct 2016 23:41:03 GMT  
		Size: 48.3 MB (48288494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af9bebd3ac92605303612e9f49a36146006a2e79a5854e87e6027cc653ba2f`  
		Last Modified: Tue, 18 Oct 2016 20:54:37 GMT  
		Size: 635.2 KB (635211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a8b3d97f9ec158a76cc7a9b135022d2879c8bad50545e8489b035c5ec117bb`  
		Last Modified: Tue, 01 Nov 2016 17:47:25 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf2e5d403074cda795f6dbb5eb780c54d1228c4721baecc38d81207f376f75b`  
		Last Modified: Tue, 01 Nov 2016 17:47:25 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d7b126890936d56eda9052eb4d78f32533381bc4bea0b621ddbbd9cd9ffff9`  
		Last Modified: Tue, 01 Nov 2016 17:47:47 GMT  
		Size: 130.8 MB (130834247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e1a5ba0ef9b1c4cce3beb8bd69da4910d14329b133eff8a907157d53b82031`  
		Last Modified: Tue, 01 Nov 2016 21:10:02 GMT  
		Size: 8.6 MB (8598855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a600c2f6671c0be801df4b944103f1fae7f6262ff6cb6c5abc916b2b584984`  
		Last Modified: Tue, 01 Nov 2016 21:10:00 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f7204b7980e92509a4511f548b3d6d6e51d8ce18275231a061b4d1dc9b1547`  
		Last Modified: Tue, 01 Nov 2016 21:10:00 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3-jdk-9`

```console
$ docker pull maven@sha256:3a23f78ce97aabf62bcd0d642c570ab58b8b332094f632c2a44e98e02c215371
```

-	Platforms:
	-	linux; amd64

### `maven:3-jdk-9` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.1 MB (252134352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1410423cb508c4c25c4e2788b10de9b7d3db6e579f1b00738a8b502dcfba690`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 17 Oct 2016 21:26:09 GMT
ADD file:7a91bb1a28e088d8d427022bb612873476ea54ec75cb559e5943b771d7412386 in / 
# Mon, 17 Oct 2016 21:26:10 GMT
CMD ["/bin/bash"]
# Mon, 17 Oct 2016 23:39:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Mon, 17 Oct 2016 23:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Oct 2016 20:40:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:55:25 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
# Mon, 31 Oct 2016 21:55:26 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:55:27 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:55:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-9-openjdk-amd64
# Tue, 01 Nov 2016 17:32:07 GMT
ENV JAVA_VERSION=9~b142
# Tue, 01 Nov 2016 17:32:07 GMT
ENV JAVA_DEBIAN_VERSION=9~b142-1
# Tue, 01 Nov 2016 17:33:02 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-9-jdk-headless="$JAVA_DEBIAN_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 01 Nov 2016 21:09:43 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 21:09:43 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 21:09:46 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 21:09:46 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 21:09:47 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 21:09:47 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 21:09:48 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 21:09:48 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 21:09:49 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 21:09:49 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:279daf9814f4ba6feba147fd51356389273017b7d4a057e5a7cf724467c2fbcd`  
		Last Modified: Mon, 17 Oct 2016 21:26:30 GMT  
		Size: 43.2 MB (43195045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee53d9e55ce8c4310eed9df888489b1e79dc22764f3c442d8e767d0f4218b57`  
		Last Modified: Mon, 17 Oct 2016 23:40:01 GMT  
		Size: 20.6 MB (20581005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1bde82dbdb2519006f9578e8408db12a546bf1b5ae03940b08f3f20ca8b3dc`  
		Last Modified: Mon, 17 Oct 2016 23:41:03 GMT  
		Size: 48.3 MB (48288494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af9bebd3ac92605303612e9f49a36146006a2e79a5854e87e6027cc653ba2f`  
		Last Modified: Tue, 18 Oct 2016 20:54:37 GMT  
		Size: 635.2 KB (635211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a8b3d97f9ec158a76cc7a9b135022d2879c8bad50545e8489b035c5ec117bb`  
		Last Modified: Tue, 01 Nov 2016 17:47:25 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf2e5d403074cda795f6dbb5eb780c54d1228c4721baecc38d81207f376f75b`  
		Last Modified: Tue, 01 Nov 2016 17:47:25 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d7b126890936d56eda9052eb4d78f32533381bc4bea0b621ddbbd9cd9ffff9`  
		Last Modified: Tue, 01 Nov 2016 17:47:47 GMT  
		Size: 130.8 MB (130834247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e1a5ba0ef9b1c4cce3beb8bd69da4910d14329b133eff8a907157d53b82031`  
		Last Modified: Tue, 01 Nov 2016 21:10:02 GMT  
		Size: 8.6 MB (8598855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a600c2f6671c0be801df4b944103f1fae7f6262ff6cb6c5abc916b2b584984`  
		Last Modified: Tue, 01 Nov 2016 21:10:00 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f7204b7980e92509a4511f548b3d6d6e51d8ce18275231a061b4d1dc9b1547`  
		Last Modified: Tue, 01 Nov 2016 21:10:00 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3.9-jdk-9-onbuild`

```console
$ docker pull maven@sha256:6afd01c75be4e929ce966ef4cf33e97073700f2f40b88e832067af810a9f9d10
```

-	Platforms:
	-	linux; amd64

### `maven:3.3.9-jdk-9-onbuild` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.1 MB (252134509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a182ec57db005bdf1e0a87db5a8613ab58bbd74a302770af34453d37888a573`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 17 Oct 2016 21:26:09 GMT
ADD file:7a91bb1a28e088d8d427022bb612873476ea54ec75cb559e5943b771d7412386 in / 
# Mon, 17 Oct 2016 21:26:10 GMT
CMD ["/bin/bash"]
# Mon, 17 Oct 2016 23:39:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Mon, 17 Oct 2016 23:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Oct 2016 20:40:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:55:25 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
# Mon, 31 Oct 2016 21:55:26 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:55:27 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:55:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-9-openjdk-amd64
# Tue, 01 Nov 2016 17:32:07 GMT
ENV JAVA_VERSION=9~b142
# Tue, 01 Nov 2016 17:32:07 GMT
ENV JAVA_DEBIAN_VERSION=9~b142-1
# Tue, 01 Nov 2016 17:33:02 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-9-jdk-headless="$JAVA_DEBIAN_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 01 Nov 2016 21:09:43 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 21:09:43 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 21:09:46 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 21:09:46 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 21:09:47 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 21:09:47 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 21:09:48 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 21:09:48 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 21:09:49 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 21:09:49 GMT
CMD ["mvn"]
# Tue, 01 Nov 2016 21:10:34 GMT
RUN mkdir -p /usr/src/app
# Tue, 01 Nov 2016 21:10:35 GMT
WORKDIR /usr/src/app
# Tue, 01 Nov 2016 21:10:35 GMT
ONBUILD ADD . /usr/src/app
# Tue, 01 Nov 2016 21:10:35 GMT
ONBUILD RUN mvn install
```

-	Layers:
	-	`sha256:279daf9814f4ba6feba147fd51356389273017b7d4a057e5a7cf724467c2fbcd`  
		Last Modified: Mon, 17 Oct 2016 21:26:30 GMT  
		Size: 43.2 MB (43195045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee53d9e55ce8c4310eed9df888489b1e79dc22764f3c442d8e767d0f4218b57`  
		Last Modified: Mon, 17 Oct 2016 23:40:01 GMT  
		Size: 20.6 MB (20581005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1bde82dbdb2519006f9578e8408db12a546bf1b5ae03940b08f3f20ca8b3dc`  
		Last Modified: Mon, 17 Oct 2016 23:41:03 GMT  
		Size: 48.3 MB (48288494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af9bebd3ac92605303612e9f49a36146006a2e79a5854e87e6027cc653ba2f`  
		Last Modified: Tue, 18 Oct 2016 20:54:37 GMT  
		Size: 635.2 KB (635211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a8b3d97f9ec158a76cc7a9b135022d2879c8bad50545e8489b035c5ec117bb`  
		Last Modified: Tue, 01 Nov 2016 17:47:25 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf2e5d403074cda795f6dbb5eb780c54d1228c4721baecc38d81207f376f75b`  
		Last Modified: Tue, 01 Nov 2016 17:47:25 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d7b126890936d56eda9052eb4d78f32533381bc4bea0b621ddbbd9cd9ffff9`  
		Last Modified: Tue, 01 Nov 2016 17:47:47 GMT  
		Size: 130.8 MB (130834247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e1a5ba0ef9b1c4cce3beb8bd69da4910d14329b133eff8a907157d53b82031`  
		Last Modified: Tue, 01 Nov 2016 21:10:02 GMT  
		Size: 8.6 MB (8598855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a600c2f6671c0be801df4b944103f1fae7f6262ff6cb6c5abc916b2b584984`  
		Last Modified: Tue, 01 Nov 2016 21:10:00 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f7204b7980e92509a4511f548b3d6d6e51d8ce18275231a061b4d1dc9b1547`  
		Last Modified: Tue, 01 Nov 2016 21:10:00 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a38911a8551d1fad5973bac3be29ec5b274d3d5086ae3fe1d32fd73c14cedaa`  
		Last Modified: Tue, 01 Nov 2016 21:10:47 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3.3-jdk-9-onbuild`

```console
$ docker pull maven@sha256:6afd01c75be4e929ce966ef4cf33e97073700f2f40b88e832067af810a9f9d10
```

-	Platforms:
	-	linux; amd64

### `maven:3.3-jdk-9-onbuild` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.1 MB (252134509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a182ec57db005bdf1e0a87db5a8613ab58bbd74a302770af34453d37888a573`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 17 Oct 2016 21:26:09 GMT
ADD file:7a91bb1a28e088d8d427022bb612873476ea54ec75cb559e5943b771d7412386 in / 
# Mon, 17 Oct 2016 21:26:10 GMT
CMD ["/bin/bash"]
# Mon, 17 Oct 2016 23:39:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Mon, 17 Oct 2016 23:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Oct 2016 20:40:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:55:25 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
# Mon, 31 Oct 2016 21:55:26 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:55:27 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:55:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-9-openjdk-amd64
# Tue, 01 Nov 2016 17:32:07 GMT
ENV JAVA_VERSION=9~b142
# Tue, 01 Nov 2016 17:32:07 GMT
ENV JAVA_DEBIAN_VERSION=9~b142-1
# Tue, 01 Nov 2016 17:33:02 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-9-jdk-headless="$JAVA_DEBIAN_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 01 Nov 2016 21:09:43 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 21:09:43 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 21:09:46 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 21:09:46 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 21:09:47 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 21:09:47 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 21:09:48 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 21:09:48 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 21:09:49 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 21:09:49 GMT
CMD ["mvn"]
# Tue, 01 Nov 2016 21:10:34 GMT
RUN mkdir -p /usr/src/app
# Tue, 01 Nov 2016 21:10:35 GMT
WORKDIR /usr/src/app
# Tue, 01 Nov 2016 21:10:35 GMT
ONBUILD ADD . /usr/src/app
# Tue, 01 Nov 2016 21:10:35 GMT
ONBUILD RUN mvn install
```

-	Layers:
	-	`sha256:279daf9814f4ba6feba147fd51356389273017b7d4a057e5a7cf724467c2fbcd`  
		Last Modified: Mon, 17 Oct 2016 21:26:30 GMT  
		Size: 43.2 MB (43195045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee53d9e55ce8c4310eed9df888489b1e79dc22764f3c442d8e767d0f4218b57`  
		Last Modified: Mon, 17 Oct 2016 23:40:01 GMT  
		Size: 20.6 MB (20581005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1bde82dbdb2519006f9578e8408db12a546bf1b5ae03940b08f3f20ca8b3dc`  
		Last Modified: Mon, 17 Oct 2016 23:41:03 GMT  
		Size: 48.3 MB (48288494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af9bebd3ac92605303612e9f49a36146006a2e79a5854e87e6027cc653ba2f`  
		Last Modified: Tue, 18 Oct 2016 20:54:37 GMT  
		Size: 635.2 KB (635211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a8b3d97f9ec158a76cc7a9b135022d2879c8bad50545e8489b035c5ec117bb`  
		Last Modified: Tue, 01 Nov 2016 17:47:25 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf2e5d403074cda795f6dbb5eb780c54d1228c4721baecc38d81207f376f75b`  
		Last Modified: Tue, 01 Nov 2016 17:47:25 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d7b126890936d56eda9052eb4d78f32533381bc4bea0b621ddbbd9cd9ffff9`  
		Last Modified: Tue, 01 Nov 2016 17:47:47 GMT  
		Size: 130.8 MB (130834247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e1a5ba0ef9b1c4cce3beb8bd69da4910d14329b133eff8a907157d53b82031`  
		Last Modified: Tue, 01 Nov 2016 21:10:02 GMT  
		Size: 8.6 MB (8598855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a600c2f6671c0be801df4b944103f1fae7f6262ff6cb6c5abc916b2b584984`  
		Last Modified: Tue, 01 Nov 2016 21:10:00 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f7204b7980e92509a4511f548b3d6d6e51d8ce18275231a061b4d1dc9b1547`  
		Last Modified: Tue, 01 Nov 2016 21:10:00 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a38911a8551d1fad5973bac3be29ec5b274d3d5086ae3fe1d32fd73c14cedaa`  
		Last Modified: Tue, 01 Nov 2016 21:10:47 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `maven:3-jdk-9-onbuild`

```console
$ docker pull maven@sha256:6afd01c75be4e929ce966ef4cf33e97073700f2f40b88e832067af810a9f9d10
```

-	Platforms:
	-	linux; amd64

### `maven:3-jdk-9-onbuild` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.1 MB (252134509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a182ec57db005bdf1e0a87db5a8613ab58bbd74a302770af34453d37888a573`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 17 Oct 2016 21:26:09 GMT
ADD file:7a91bb1a28e088d8d427022bb612873476ea54ec75cb559e5943b771d7412386 in / 
# Mon, 17 Oct 2016 21:26:10 GMT
CMD ["/bin/bash"]
# Mon, 17 Oct 2016 23:39:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Mon, 17 Oct 2016 23:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Oct 2016 20:40:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:55:25 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
# Mon, 31 Oct 2016 21:55:26 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:55:27 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:55:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-9-openjdk-amd64
# Tue, 01 Nov 2016 17:32:07 GMT
ENV JAVA_VERSION=9~b142
# Tue, 01 Nov 2016 17:32:07 GMT
ENV JAVA_DEBIAN_VERSION=9~b142-1
# Tue, 01 Nov 2016 17:33:02 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-9-jdk-headless="$JAVA_DEBIAN_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 01 Nov 2016 21:09:43 GMT
ARG MAVEN_VERSION=3.3.9
# Tue, 01 Nov 2016 21:09:43 GMT
ARG USER_HOME_DIR=/root
# Tue, 01 Nov 2016 21:09:46 GMT
# ARGS: MAVEN_VERSION=3.3.9 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL http://apache.osuosl.org/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz     | tar -xzC /usr/share/maven --strip-components=1   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 01 Nov 2016 21:09:46 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 01 Nov 2016 21:09:47 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 01 Nov 2016 21:09:47 GMT
COPY file:e3aa30a24fcf60a59710465ac66fc1d53c35590a74fcdd51e12a5cbce393904b in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 01 Nov 2016 21:09:48 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 01 Nov 2016 21:09:48 GMT
VOLUME [/root/.m2]
# Tue, 01 Nov 2016 21:09:49 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 01 Nov 2016 21:09:49 GMT
CMD ["mvn"]
# Tue, 01 Nov 2016 21:10:34 GMT
RUN mkdir -p /usr/src/app
# Tue, 01 Nov 2016 21:10:35 GMT
WORKDIR /usr/src/app
# Tue, 01 Nov 2016 21:10:35 GMT
ONBUILD ADD . /usr/src/app
# Tue, 01 Nov 2016 21:10:35 GMT
ONBUILD RUN mvn install
```

-	Layers:
	-	`sha256:279daf9814f4ba6feba147fd51356389273017b7d4a057e5a7cf724467c2fbcd`  
		Last Modified: Mon, 17 Oct 2016 21:26:30 GMT  
		Size: 43.2 MB (43195045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee53d9e55ce8c4310eed9df888489b1e79dc22764f3c442d8e767d0f4218b57`  
		Last Modified: Mon, 17 Oct 2016 23:40:01 GMT  
		Size: 20.6 MB (20581005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1bde82dbdb2519006f9578e8408db12a546bf1b5ae03940b08f3f20ca8b3dc`  
		Last Modified: Mon, 17 Oct 2016 23:41:03 GMT  
		Size: 48.3 MB (48288494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af9bebd3ac92605303612e9f49a36146006a2e79a5854e87e6027cc653ba2f`  
		Last Modified: Tue, 18 Oct 2016 20:54:37 GMT  
		Size: 635.2 KB (635211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a8b3d97f9ec158a76cc7a9b135022d2879c8bad50545e8489b035c5ec117bb`  
		Last Modified: Tue, 01 Nov 2016 17:47:25 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf2e5d403074cda795f6dbb5eb780c54d1228c4721baecc38d81207f376f75b`  
		Last Modified: Tue, 01 Nov 2016 17:47:25 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d7b126890936d56eda9052eb4d78f32533381bc4bea0b621ddbbd9cd9ffff9`  
		Last Modified: Tue, 01 Nov 2016 17:47:47 GMT  
		Size: 130.8 MB (130834247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e1a5ba0ef9b1c4cce3beb8bd69da4910d14329b133eff8a907157d53b82031`  
		Last Modified: Tue, 01 Nov 2016 21:10:02 GMT  
		Size: 8.6 MB (8598855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a600c2f6671c0be801df4b944103f1fae7f6262ff6cb6c5abc916b2b584984`  
		Last Modified: Tue, 01 Nov 2016 21:10:00 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f7204b7980e92509a4511f548b3d6d6e51d8ce18275231a061b4d1dc9b1547`  
		Last Modified: Tue, 01 Nov 2016 21:10:00 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a38911a8551d1fad5973bac3be29ec5b274d3d5086ae3fe1d32fd73c14cedaa`  
		Last Modified: Tue, 01 Nov 2016 21:10:47 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
