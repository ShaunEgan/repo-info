## `jruby:latest`

```console
$ docker pull jruby@sha256:bbdf73799d5af084a6879c6d038b00421fdca9ab677ee5dda662ef4c29151e84
```

-	Platforms:
	-	linux; amd64

### `jruby:latest` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.5 MB (161502433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc59e1b16a6b514db7b6c060c0721cad6428384d47162d0caa09dda6fb5d5993`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:10:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Oct 2016 21:55:01 GMT
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Mon, 31 Oct 2016 21:55:02 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2016 21:55:03 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 31 Oct 2016 21:55:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64/jre
# Mon, 31 Oct 2016 21:55:03 GMT
ENV JAVA_VERSION=8u102
# Mon, 31 Oct 2016 21:55:04 GMT
ENV JAVA_DEBIAN_VERSION=8u102-b14.1-1~bpo8+1
# Mon, 31 Oct 2016 21:55:04 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20140324
# Mon, 31 Oct 2016 21:55:22 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-8-jre-headless="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 31 Oct 2016 21:55:24 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 01 Nov 2016 05:32:35 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 01 Nov 2016 20:40:21 GMT
ENV JRUBY_VERSION=9.1.5.0
# Tue, 01 Nov 2016 20:40:21 GMT
ENV JRUBY_SHA256=28e4f3aefbb4497c5c5edc04246778b3305105c3d3d6de11be067826cc5bb766
# Tue, 01 Nov 2016 20:40:28 GMT
RUN mkdir /opt/jruby   && curl -fSL https://s3.amazonaws.com/jruby.org/downloads/${JRUBY_VERSION}/jruby-bin-${JRUBY_VERSION}.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 01 Nov 2016 20:40:28 GMT
ENV PATH=/opt/jruby/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2016 20:40:29 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 01 Nov 2016 20:40:39 GMT
RUN gem install bundler
# Tue, 01 Nov 2016 20:40:40 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 01 Nov 2016 20:40:40 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_BIN=/usr/local/bundle/bin BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 01 Nov 2016 20:40:41 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2016 20:40:42 GMT
RUN mkdir -p "$GEM_HOME" "$BUNDLE_BIN" 	&& chmod 777 "$GEM_HOME" "$BUNDLE_BIN"
# Tue, 01 Nov 2016 20:40:42 GMT
CMD ["irb"]
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
	-	`sha256:2b7b4d10e1c13c063d94bb83588b327f4c4f5a10fb1a1a89a9c1c73ef15710a7`  
		Last Modified: Fri, 21 Oct 2016 20:11:17 GMT  
		Size: 566.6 KB (566556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264389d8f2fec4e89e2293411211bb57154f24ad836163d897d019b97d5fd5c`  
		Last Modified: Tue, 01 Nov 2016 05:33:16 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2c46e93f4ac4f4f2f114c689f42a1435409b2db78ab6d19f525866037de473`  
		Last Modified: Tue, 01 Nov 2016 05:33:12 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9506bb322c04c882de48ee789337b636c47cf67c89c402a686f4a03dc6c1eb9`  
		Last Modified: Tue, 01 Nov 2016 05:33:24 GMT  
		Size: 53.4 MB (53439646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f5dad14c2c78802e41cc9c1722caf14f5d7437a81c6d59855b9a835102d67a`  
		Last Modified: Tue, 01 Nov 2016 05:33:10 GMT  
		Size: 284.2 KB (284204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4ab534d298afc09d3103f022896674d076b3dc927c03f791d955c6d5b8c9ba`  
		Last Modified: Tue, 01 Nov 2016 05:33:10 GMT  
		Size: 4.8 MB (4829529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3436abf7c65bd20868bfca5dd8484c1a6f1e4c0a866a9b28d593ff96485f9d`  
		Last Modified: Tue, 01 Nov 2016 20:40:58 GMT  
		Size: 31.9 MB (31887909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9a10f40c27605cb7a8bf3f9ba9683bb51e679b8a6f39e53749f9faf93114ab`  
		Last Modified: Tue, 01 Nov 2016 20:40:53 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb81bbe8eba5bb6d58664965931f8923728429d983cf2414f2e5a6dcb5165e6`  
		Last Modified: Tue, 01 Nov 2016 20:40:54 GMT  
		Size: 612.5 KB (612520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71406be5dabd9a3a32fc9a1df5704b5f14125fc06c1685fc75b2651e34f23242`  
		Last Modified: Tue, 01 Nov 2016 20:40:53 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
