## `php:5-alpine`

```console
$ docker pull php@sha256:07863a34f2be060572c34f714c2cab1e9f821a55afe26651132c19ec46b2745d
```

-	Platforms:
	-	linux; amd64

### `php:5-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22906981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a21df5039ef8a83f7d0657d3387d79e87c99f2d9ad457a783b2808a62d528eca`
-	Default Command: `["php","-a"]`

```dockerfile
# Mon, 29 Aug 2016 23:49:14 GMT
ADD file:852e9d0cb9d906535af512a89339fc70b2873a0f94defbcbe41cd44942dd6ac8 in / 
# Tue, 30 Aug 2016 16:38:39 GMT
ENV PHPIZE_DEPS=autoconf 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Aug 2016 16:38:40 GMT
RUN apk add --no-cache --virtual .persistent-deps 		ca-certificates 		curl 		tar 		xz
# Tue, 30 Aug 2016 16:38:41 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Aug 2016 16:38:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Aug 2016 16:38:42 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Tue, 30 Aug 2016 17:04:18 GMT
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
# Tue, 30 Aug 2016 17:04:18 GMT
ENV PHP_VERSION=5.6.25
# Tue, 30 Aug 2016 17:04:19 GMT
ENV PHP_FILENAME=php-5.6.25.tar.xz
# Tue, 30 Aug 2016 17:04:19 GMT
ENV PHP_SHA256=7535cd6e20040ccec4594cc386c6f15c3f2c88f24163294a31068cf7dfe7f644
# Tue, 30 Aug 2016 17:04:29 GMT
RUN set -xe 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 	&& mkdir -p /usr/src 	&& cd /usr/src 	&& curl -fSL "https://secure.php.net/get/$PHP_FILENAME/from/this/mirror" -o php.tar.xz 	&& echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c - 	&& curl -fSL "https://secure.php.net/get/$PHP_FILENAME.asc/from/this/mirror" -o php.tar.xz.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done 	&& gpg --batch --verify php.tar.xz.asc php.tar.xz 	&& rm -r "$GNUPGHOME" 	&& apk del .fetch-deps
# Tue, 30 Aug 2016 17:04:30 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Tue, 30 Aug 2016 17:08:04 GMT
RUN set -xe 	&& apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		curl-dev 		libedit-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 		&& docker-php-source extract 	&& cd /usr/src/php 	&& ./configure 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j"$(getconf _NPROCESSORS_ONLN)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& docker-php-source delete 		&& runDeps="$( 		scanelf --needed --nobanner --recursive /usr/local 			| awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }' 			| sort -u 			| xargs -r apk info --installed 			| sort -u 	)" 	&& apk add --no-cache --virtual .php-rundeps $runDeps 		&& apk del .build-deps
# Tue, 30 Aug 2016 17:08:05 GMT
COPY multi:ed54b4fe7bef284934703fa6e979b7cc0daed0549a07586d0c1ccd4e2b41884a in /usr/local/bin/ 
# Tue, 30 Aug 2016 17:08:05 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:e110a4a1794126ef308a49f2d65785af2f25538f06700721aad8283b81fdfa58`  
		Last Modified: Thu, 23 Jun 2016 19:56:16 GMT  
		Size: 2.3 MB (2310286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e161e9d6929b9a7736e565c6bb73c386617d410c1acb38b1f444b51c2d623b4`  
		Last Modified: Wed, 07 Sep 2016 18:55:33 GMT  
		Size: 1.0 MB (1047590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d196bef415b6de51bf0b60843ff47d9875d6cbbdd8d12a54c61d3849bdefae4`  
		Last Modified: Wed, 07 Sep 2016 18:55:33 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b12a7178d880fd91653abf89153c0eaf2372868943c2f4fc2346677b424a56`  
		Last Modified: Wed, 07 Sep 2016 18:55:30 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b537d43bb0965e212b381bde075bffda5642e2bc9611b6f3dc0f7849832a9b84`  
		Last Modified: Wed, 07 Sep 2016 19:03:45 GMT  
		Size: 12.4 MB (12423799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201ad89cb00fbdf60de1365e8c28ef58d6ec56d5c74a169bec78dba5e2b74270`  
		Last Modified: Wed, 07 Sep 2016 19:03:43 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3d82ad88b58a247333df482e7fe536fb992913caf99e79c49693bbcd57a775`  
		Last Modified: Wed, 07 Sep 2016 19:03:48 GMT  
		Size: 7.1 MB (7121568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be03d6ae8b6c3fe35f32400896591a7978a4db560ef6dd9c313334687d133140`  
		Last Modified: Wed, 07 Sep 2016 19:03:44 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip