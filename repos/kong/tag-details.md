<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kong`

-	[`kong:0.9`](#kong09)
-	[`kong:0.9.4`](#kong094)
-	[`kong:latest`](#konglatest)

## `kong:0.9`

```console
$ docker pull kong@sha256:3c973a9cffd47e222498cf74bbe3704e266ae38d9b555d62f35c7f7bf002a1b2
```

-	Platforms:
	-	linux; amd64

### `kong:0.9` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121919117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fded5f135fc67625cd5f04baa834677d6371d38ee5142263d4ec6a9c39cfe7c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","start"]`

```dockerfile
# Tue, 30 Aug 2016 18:18:45 GMT
MAINTAINER https://github.com/CentOS/sig-cloud-instance-images
# Wed, 02 Nov 2016 19:52:05 GMT
ADD file:54df3580ac9fb66389b09230a74115a49ace2d193603bce0b5786dcb2957eb52 in / 
# Wed, 02 Nov 2016 19:52:08 GMT
LABEL name=CentOS Base Image vendor=CentOS license=GPLv2 build-date=20161102
# Wed, 02 Nov 2016 19:52:09 GMT
CMD ["/bin/bash"]
# Wed, 02 Nov 2016 20:11:05 GMT
MAINTAINER Marco Palladino, marco@mashape.com
# Thu, 03 Nov 2016 16:45:18 GMT
ENV KONG_VERSION=0.9.4
# Thu, 03 Nov 2016 16:45:43 GMT
RUN yum install -y wget https://github.com/Mashape/kong/releases/download/$KONG_VERSION/kong-$KONG_VERSION.el7.noarch.rpm &&     yum clean all
# Thu, 03 Nov 2016 16:45:46 GMT
RUN wget -O /usr/local/bin/dumb-init https://github.com/Yelp/dumb-init/releases/download/v1.1.3/dumb-init_1.1.3_amd64 &&     chmod +x /usr/local/bin/dumb-init
# Thu, 03 Nov 2016 16:45:47 GMT
COPY file:324f2e5f56829733b3c3c8b6971998202fa01bf7368caac6c1971fcec0464e8c in /docker-entrypoint.sh 
# Thu, 03 Nov 2016 16:45:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 03 Nov 2016 16:45:49 GMT
EXPOSE 7946/tcp 8000/tcp 8001/tcp 8443/tcp
# Thu, 03 Nov 2016 16:45:50 GMT
CMD ["kong" "start"]
```

-	Layers:
	-	`sha256:08d48e6f1cff259389732d35307bb877215fa28867cdaff50c1dbd6e0b993c1f`  
		Last Modified: Wed, 02 Nov 2016 19:52:49 GMT  
		Size: 70.5 MB (70481699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455e533a1d9d7eed6d2832d831d9015ea2d7a6d5dde59d2de0dd2e3834353b1f`  
		Last Modified: Thu, 03 Nov 2016 16:46:08 GMT  
		Size: 51.4 MB (51412532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d26f813abc21d3f5f6aa7f600146d915301ede9c4e3a92020aafa3c63c57e24`  
		Last Modified: Thu, 03 Nov 2016 16:45:55 GMT  
		Size: 24.6 KB (24648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1742f077492358bb5d11d5434ef284df712aec69b38affb5aef2fbc27b4d9740`  
		Last Modified: Thu, 03 Nov 2016 16:45:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:0.9.4`

```console
$ docker pull kong@sha256:3c973a9cffd47e222498cf74bbe3704e266ae38d9b555d62f35c7f7bf002a1b2
```

-	Platforms:
	-	linux; amd64

### `kong:0.9.4` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121919117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fded5f135fc67625cd5f04baa834677d6371d38ee5142263d4ec6a9c39cfe7c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","start"]`

```dockerfile
# Tue, 30 Aug 2016 18:18:45 GMT
MAINTAINER https://github.com/CentOS/sig-cloud-instance-images
# Wed, 02 Nov 2016 19:52:05 GMT
ADD file:54df3580ac9fb66389b09230a74115a49ace2d193603bce0b5786dcb2957eb52 in / 
# Wed, 02 Nov 2016 19:52:08 GMT
LABEL name=CentOS Base Image vendor=CentOS license=GPLv2 build-date=20161102
# Wed, 02 Nov 2016 19:52:09 GMT
CMD ["/bin/bash"]
# Wed, 02 Nov 2016 20:11:05 GMT
MAINTAINER Marco Palladino, marco@mashape.com
# Thu, 03 Nov 2016 16:45:18 GMT
ENV KONG_VERSION=0.9.4
# Thu, 03 Nov 2016 16:45:43 GMT
RUN yum install -y wget https://github.com/Mashape/kong/releases/download/$KONG_VERSION/kong-$KONG_VERSION.el7.noarch.rpm &&     yum clean all
# Thu, 03 Nov 2016 16:45:46 GMT
RUN wget -O /usr/local/bin/dumb-init https://github.com/Yelp/dumb-init/releases/download/v1.1.3/dumb-init_1.1.3_amd64 &&     chmod +x /usr/local/bin/dumb-init
# Thu, 03 Nov 2016 16:45:47 GMT
COPY file:324f2e5f56829733b3c3c8b6971998202fa01bf7368caac6c1971fcec0464e8c in /docker-entrypoint.sh 
# Thu, 03 Nov 2016 16:45:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 03 Nov 2016 16:45:49 GMT
EXPOSE 7946/tcp 8000/tcp 8001/tcp 8443/tcp
# Thu, 03 Nov 2016 16:45:50 GMT
CMD ["kong" "start"]
```

-	Layers:
	-	`sha256:08d48e6f1cff259389732d35307bb877215fa28867cdaff50c1dbd6e0b993c1f`  
		Last Modified: Wed, 02 Nov 2016 19:52:49 GMT  
		Size: 70.5 MB (70481699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455e533a1d9d7eed6d2832d831d9015ea2d7a6d5dde59d2de0dd2e3834353b1f`  
		Last Modified: Thu, 03 Nov 2016 16:46:08 GMT  
		Size: 51.4 MB (51412532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d26f813abc21d3f5f6aa7f600146d915301ede9c4e3a92020aafa3c63c57e24`  
		Last Modified: Thu, 03 Nov 2016 16:45:55 GMT  
		Size: 24.6 KB (24648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1742f077492358bb5d11d5434ef284df712aec69b38affb5aef2fbc27b4d9740`  
		Last Modified: Thu, 03 Nov 2016 16:45:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:3c973a9cffd47e222498cf74bbe3704e266ae38d9b555d62f35c7f7bf002a1b2
```

-	Platforms:
	-	linux; amd64

### `kong:latest` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121919117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fded5f135fc67625cd5f04baa834677d6371d38ee5142263d4ec6a9c39cfe7c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","start"]`

```dockerfile
# Tue, 30 Aug 2016 18:18:45 GMT
MAINTAINER https://github.com/CentOS/sig-cloud-instance-images
# Wed, 02 Nov 2016 19:52:05 GMT
ADD file:54df3580ac9fb66389b09230a74115a49ace2d193603bce0b5786dcb2957eb52 in / 
# Wed, 02 Nov 2016 19:52:08 GMT
LABEL name=CentOS Base Image vendor=CentOS license=GPLv2 build-date=20161102
# Wed, 02 Nov 2016 19:52:09 GMT
CMD ["/bin/bash"]
# Wed, 02 Nov 2016 20:11:05 GMT
MAINTAINER Marco Palladino, marco@mashape.com
# Thu, 03 Nov 2016 16:45:18 GMT
ENV KONG_VERSION=0.9.4
# Thu, 03 Nov 2016 16:45:43 GMT
RUN yum install -y wget https://github.com/Mashape/kong/releases/download/$KONG_VERSION/kong-$KONG_VERSION.el7.noarch.rpm &&     yum clean all
# Thu, 03 Nov 2016 16:45:46 GMT
RUN wget -O /usr/local/bin/dumb-init https://github.com/Yelp/dumb-init/releases/download/v1.1.3/dumb-init_1.1.3_amd64 &&     chmod +x /usr/local/bin/dumb-init
# Thu, 03 Nov 2016 16:45:47 GMT
COPY file:324f2e5f56829733b3c3c8b6971998202fa01bf7368caac6c1971fcec0464e8c in /docker-entrypoint.sh 
# Thu, 03 Nov 2016 16:45:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 03 Nov 2016 16:45:49 GMT
EXPOSE 7946/tcp 8000/tcp 8001/tcp 8443/tcp
# Thu, 03 Nov 2016 16:45:50 GMT
CMD ["kong" "start"]
```

-	Layers:
	-	`sha256:08d48e6f1cff259389732d35307bb877215fa28867cdaff50c1dbd6e0b993c1f`  
		Last Modified: Wed, 02 Nov 2016 19:52:49 GMT  
		Size: 70.5 MB (70481699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455e533a1d9d7eed6d2832d831d9015ea2d7a6d5dde59d2de0dd2e3834353b1f`  
		Last Modified: Thu, 03 Nov 2016 16:46:08 GMT  
		Size: 51.4 MB (51412532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d26f813abc21d3f5f6aa7f600146d915301ede9c4e3a92020aafa3c63c57e24`  
		Last Modified: Thu, 03 Nov 2016 16:45:55 GMT  
		Size: 24.6 KB (24648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1742f077492358bb5d11d5434ef284df712aec69b38affb5aef2fbc27b4d9740`  
		Last Modified: Thu, 03 Nov 2016 16:45:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
