## `jruby:9-alpine`

```console
$ docker pull jruby@sha256:955808eb0938cb3330e49d458eab3ed53601e91ff1e01a801f2225be3ebb009f
```

-	Platforms:
	-	linux; amd64

### `jruby:9-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75962677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9fab17c7688798179678cb0f48b0ba87dc1dc98f6e436db810145c748ae55f`
-	Default Command: `["irb"]`

```dockerfile
# Mon, 29 Aug 2016 23:49:14 GMT
ADD file:852e9d0cb9d906535af512a89339fc70b2873a0f94defbcbe41cd44942dd6ac8 in / 
# Tue, 30 Aug 2016 19:53:16 GMT
ENV LANG=C.UTF-8
# Tue, 30 Aug 2016 19:53:17 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 30 Aug 2016 19:56:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk/jre
# Tue, 30 Aug 2016 19:56:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Tue, 30 Aug 2016 19:56:05 GMT
ENV JAVA_VERSION=8u92
# Tue, 30 Aug 2016 19:56:05 GMT
ENV JAVA_ALPINE_VERSION=8.92.14-r1
# Tue, 30 Aug 2016 19:56:10 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8-jre="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 30 Aug 2016 20:09:11 GMT
RUN apk add --no-cache       bash       libc6-compat
# Thu, 08 Sep 2016 17:59:50 GMT
ENV JRUBY_VERSION=9.1.5.0
# Thu, 08 Sep 2016 17:59:50 GMT
ENV JRUBY_SHA256=28e4f3aefbb4497c5c5edc04246778b3305105c3d3d6de11be067826cc5bb766
# Thu, 08 Sep 2016 17:59:57 GMT
RUN apk add --no-cache --virtual .build-deps       curl       tar   && mkdir -p /opt/jruby   && curl -fSL https://s3.amazonaws.com/jruby.org/downloads/${JRUBY_VERSION}/jruby-bin-${JRUBY_VERSION}.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 */tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && ln -s /opt/jruby/bin/jruby /usr/local/bin/ruby   && apk del .build-deps
# Thu, 08 Sep 2016 17:59:58 GMT
ENV PATH=/opt/jruby/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Thu, 08 Sep 2016 17:59:58 GMT
RUN mkdir -p /opt/jruby/etc     && {         echo 'install: --no-document';         echo 'update: --no-document';     } >> /opt/jruby/etc/gemrc
# Thu, 08 Sep 2016 18:00:08 GMT
RUN gem install bundler
# Thu, 08 Sep 2016 18:00:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Sep 2016 18:00:09 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_BIN=/usr/local/bundle/bin BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Sep 2016 18:00:09 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Thu, 08 Sep 2016 18:00:10 GMT
RUN mkdir -p "$GEM_HOME" "$BUNDLE_BIN"     && chmod 777 "$GEM_HOME" "$BUNDLE_BIN"
# Thu, 08 Sep 2016 18:00:10 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:e110a4a1794126ef308a49f2d65785af2f25538f06700721aad8283b81fdfa58`  
		Last Modified: Thu, 23 Jun 2016 19:56:16 GMT  
		Size: 2.3 MB (2310286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a696cba1f6e865421664a7bf9bf585bcfaa924d56b7d2a112a799e00a7433791`  
		Last Modified: Tue, 30 Aug 2016 21:11:27 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc427bd93e958b2f8b2cadc810c692edbba6856a8ff08434066b43be35ec6b68`  
		Last Modified: Tue, 30 Aug 2016 21:11:37 GMT  
		Size: 39.6 MB (39647584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97edc5003bec2706446592539d168a6a1d46c85555e2d96d6d75e973f37cb03e`  
		Last Modified: Tue, 30 Aug 2016 21:53:45 GMT  
		Size: 1.5 MB (1477719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71af39d7ffc098b7ce0d2a5269e11a1d22be9305ed0a5d0b0792f888de1851e6`  
		Last Modified: Thu, 08 Sep 2016 18:02:26 GMT  
		Size: 32.0 MB (31969209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f144af729354792f20c93315a5ca26bae496098d4f70939d4729ab88ffb66380`  
		Last Modified: Thu, 08 Sep 2016 18:02:23 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239664674ea7b5b3ea6171585bddaeaa1fbc6a89a4b73d7d94f6f099629d2a66`  
		Last Modified: Thu, 08 Sep 2016 18:02:24 GMT  
		Size: 557.3 KB (557295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da225007fa8904afa475ce691150aaf6fb2136bd6d64b7fc4ced0604fb521a2c`  
		Last Modified: Thu, 08 Sep 2016 18:02:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip