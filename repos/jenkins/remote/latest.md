## `jenkins:latest`

```console
$ docker pull jenkins@sha256:ed88a89fd774d5898c37d1f04246b90dd2b98319a446a725ad3127397488e392
```

-	Platforms:
	-	linux; amd64

### `jenkins:latest` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.3 MB (313254819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55720d63e3285b2ce23316063259337c8550c28d459307cc910ae956b9fd5bac`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/jenkins.sh"]`

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
# Tue, 01 Nov 2016 20:30:04 GMT
RUN apt-get update && apt-get install -y git curl && rm -rf /var/lib/apt/lists/*
# Tue, 01 Nov 2016 20:30:05 GMT
ENV JENKINS_HOME=/var/jenkins_home
# Tue, 01 Nov 2016 20:30:05 GMT
ENV JENKINS_SLAVE_AGENT_PORT=50000
# Tue, 01 Nov 2016 20:30:05 GMT
ARG user=jenkins
# Tue, 01 Nov 2016 20:30:06 GMT
ARG group=jenkins
# Tue, 01 Nov 2016 20:30:06 GMT
ARG uid=1000
# Tue, 01 Nov 2016 20:30:07 GMT
ARG gid=1000
# Tue, 01 Nov 2016 20:30:08 GMT
# ARGS: gid=1000 group=jenkins uid=1000 user=jenkins
RUN groupadd -g ${gid} ${group}     && useradd -d "$JENKINS_HOME" -u ${uid} -g ${gid} -m -s /bin/bash ${user}
# Tue, 01 Nov 2016 20:30:08 GMT
VOLUME [/var/jenkins_home]
# Tue, 01 Nov 2016 20:30:09 GMT
# ARGS: gid=1000 group=jenkins uid=1000 user=jenkins
RUN mkdir -p /usr/share/jenkins/ref/init.groovy.d
# Tue, 01 Nov 2016 20:30:10 GMT
ENV TINI_VERSION=0.9.0
# Tue, 01 Nov 2016 20:30:10 GMT
ENV TINI_SHA=fa23d1e20732501c3bb8eeeca423c89ac80ed452
# Tue, 01 Nov 2016 20:30:13 GMT
# ARGS: gid=1000 group=jenkins uid=1000 user=jenkins
RUN curl -fsSL https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-static -o /bin/tini && chmod +x /bin/tini   && echo "$TINI_SHA  /bin/tini" | sha1sum -c -
# Tue, 01 Nov 2016 20:30:14 GMT
COPY file:c629bc0b9ecb5b7233000c973f65721df4ce1307a5d5b33ac3871ff61a9172ff in /usr/share/jenkins/ref/init.groovy.d/tcp-slave-agent-port.groovy 
# Tue, 01 Nov 2016 20:30:14 GMT
ARG JENKINS_VERSION
# Tue, 01 Nov 2016 20:30:15 GMT
ENV JENKINS_VERSION=2.19.1
# Tue, 01 Nov 2016 20:30:15 GMT
ARG JENKINS_SHA=dc28b91e553c1cd42cc30bd75d0f651671e6de0b
# Tue, 01 Nov 2016 20:30:16 GMT
ARG JENKINS_URL=http://repo.jenkins-ci.org/public/org/jenkins-ci/main/jenkins-war/2.19.1/jenkins-war-2.19.1.war
# Tue, 01 Nov 2016 20:30:21 GMT
# ARGS: JENKINS_SHA=dc28b91e553c1cd42cc30bd75d0f651671e6de0b JENKINS_URL=http://repo.jenkins-ci.org/public/org/jenkins-ci/main/jenkins-war/2.19.1/jenkins-war-2.19.1.war gid=1000 group=jenkins uid=1000 user=jenkins
RUN curl -fsSL ${JENKINS_URL} -o /usr/share/jenkins/jenkins.war   && echo "${JENKINS_SHA}  /usr/share/jenkins/jenkins.war" | sha1sum -c -
# Tue, 01 Nov 2016 20:30:21 GMT
ENV JENKINS_UC=https://updates.jenkins.io
# Tue, 01 Nov 2016 20:30:22 GMT
# ARGS: JENKINS_SHA=dc28b91e553c1cd42cc30bd75d0f651671e6de0b JENKINS_URL=http://repo.jenkins-ci.org/public/org/jenkins-ci/main/jenkins-war/2.19.1/jenkins-war-2.19.1.war gid=1000 group=jenkins uid=1000 user=jenkins
RUN chown -R ${user} "$JENKINS_HOME" /usr/share/jenkins/ref
# Tue, 01 Nov 2016 20:30:23 GMT
EXPOSE 8080/tcp
# Tue, 01 Nov 2016 20:30:23 GMT
EXPOSE 50000/tcp
# Tue, 01 Nov 2016 20:30:24 GMT
ENV COPY_REFERENCE_FILE_LOG=/var/jenkins_home/copy_reference_file.log
# Tue, 01 Nov 2016 20:30:24 GMT
USER [jenkins]
# Tue, 01 Nov 2016 20:30:25 GMT
COPY file:26c3c5818bc87662d1f4905a3ed73bd55a0a75f731c7dc52d0599c00f51408e9 in /usr/local/bin/jenkins-support 
# Tue, 01 Nov 2016 20:30:26 GMT
COPY file:7af8c0bd35066db9b0d029c9b74e72bf81420b1fd51ee55d2c28a26c36f829dd in /usr/local/bin/jenkins.sh 
# Tue, 01 Nov 2016 20:30:26 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/jenkins.sh"]
# Tue, 01 Nov 2016 20:30:27 GMT
COPY file:93fb511d485dd2d6060c484dcedb902947875042048de529676a0a0aed27b5a3 in /usr/local/bin/plugins.sh 
# Tue, 01 Nov 2016 20:30:28 GMT
COPY file:2a6a3e16202b8dddab5edef50f712c16fe8f6980f5aea80c8c76b5db4f903913 in /usr/local/bin/install-plugins.sh 
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
	-	`sha256:500a4c89bfdd5c941fc15ba7dbd1b2d824d452ff2f500f8c461a5dfacf40638f`  
		Last Modified: Tue, 01 Nov 2016 20:30:45 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81908e885bb81a1520a62e5a6c0e4fcbed73654df4bb5f5e20be1d13e6dbcd95`  
		Last Modified: Tue, 01 Nov 2016 20:30:42 GMT  
		Size: 4.4 KB (4395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb4df1a440333d070ff95db2567118aa1318a084ef73c35e201dab2326926b3`  
		Last Modified: Tue, 01 Nov 2016 20:30:42 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cf508b0033d3087b452baf8e100dfd31ea862d16d4599c42d1494fb821b36b`  
		Last Modified: Tue, 01 Nov 2016 20:30:42 GMT  
		Size: 337.2 KB (337236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfbae318ffe1f814143392a0bd85e68b85e40c74fd3c6bf839907910dbba757`  
		Last Modified: Tue, 01 Nov 2016 20:30:41 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3c2b2f66589de256ffeceda0df2a59d34d34be034a8b6414571a1a8e85b43d`  
		Last Modified: Tue, 01 Nov 2016 20:30:47 GMT  
		Size: 69.5 MB (69542135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485b713d03ffc56faa716effb21104da79a3cc5bcbd4d8e703710d7fe798844c`  
		Last Modified: Tue, 01 Nov 2016 20:30:38 GMT  
		Size: 425.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cbbeb4c01592d267e8e6d0c318cf473f277ce57a5aadf40655229b8bc28944`  
		Last Modified: Tue, 01 Nov 2016 20:30:39 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e076a218a80cf19cb4da3fda23902ab7212c5461d21c8acc29db221f8e6dfbae`  
		Last Modified: Tue, 01 Nov 2016 20:30:38 GMT  
		Size: 819.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe914e4cec916d71ab4340b2a432fdf3fd26946fb3d8e0b0fb848b8fad03154`  
		Last Modified: Tue, 01 Nov 2016 20:30:39 GMT  
		Size: 1.5 KB (1523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755133f83251df5ca869b04084282480c11af7f319e331475c457d994187a615`  
		Last Modified: Tue, 01 Nov 2016 20:30:39 GMT  
		Size: 2.2 KB (2177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
