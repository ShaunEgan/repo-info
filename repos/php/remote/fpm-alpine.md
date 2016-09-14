## `php:fpm-alpine`

```console
$ docker pull php@sha256:f9546624b56f179b6a8d366a4349c059fb7bd7772bf6fcb3c079a7d29e5b5396
```

-	Platforms:
	-	linux; amd64

### `php:fpm-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30677996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7085d3053452d4728a5beeed8538c7956496a5922afef4bf921f90b1ab0d0a8e`
-	Default Command: `["php-fpm"]`

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
# Tue, 30 Aug 2016 16:49:03 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data
# Tue, 30 Aug 2016 16:49:03 GMT
ENV GPG_KEYS=1A4E8B7277C42E53DBA9C7B9BCAA30EA9C0D5763
# Tue, 30 Aug 2016 16:49:04 GMT
ENV PHP_VERSION=7.0.10
# Tue, 30 Aug 2016 16:49:04 GMT
ENV PHP_FILENAME=php-7.0.10.tar.xz
# Tue, 30 Aug 2016 16:49:04 GMT
ENV PHP_SHA256=348476ff7ba8d95a1e28e1059430c10470c5f8110f6d9133d30153dda4cdf56a
# Tue, 30 Aug 2016 16:49:11 GMT
RUN set -xe 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 	&& mkdir -p /usr/src 	&& cd /usr/src 	&& curl -fSL "https://secure.php.net/get/$PHP_FILENAME/from/this/mirror" -o php.tar.xz 	&& echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c - 	&& curl -fSL "https://secure.php.net/get/$PHP_FILENAME.asc/from/this/mirror" -o php.tar.xz.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done 	&& gpg --batch --verify php.tar.xz.asc php.tar.xz 	&& rm -r "$GNUPGHOME" 	&& apk del .fetch-deps
# Tue, 30 Aug 2016 16:49:11 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Tue, 30 Aug 2016 16:53:01 GMT
RUN set -xe 	&& apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		curl-dev 		libedit-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 		&& docker-php-source extract 	&& cd /usr/src/php 	&& ./configure 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j"$(getconf _NPROCESSORS_ONLN)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& docker-php-source delete 		&& runDeps="$( 		scanelf --needed --nobanner --recursive /usr/local 			| awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }' 			| sort -u 			| xargs -r apk info --installed 			| sort -u 	)" 	&& apk add --no-cache --virtual .php-rundeps $runDeps 		&& apk del .build-deps
# Tue, 30 Aug 2016 16:53:01 GMT
COPY multi:ed54b4fe7bef284934703fa6e979b7cc0daed0549a07586d0c1ccd4e2b41884a in /usr/local/bin/ 
# Tue, 30 Aug 2016 16:53:02 GMT
WORKDIR /var/www/html
# Tue, 30 Aug 2016 16:53:02 GMT
RUN set -ex 	&& cd /usr/local/etc 	&& if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi 	&& { 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf 	&& { 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = [::]:9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 30 Aug 2016 16:53:03 GMT
EXPOSE 9000/tcp
# Tue, 30 Aug 2016 16:53:03 GMT
CMD ["php-fpm"]
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
	-	`sha256:ebcd06baa62f74a2676adb6f965a0f6b8450881acaae9f6581f58768f7ee4377`  
		Last Modified: Wed, 07 Sep 2016 19:00:58 GMT  
		Size: 12.5 MB (12493491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b17051912e37da71b4defc89cea92a8001e4ed077e458a922d5030e31fabd0`  
		Last Modified: Wed, 07 Sep 2016 19:00:54 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5790c4dd7db41b11b6bbc7af091310fb1bea6ac839cd7409562852d0fb4377bc`  
		Last Modified: Wed, 07 Sep 2016 19:01:01 GMT  
		Size: 14.8 MB (14815087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89df7e4318a7a73affcf391fea766a4d2e5eba7d0435dc51a289833817e4c755`  
		Last Modified: Wed, 07 Sep 2016 19:00:54 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bf6857178825dc26ff589c0d0bab28f19a6f580efca859ab6724e55c5ccd86`  
		Last Modified: Wed, 07 Sep 2016 19:00:54 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253d6f307afc1ae36ddc8e748e2ce6d504213a848fc98b0ccc30e745b7e9b915`  
		Last Modified: Wed, 07 Sep 2016 19:00:54 GMT  
		Size: 7.7 KB (7678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip