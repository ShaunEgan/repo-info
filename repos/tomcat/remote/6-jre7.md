## `tomcat:6-jre7`

```console
$ docker pull tomcat@sha256:a7b94978dabc5a88b22c19477ab4f985ff987a66bb132899e695cfb7dcac4bc4
```

-	Platforms:
	-	linux; amd64

### `tomcat:6-jre7` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.3 MB (159323472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59f698607953083eee1154af79d944a101dfb7077c556569b76df96752f4fe18`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:10:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 20:10:25 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2016 20:10:26 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 21 Oct 2016 20:10:26 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-7-openjdk-amd64/jre
# Fri, 21 Oct 2016 20:10:26 GMT
ENV JAVA_VERSION=7u111
# Fri, 21 Oct 2016 20:10:27 GMT
ENV JAVA_DEBIAN_VERSION=7u111-2.6.7-1~deb8u1
# Fri, 21 Oct 2016 20:11:06 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		openjdk-7-jre-headless="$JAVA_DEBIAN_VERSION" 	&& rm -rf /var/lib/apt/lists/* 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sat, 22 Oct 2016 01:47:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Oct 2016 01:47:07 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Oct 2016 01:47:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Oct 2016 01:47:09 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Oct 2016 01:47:09 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Oct 2016 01:47:09 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Oct 2016 01:47:10 GMT
ENV OPENSSL_VERSION=1.0.2j-1
# Tue, 01 Nov 2016 01:00:57 GMT
RUN { 		echo 'deb http://deb.debian.org/debian unstable main'; 	} > /etc/apt/sources.list.d/unstable.list 	&& { 		echo 'Package: *'; 		echo 'Pin: release a=unstable'; 		echo 'Pin-Priority: -10'; 		echo; 		echo 'Package: openssl libssl*'; 		echo "Pin: version $OPENSSL_VERSION"; 		echo 'Pin-Priority: 990'; 	} > /etc/apt/preferences.d/unstable-openssl
# Tue, 01 Nov 2016 01:01:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libapr1 		openssl="$OPENSSL_VERSION" 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Nov 2016 01:01:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 80FF76D88A969FE46108558A80B953A041E49465 8B39757B1D8A994DF2433ED58B3A601F08C975E5 A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 B3F49CD3B9BD2996DA90F817ED3873F5D3262722 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 01 Nov 2016 01:02:20 GMT
RUN set -ex; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done
# Tue, 01 Nov 2016 01:02:21 GMT
ENV TOMCAT_MAJOR=6
# Tue, 01 Nov 2016 01:02:21 GMT
ENV TOMCAT_VERSION=6.0.47
# Tue, 01 Nov 2016 01:02:21 GMT
ENV TOMCAT_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=tomcat/tomcat-6/v6.0.47/bin/apache-tomcat-6.0.47.tar.gz
# Tue, 01 Nov 2016 01:02:22 GMT
ENV TOMCAT_ASC_URL=https://www.apache.org/dist/tomcat/tomcat-6/v6.0.47/bin/apache-tomcat-6.0.47.tar.gz.asc
# Tue, 01 Nov 2016 01:03:04 GMT
RUN set -x 		&& wget -O tomcat.tar.gz "$TOMCAT_TGZ_URL" 	&& wget -O tomcat.tar.gz.asc "$TOMCAT_ASC_URL" 	&& gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz 	&& tar -xvf tomcat.tar.gz --strip-components=1 	&& rm bin/*.bat 	&& rm tomcat.tar.gz* 		&& nativeBuildDir="$(mktemp -d)" 	&& tar -xvf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1 	&& nativeBuildDeps=" 		gcc 		libapr1-dev 		libssl-dev 		make 		openjdk-${JAVA_VERSION%%[-~bu]*}-jdk=$JAVA_DEBIAN_VERSION 	" 	&& apt-get update && apt-get install -y --no-install-recommends $nativeBuildDeps && rm -rf /var/lib/apt/lists/* 	&& ( 		export CATALINA_HOME="$PWD" 		&& cd "$nativeBuildDir/native" 		&& ./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$(which apr-1-config)" 			--with-java-home="$(docker-java-home)" 			--with-ssl=yes 		&& make -j$(nproc) 		&& make install 	) 	&& apt-get purge -y --auto-remove $nativeBuildDeps 	&& rm -rf "$nativeBuildDir" 	&& rm bin/tomcat-native.tar.gz
# Tue, 01 Nov 2016 01:03:04 GMT
EXPOSE 8080/tcp
# Tue, 01 Nov 2016 01:03:05 GMT
CMD ["catalina.sh" "run"]
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
	-	`sha256:35dfd23791b53c2fae237e583621203cd5e4434fcdc0254d94ca83b147286666`  
		Last Modified: Fri, 21 Oct 2016 20:11:16 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0aca12f0dd9d53ec59f50958e2a10bbacbdc29757327b216c13f6ca8214f4c`  
		Last Modified: Fri, 21 Oct 2016 20:11:31 GMT  
		Size: 77.7 MB (77740287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3e424fb5e81e76b782f1e574d13ada30882ef94304008786d45ac449965f1e`  
		Last Modified: Sat, 22 Oct 2016 01:49:31 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3134459e064cf1cd8db42ded4b0db802b571dda536976f3fe24285da724bd250`  
		Last Modified: Tue, 01 Nov 2016 01:11:25 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3189bffb00a14e014ea78167059a646c5c1f8c00da8e00a0a82893f071e25951`  
		Last Modified: Tue, 01 Nov 2016 01:11:26 GMT  
		Size: 3.0 MB (3001044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3f47b7becd791987d0e463b0dadd173ee9605f9b8228b9841064b9963edc79`  
		Last Modified: Tue, 01 Nov 2016 01:11:25 GMT  
		Size: 273.8 KB (273838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f488f766d7c9d3781ae764ded6b0bb43ca8e519d384a5c0c7bd0a5453b9752`  
		Last Modified: Tue, 01 Nov 2016 01:11:27 GMT  
		Size: 7.9 MB (7859773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
