## `php-zendserver:latest`

```console
$ docker pull php-zendserver@sha256:b9c96440fb0d414fea26e2b784f4bc0d97c33cc4d0a626f405c456b31b7ac5fa
```

-	Platforms:
	-	linux; amd64

### `php-zendserver:latest` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **379.0 MB (379033307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ca4b6438bfa452bd6636511e59ba7b2c613d08c21c5b356079e05d054a0135`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Thu, 13 Oct 2016 21:13:01 GMT
ADD file:bc2e0eb31424a88aadc42486b6762c321e3457527daa43bcad45819d38c3a2ed in / 
# Thu, 13 Oct 2016 21:13:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 13 Oct 2016 21:13:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 13 Oct 2016 21:13:04 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Thu, 13 Oct 2016 21:13:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 13 Oct 2016 21:13:06 GMT
CMD ["/bin/bash"]
# Thu, 13 Oct 2016 23:17:48 GMT
RUN apt-key adv --keyserver pgp.mit.edu --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Thu, 13 Oct 2016 23:29:25 GMT
RUN echo "deb http://repos.zend.com/zend-server/9.0/deb_apache2.4 server non-free" >> /etc/apt/sources.list.d/zend-server.list
# Thu, 13 Oct 2016 23:32:12 GMT
RUN apt-get update && apt-get install -y libmysqlclient18 unzip git zend-server-php-7.0 && /usr/local/zend/bin/zendctl.sh stop
# Thu, 13 Oct 2016 23:32:14 GMT
COPY file:7ead1fa52a84d592d3f6402f7ec6a593311aac6f7d31aaed200d310d67f34d54 in /etc/ 
# Thu, 13 Oct 2016 23:32:14 GMT
COPY file:82de006e31874ac4e03685b3e87e988446f42138aaaf0fc5faad9cddb48040ba in /etc/apache2/conf-available 
# Thu, 13 Oct 2016 23:32:15 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Thu, 13 Oct 2016 23:32:21 GMT
RUN /usr/sbin/a2enmod headers
# Thu, 13 Oct 2016 23:32:21 GMT
ENV ZS_INIT_VERSION=0.2
# Thu, 13 Oct 2016 23:32:21 GMT
ENV ZS_INIT_SHA256=1c5cf557daf48cf018dba1cf46208f215d3b5fab47c73ff2d39988581ebd6932
# Thu, 13 Oct 2016 23:32:25 GMT
RUN apt-get install -y curl
# Thu, 13 Oct 2016 23:32:25 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Thu, 13 Oct 2016 23:32:26 GMT
WORKDIR /usr/local/zs-init
# Thu, 13 Oct 2016 23:32:31 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php
# Thu, 13 Oct 2016 23:33:28 GMT
RUN /usr/local/zend/bin/php composer.phar update
# Thu, 13 Oct 2016 23:33:29 GMT
COPY dir:6174d7fdcd8142a1b143e80efd2994e57dd5d7610a8fbfee3a7288ddf495dfdf in /usr/local/bin 
# Thu, 13 Oct 2016 23:33:30 GMT
COPY dir:b14dbc48195e4d5367d3aea2ed0fb26985bacb8d8229d24961363db2e2edf8f0 in /usr/local/zend/var/plugins/ 
# Thu, 13 Oct 2016 23:33:31 GMT
RUN rm /var/www/html/index.html
# Thu, 13 Oct 2016 23:33:31 GMT
COPY dir:9f1a7f23dfcf85f3c7148d98ae7914654fe8acfc4e4651f3a08427c09af24198 in /var/www/html 
# Thu, 13 Oct 2016 23:33:31 GMT
EXPOSE 80/tcp
# Thu, 13 Oct 2016 23:33:32 GMT
EXPOSE 443/tcp
# Thu, 13 Oct 2016 23:33:37 GMT
EXPOSE 10081/tcp
# Thu, 13 Oct 2016 23:33:37 GMT
EXPOSE 10082/tcp
# Thu, 13 Oct 2016 23:33:38 GMT
WORKDIR /var/www/html
# Thu, 13 Oct 2016 23:33:38 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:bf5d463153227eaf2c0a3d3f479bb5f2357f060fbce8088e61b2329d3d312d0c`  
		Last Modified: Thu, 13 Oct 2016 21:14:45 GMT  
		Size: 65.7 MB (65703010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f13e0ac480c2c862ae7aca8536bf2250b4d410468e6d33dc2f8ade1d368e184`  
		Last Modified: Thu, 13 Oct 2016 21:14:23 GMT  
		Size: 71.5 KB (71550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8988b5b3097ba5b9f10f45cd3545adea8b70bf9779f987d5b99cca08be818c3`  
		Last Modified: Thu, 13 Oct 2016 21:14:22 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40af181810e71ae2b871c81aed2bc990d2748f0e11adedda056f12cb4af08712`  
		Last Modified: Thu, 13 Oct 2016 21:14:23 GMT  
		Size: 678.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f7c7e5c03ef6687a44551a4675336e6500f5379f4cc7e5b14b20ac05f127c4`  
		Last Modified: Thu, 13 Oct 2016 21:14:22 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4704ff743b7b8d1fa799ccb9210eb2a9693855f627cf73cc127a71b1ba8d38e8`  
		Last Modified: Thu, 13 Oct 2016 23:22:13 GMT  
		Size: 13.1 KB (13057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df78834fd912bc60cec1fb25904de729e574ce1f7f06b73001114aa8bfd46ff`  
		Last Modified: Thu, 13 Oct 2016 23:33:53 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b15d2ceb50fca01be7497e7e1fdec8f2e4458957324f511868c026ce885032`  
		Last Modified: Thu, 13 Oct 2016 23:35:09 GMT  
		Size: 303.0 MB (303025537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b0bde511e13c8e012e8a077f9e8802e0830161629c25437950eef134114440`  
		Last Modified: Thu, 13 Oct 2016 23:33:53 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126f5f07b13600e599840f6fe3430e853f1be0b95b810cffe676e087b54abfb8`  
		Last Modified: Thu, 13 Oct 2016 23:33:52 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f45b10ae9cfedcc97852a32aebc17f3aed6566dedcb3aa163491f438e22496`  
		Last Modified: Thu, 13 Oct 2016 23:33:51 GMT  
		Size: 301.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342f1846ed9a15d561f1e42530b7cffeae705db68aa77be7e7f587873caa5361`  
		Last Modified: Thu, 13 Oct 2016 23:33:51 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e894df8d0ee342bb3cabc217d06d4dd8c285ac5aa590f6b7a85a3d68d65426`  
		Last Modified: Thu, 13 Oct 2016 23:33:50 GMT  
		Size: 467.0 KB (467030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d845ebec75d990744af13f583500d1290a42a758a9caeac6a724d456eeaeaeed`  
		Last Modified: Thu, 13 Oct 2016 23:33:49 GMT  
		Size: 15.6 KB (15590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f558aae1403b2ab32f4722e0d744e18f7e8f8f0e803a21047cb033afe5ba7d76`  
		Last Modified: Thu, 13 Oct 2016 23:33:49 GMT  
		Size: 457.0 KB (456963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df2b191eae5a74b6a20436fd1441b3ad1be3e679b0e126dc5b62f891b4361f8`  
		Last Modified: Thu, 13 Oct 2016 23:33:49 GMT  
		Size: 9.3 MB (9261071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5e218e226face279de34a488015ae480960c26331a033a8564265ba69c3b28`  
		Last Modified: Thu, 13 Oct 2016 23:33:46 GMT  
		Size: 13.1 KB (13102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a84b323275c6fc4f3ce89ac5ed05e268424dd02da3162e5265dc9c0af25a8e9`  
		Last Modified: Thu, 13 Oct 2016 23:33:46 GMT  
		Size: 2.5 KB (2501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7134b047da7407b25a12404d292d7b035fc5dfe8d84f0503aae682abb6cf7261`  
		Last Modified: Thu, 13 Oct 2016 23:33:46 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542509262a698a77b09701d6b19042675a102a0bcf41170da8c36b72e641600d`  
		Last Modified: Thu, 13 Oct 2016 23:33:46 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
