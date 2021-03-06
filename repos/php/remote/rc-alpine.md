## `php:rc-alpine`

```console
$ docker pull php@sha256:fbaf4972ccfbfdd6035c5d08a287916394497f2a8798f0b6eb6ea6807d20a625
```

-	Platforms:
	-	linux; amd64

### `php:rc-alpine` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.2 MB (28187772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982b6b48517c1f7a12c15416fecebfc74b8255542d88440ea4ffc5d8667915a6`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 21:17:33 GMT
ENV PHPIZE_DEPS=autoconf 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 18 Oct 2016 21:17:35 GMT
RUN apk add --no-cache --virtual .persistent-deps 		ca-certificates 		curl 		tar 		xz
# Tue, 18 Oct 2016 21:17:36 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Tue, 18 Oct 2016 21:17:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 18 Oct 2016 21:17:37 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Tue, 18 Oct 2016 21:17:37 GMT
ENV GPG_KEYS=A917B1ECDA84AEC2B568FED6F50ABC807BD5DCD0
# Mon, 31 Oct 2016 22:30:32 GMT
ENV PHP_VERSION=7.1.0RC5
# Mon, 31 Oct 2016 22:30:33 GMT
ENV PHP_URL=http://downloads.php.net/~krakjoe/php-7.1.0RC5.tar.xz PHP_ASC_URL=
# Mon, 31 Oct 2016 22:30:33 GMT
ENV PHP_SHA256=55a1b47cfa090760bb26438eb4faa7c62cd16eca4e527759e3941b38941f8f14 PHP_MD5=1d195b0aeb63914a308fb215671445a5
# Mon, 31 Oct 2016 22:30:39 GMT
RUN set -xe; 		apk add --no-cache --virtual .fetch-deps 		gnupg 		openssl 	; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -r "$GNUPGHOME"; 	fi; 		apk del .fetch-deps
# Mon, 31 Oct 2016 22:30:40 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Mon, 31 Oct 2016 22:34:43 GMT
RUN set -xe 	&& apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		curl-dev 		libedit-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 		&& docker-php-source extract 	&& cd /usr/src/php 	&& ./configure 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(getconf _NPROCESSORS_ONLN)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& docker-php-source delete 		&& runDeps="$( 		scanelf --needed --nobanner --recursive /usr/local 			| awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }' 			| sort -u 			| xargs -r apk info --installed 			| sort -u 	)" 	&& apk add --no-cache --virtual .php-rundeps $runDeps 		&& apk del .build-deps
# Mon, 31 Oct 2016 22:34:44 GMT
COPY multi:ed54b4fe7bef284934703fa6e979b7cc0daed0549a07586d0c1ccd4e2b41884a in /usr/local/bin/ 
# Mon, 31 Oct 2016 22:34:44 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67654b7bd8a6f817e849f77cd102331617f4e2394feeae4f77f8683b9b466ed9`  
		Last Modified: Tue, 18 Oct 2016 22:37:25 GMT  
		Size: 1.0 MB (1048149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c453327105c5d394a206069893aa1527b7cc4e58699b4a4b0c2453f5b02a7f`  
		Last Modified: Tue, 18 Oct 2016 22:37:23 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481e68959c15a56029b84021fca8cce378aaa0aa08837e08878bbddc694e798c`  
		Last Modified: Tue, 18 Oct 2016 22:37:22 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1622d88f1aa66c6cf2b2f64238dc8c85fce9c90d653ef9036618b096f0d6bfde`  
		Last Modified: Mon, 31 Oct 2016 22:56:40 GMT  
		Size: 12.9 MB (12873109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4486866d609e13b105711d2e3e905f2e14399b6d089b0b26c5eeac73c38c067e`  
		Last Modified: Mon, 31 Oct 2016 22:56:38 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d712e58262fb6f46dc75fcd739dff6d7e4a1273169cebe04c013fc6863b64da`  
		Last Modified: Mon, 31 Oct 2016 22:56:42 GMT  
		Size: 11.9 MB (11949811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970e2cc9a9c437d2b623fb3b2ecd8295146732a43292a8cd832cc256a67a5b2e`  
		Last Modified: Mon, 31 Oct 2016 22:56:38 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
