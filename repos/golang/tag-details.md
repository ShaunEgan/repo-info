<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `golang`

-	[`golang:1.6.3`](#golang163)
-	[`golang:1.6`](#golang16)
-	[`golang:1.6.3-onbuild`](#golang163-onbuild)
-	[`golang:1.6-onbuild`](#golang16-onbuild)
-	[`golang:1.6.3-wheezy`](#golang163-wheezy)
-	[`golang:1.6-wheezy`](#golang16-wheezy)
-	[`golang:1.6.3-alpine`](#golang163-alpine)
-	[`golang:1.6-alpine`](#golang16-alpine)
-	[`golang:1.6.3-windowsservercore`](#golang163-windowsservercore)
-	[`golang:1.6-windowsservercore`](#golang16-windowsservercore)
-	[`golang:1.6.3-nanoserver`](#golang163-nanoserver)
-	[`golang:1.6-nanoserver`](#golang16-nanoserver)
-	[`golang:1.7.3`](#golang173)
-	[`golang:1.7`](#golang17)
-	[`golang:1`](#golang1)
-	[`golang:latest`](#golanglatest)
-	[`golang:1.7.3-onbuild`](#golang173-onbuild)
-	[`golang:1.7-onbuild`](#golang17-onbuild)
-	[`golang:1-onbuild`](#golang1-onbuild)
-	[`golang:onbuild`](#golangonbuild)
-	[`golang:1.7.3-wheezy`](#golang173-wheezy)
-	[`golang:1.7-wheezy`](#golang17-wheezy)
-	[`golang:1-wheezy`](#golang1-wheezy)
-	[`golang:wheezy`](#golangwheezy)
-	[`golang:1.7.3-alpine`](#golang173-alpine)
-	[`golang:1.7-alpine`](#golang17-alpine)
-	[`golang:1-alpine`](#golang1-alpine)
-	[`golang:alpine`](#golangalpine)
-	[`golang:1.7.3-windowsservercore`](#golang173-windowsservercore)
-	[`golang:1.7-windowsservercore`](#golang17-windowsservercore)
-	[`golang:1-windowsservercore`](#golang1-windowsservercore)
-	[`golang:windowsservercore`](#golangwindowsservercore)
-	[`golang:1.7.3-nanoserver`](#golang173-nanoserver)
-	[`golang:1.7-nanoserver`](#golang17-nanoserver)
-	[`golang:1-nanoserver`](#golang1-nanoserver)
-	[`golang:nanoserver`](#golangnanoserver)

## `golang:1.6.3`

```console
$ docker pull golang@sha256:f5cf85d6bdf90d812bbd3b31bef1428871abec6e7e02860c626389aeb41fa0b9
```

-	Platforms:
	-	linux; amd64

### `golang:1.6.3` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.9 MB (256904360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b0a30b21a1503747270124b15d95a86e81178ed876c18d6a220159d48486d98`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:41:25 GMT
ENV GOLANG_VERSION=1.6.3
# Fri, 21 Oct 2016 19:41:25 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:41:26 GMT
ENV GOLANG_DOWNLOAD_SHA256=cdde5e08530c0579255d6153b08fdb3b8e47caabbe717bc7bcd7561275a87aeb
# Fri, 21 Oct 2016 19:41:36 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:41:37 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:41:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:41:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:41:38 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:41:39 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
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
	-	`sha256:25ffd5f08b9d0c29dc200ae6f4c5adc48838bef9b27b80f4620de526719d4a16`  
		Last Modified: Fri, 21 Oct 2016 19:38:00 GMT  
		Size: 59.7 MB (59651478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0063428f95efd4f9501781b28b20301a5021711936af7e15626b7a921c05b02`  
		Last Modified: Fri, 21 Oct 2016 19:42:14 GMT  
		Size: 84.9 MB (84869331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b34e92966775837f54381c00aa2134a556f808d5d945c55392197abce7978e0`  
		Last Modified: Fri, 21 Oct 2016 19:41:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4830fc52ed16a1fa51b545ab81c9b217d16d4f6900d177c0364858aa96623374`  
		Last Modified: Fri, 21 Oct 2016 19:41:49 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6`

```console
$ docker pull golang@sha256:f5cf85d6bdf90d812bbd3b31bef1428871abec6e7e02860c626389aeb41fa0b9
```

-	Platforms:
	-	linux; amd64

### `golang:1.6` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.9 MB (256904360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b0a30b21a1503747270124b15d95a86e81178ed876c18d6a220159d48486d98`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:41:25 GMT
ENV GOLANG_VERSION=1.6.3
# Fri, 21 Oct 2016 19:41:25 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:41:26 GMT
ENV GOLANG_DOWNLOAD_SHA256=cdde5e08530c0579255d6153b08fdb3b8e47caabbe717bc7bcd7561275a87aeb
# Fri, 21 Oct 2016 19:41:36 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:41:37 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:41:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:41:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:41:38 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:41:39 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
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
	-	`sha256:25ffd5f08b9d0c29dc200ae6f4c5adc48838bef9b27b80f4620de526719d4a16`  
		Last Modified: Fri, 21 Oct 2016 19:38:00 GMT  
		Size: 59.7 MB (59651478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0063428f95efd4f9501781b28b20301a5021711936af7e15626b7a921c05b02`  
		Last Modified: Fri, 21 Oct 2016 19:42:14 GMT  
		Size: 84.9 MB (84869331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b34e92966775837f54381c00aa2134a556f808d5d945c55392197abce7978e0`  
		Last Modified: Fri, 21 Oct 2016 19:41:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4830fc52ed16a1fa51b545ab81c9b217d16d4f6900d177c0364858aa96623374`  
		Last Modified: Fri, 21 Oct 2016 19:41:49 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6.3-onbuild`

```console
$ docker pull golang@sha256:83b1e7f04bbc2527034d5a3e89b259aafd116226af139fe347ebf3c19b19c906
```

-	Platforms:
	-	linux; amd64

### `golang:1.6.3-onbuild` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.9 MB (256904493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5005615cfb189ca68fe29bdc1ce189c727213d02b245e2e9c4903f54f7b9a0`
-	Default Command: `["go-wrapper","run"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:41:25 GMT
ENV GOLANG_VERSION=1.6.3
# Fri, 21 Oct 2016 19:41:25 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:41:26 GMT
ENV GOLANG_DOWNLOAD_SHA256=cdde5e08530c0579255d6153b08fdb3b8e47caabbe717bc7bcd7561275a87aeb
# Fri, 21 Oct 2016 19:41:36 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:41:37 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:41:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:41:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:41:38 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:41:39 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
# Fri, 21 Oct 2016 19:42:34 GMT
RUN mkdir -p /go/src/app
# Fri, 21 Oct 2016 19:42:34 GMT
WORKDIR /go/src/app
# Fri, 21 Oct 2016 19:42:34 GMT
CMD ["go-wrapper" "run"]
# Fri, 21 Oct 2016 19:42:35 GMT
ONBUILD COPY . /go/src/app
# Fri, 21 Oct 2016 19:42:35 GMT
ONBUILD RUN go-wrapper download
# Fri, 21 Oct 2016 19:42:35 GMT
ONBUILD RUN go-wrapper install
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
	-	`sha256:25ffd5f08b9d0c29dc200ae6f4c5adc48838bef9b27b80f4620de526719d4a16`  
		Last Modified: Fri, 21 Oct 2016 19:38:00 GMT  
		Size: 59.7 MB (59651478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0063428f95efd4f9501781b28b20301a5021711936af7e15626b7a921c05b02`  
		Last Modified: Fri, 21 Oct 2016 19:42:14 GMT  
		Size: 84.9 MB (84869331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b34e92966775837f54381c00aa2134a556f808d5d945c55392197abce7978e0`  
		Last Modified: Fri, 21 Oct 2016 19:41:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4830fc52ed16a1fa51b545ab81c9b217d16d4f6900d177c0364858aa96623374`  
		Last Modified: Fri, 21 Oct 2016 19:41:49 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9af1638a66d55ffe5494b538e2128765305488dcaf503873251c3894e7c7bc`  
		Last Modified: Fri, 21 Oct 2016 19:42:45 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6-onbuild`

```console
$ docker pull golang@sha256:83b1e7f04bbc2527034d5a3e89b259aafd116226af139fe347ebf3c19b19c906
```

-	Platforms:
	-	linux; amd64

### `golang:1.6-onbuild` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.9 MB (256904493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5005615cfb189ca68fe29bdc1ce189c727213d02b245e2e9c4903f54f7b9a0`
-	Default Command: `["go-wrapper","run"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:41:25 GMT
ENV GOLANG_VERSION=1.6.3
# Fri, 21 Oct 2016 19:41:25 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:41:26 GMT
ENV GOLANG_DOWNLOAD_SHA256=cdde5e08530c0579255d6153b08fdb3b8e47caabbe717bc7bcd7561275a87aeb
# Fri, 21 Oct 2016 19:41:36 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:41:37 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:41:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:41:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:41:38 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:41:39 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
# Fri, 21 Oct 2016 19:42:34 GMT
RUN mkdir -p /go/src/app
# Fri, 21 Oct 2016 19:42:34 GMT
WORKDIR /go/src/app
# Fri, 21 Oct 2016 19:42:34 GMT
CMD ["go-wrapper" "run"]
# Fri, 21 Oct 2016 19:42:35 GMT
ONBUILD COPY . /go/src/app
# Fri, 21 Oct 2016 19:42:35 GMT
ONBUILD RUN go-wrapper download
# Fri, 21 Oct 2016 19:42:35 GMT
ONBUILD RUN go-wrapper install
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
	-	`sha256:25ffd5f08b9d0c29dc200ae6f4c5adc48838bef9b27b80f4620de526719d4a16`  
		Last Modified: Fri, 21 Oct 2016 19:38:00 GMT  
		Size: 59.7 MB (59651478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0063428f95efd4f9501781b28b20301a5021711936af7e15626b7a921c05b02`  
		Last Modified: Fri, 21 Oct 2016 19:42:14 GMT  
		Size: 84.9 MB (84869331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b34e92966775837f54381c00aa2134a556f808d5d945c55392197abce7978e0`  
		Last Modified: Fri, 21 Oct 2016 19:41:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4830fc52ed16a1fa51b545ab81c9b217d16d4f6900d177c0364858aa96623374`  
		Last Modified: Fri, 21 Oct 2016 19:41:49 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9af1638a66d55ffe5494b538e2128765305488dcaf503873251c3894e7c7bc`  
		Last Modified: Fri, 21 Oct 2016 19:42:45 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6.3-wheezy`

```console
$ docker pull golang@sha256:31b7169d8c3b7e23a8d990d6fd61555792122f0eb061a82a33cc905a08589125
```

-	Platforms:
	-	linux; amd64

### `golang:1.6.3-wheezy` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202646858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:270fc65d747481bd4ab73759e78fdf6946227aece33ad797c85a028a58546f9f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2016 16:26:06 GMT
ADD file:93883f863ccd9e401e4f945206887f251075a63d25a8129c9bd73e707397f109 in / 
# Fri, 21 Oct 2016 16:26:06 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:38:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:43:06 GMT
ENV GOLANG_VERSION=1.6.3
# Fri, 21 Oct 2016 19:43:06 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:43:07 GMT
ENV GOLANG_DOWNLOAD_SHA256=cdde5e08530c0579255d6153b08fdb3b8e47caabbe717bc7bcd7561275a87aeb
# Fri, 21 Oct 2016 19:43:17 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:43:17 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:43:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:43:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:43:19 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:43:20 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
```

-	Layers:
	-	`sha256:d44a3b2e3fc2a79a071282b2ad5f6bcbefc929c0e816750b0b76f6ec5580ae23`  
		Last Modified: Fri, 21 Oct 2016 16:26:27 GMT  
		Size: 37.2 MB (37215139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5089ed91d3c0db1d6aaf79fbdf9593e28c1ea9bdabfab75dfb1b5fc1fcdf05a`  
		Last Modified: Fri, 21 Oct 2016 16:38:41 GMT  
		Size: 6.7 MB (6748520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cdd795dcc65ffd51af821a9dc9542376781af0feeb7e66d11fc5aaad7abdd`  
		Last Modified: Fri, 21 Oct 2016 16:39:37 GMT  
		Size: 37.4 MB (37366571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec030508dc3da4f5ec84d2187a65f569d53f21122e7dbdf491ba2f336e354eaf`  
		Last Modified: Fri, 21 Oct 2016 19:40:31 GMT  
		Size: 36.4 MB (36445852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee92dda245767f72dbe81e1097690489fc7b8d6b6302d8a8977e051351e0dda`  
		Last Modified: Fri, 21 Oct 2016 19:43:57 GMT  
		Size: 84.9 MB (84869299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73b75534775d13740f58a8e2c4aeecb2e0c7d7fe9947d3edb4d948de93080d3`  
		Last Modified: Fri, 21 Oct 2016 19:43:29 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f440e8a0320cccff9789318c4e4e0bf625d89495f5f6c30e3626ae74581e9556`  
		Last Modified: Fri, 21 Oct 2016 19:43:29 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6-wheezy`

```console
$ docker pull golang@sha256:31b7169d8c3b7e23a8d990d6fd61555792122f0eb061a82a33cc905a08589125
```

-	Platforms:
	-	linux; amd64

### `golang:1.6-wheezy` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202646858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:270fc65d747481bd4ab73759e78fdf6946227aece33ad797c85a028a58546f9f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2016 16:26:06 GMT
ADD file:93883f863ccd9e401e4f945206887f251075a63d25a8129c9bd73e707397f109 in / 
# Fri, 21 Oct 2016 16:26:06 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:38:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:43:06 GMT
ENV GOLANG_VERSION=1.6.3
# Fri, 21 Oct 2016 19:43:06 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:43:07 GMT
ENV GOLANG_DOWNLOAD_SHA256=cdde5e08530c0579255d6153b08fdb3b8e47caabbe717bc7bcd7561275a87aeb
# Fri, 21 Oct 2016 19:43:17 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:43:17 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:43:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:43:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:43:19 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:43:20 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
```

-	Layers:
	-	`sha256:d44a3b2e3fc2a79a071282b2ad5f6bcbefc929c0e816750b0b76f6ec5580ae23`  
		Last Modified: Fri, 21 Oct 2016 16:26:27 GMT  
		Size: 37.2 MB (37215139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5089ed91d3c0db1d6aaf79fbdf9593e28c1ea9bdabfab75dfb1b5fc1fcdf05a`  
		Last Modified: Fri, 21 Oct 2016 16:38:41 GMT  
		Size: 6.7 MB (6748520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cdd795dcc65ffd51af821a9dc9542376781af0feeb7e66d11fc5aaad7abdd`  
		Last Modified: Fri, 21 Oct 2016 16:39:37 GMT  
		Size: 37.4 MB (37366571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec030508dc3da4f5ec84d2187a65f569d53f21122e7dbdf491ba2f336e354eaf`  
		Last Modified: Fri, 21 Oct 2016 19:40:31 GMT  
		Size: 36.4 MB (36445852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee92dda245767f72dbe81e1097690489fc7b8d6b6302d8a8977e051351e0dda`  
		Last Modified: Fri, 21 Oct 2016 19:43:57 GMT  
		Size: 84.9 MB (84869299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73b75534775d13740f58a8e2c4aeecb2e0c7d7fe9947d3edb4d948de93080d3`  
		Last Modified: Fri, 21 Oct 2016 19:43:29 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f440e8a0320cccff9789318c4e4e0bf625d89495f5f6c30e3626ae74581e9556`  
		Last Modified: Fri, 21 Oct 2016 19:43:29 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6.3-alpine`

```console
$ docker pull golang@sha256:6654d7df76000e3fa23576fd94890a72392fbb1302594e5e2d0a0a1bff169c7c
```

-	Platforms:
	-	linux; amd64

### `golang:1.6.3-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.2 MB (72158797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c6e04805d43a3ea0c4ae3e46ed3175822283361179268fa2e58a2b4dfe098f2`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:32:36 GMT
RUN apk add --no-cache ca-certificates
# Tue, 18 Oct 2016 20:32:37 GMT
ENV GOLANG_VERSION=1.6.3
# Tue, 18 Oct 2016 20:32:37 GMT
ENV GOLANG_SRC_URL=https://golang.org/dl/go1.6.3.src.tar.gz
# Tue, 18 Oct 2016 20:32:37 GMT
ENV GOLANG_SRC_SHA256=6326aeed5f86cf18f16d6dc831405614f855e2d416a91fd3fdc334f772345b00
# Tue, 18 Oct 2016 20:32:38 GMT
COPY file:b2d7156cdbff1193fb20efaf40b201017b0396eb5b2e0adb97970615a8fcf61d in / 
# Tue, 18 Oct 2016 20:33:35 GMT
RUN set -ex 	&& apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 		&& export GOROOT_BOOTSTRAP="$(go env GOROOT)" 		&& wget -q "$GOLANG_SRC_URL" -O golang.tar.gz 	&& echo "$GOLANG_SRC_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz 	&& cd /usr/local/go/src 	&& patch -p2 -i /no-pic.patch 	&& ./make.bash 		&& rm -rf /*.patch 	&& apk del .build-deps
# Tue, 18 Oct 2016 20:33:36 GMT
ENV GOPATH=/go
# Tue, 18 Oct 2016 20:33:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Oct 2016 20:33:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 18 Oct 2016 20:33:38 GMT
WORKDIR /go
# Tue, 18 Oct 2016 20:33:38 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c311f66f3ac9a1d4b9fdfa8ac09821993c24d540e6147d25793c861c67892238`  
		Last Modified: Tue, 18 Oct 2016 20:36:01 GMT  
		Size: 344.0 KB (343962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7c11c7fbb68625242a12dd161fe825347cde21917e5ed9feae84792d90b6dd`  
		Last Modified: Tue, 18 Oct 2016 20:35:59 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d123bc0e4b561e6fec451e56764dd48a13599a1bc3a66a27741d0c2ed1550e`  
		Last Modified: Tue, 18 Oct 2016 20:36:24 GMT  
		Size: 69.5 MB (69499961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ee23b97f8a2a9c8f70397c6cf05270e2788b62ec5b26559c17241e6bbd2a5c`  
		Last Modified: Tue, 18 Oct 2016 20:35:59 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afe9bae2e86ba899889998b31a9ec3bdbad097a02bcfcbd01b0c5e070b8a9e3`  
		Last Modified: Tue, 18 Oct 2016 20:35:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6-alpine`

```console
$ docker pull golang@sha256:6654d7df76000e3fa23576fd94890a72392fbb1302594e5e2d0a0a1bff169c7c
```

-	Platforms:
	-	linux; amd64

### `golang:1.6-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.2 MB (72158797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c6e04805d43a3ea0c4ae3e46ed3175822283361179268fa2e58a2b4dfe098f2`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:32:36 GMT
RUN apk add --no-cache ca-certificates
# Tue, 18 Oct 2016 20:32:37 GMT
ENV GOLANG_VERSION=1.6.3
# Tue, 18 Oct 2016 20:32:37 GMT
ENV GOLANG_SRC_URL=https://golang.org/dl/go1.6.3.src.tar.gz
# Tue, 18 Oct 2016 20:32:37 GMT
ENV GOLANG_SRC_SHA256=6326aeed5f86cf18f16d6dc831405614f855e2d416a91fd3fdc334f772345b00
# Tue, 18 Oct 2016 20:32:38 GMT
COPY file:b2d7156cdbff1193fb20efaf40b201017b0396eb5b2e0adb97970615a8fcf61d in / 
# Tue, 18 Oct 2016 20:33:35 GMT
RUN set -ex 	&& apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 		&& export GOROOT_BOOTSTRAP="$(go env GOROOT)" 		&& wget -q "$GOLANG_SRC_URL" -O golang.tar.gz 	&& echo "$GOLANG_SRC_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz 	&& cd /usr/local/go/src 	&& patch -p2 -i /no-pic.patch 	&& ./make.bash 		&& rm -rf /*.patch 	&& apk del .build-deps
# Tue, 18 Oct 2016 20:33:36 GMT
ENV GOPATH=/go
# Tue, 18 Oct 2016 20:33:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Oct 2016 20:33:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 18 Oct 2016 20:33:38 GMT
WORKDIR /go
# Tue, 18 Oct 2016 20:33:38 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c311f66f3ac9a1d4b9fdfa8ac09821993c24d540e6147d25793c861c67892238`  
		Last Modified: Tue, 18 Oct 2016 20:36:01 GMT  
		Size: 344.0 KB (343962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7c11c7fbb68625242a12dd161fe825347cde21917e5ed9feae84792d90b6dd`  
		Last Modified: Tue, 18 Oct 2016 20:35:59 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d123bc0e4b561e6fec451e56764dd48a13599a1bc3a66a27741d0c2ed1550e`  
		Last Modified: Tue, 18 Oct 2016 20:36:24 GMT  
		Size: 69.5 MB (69499961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ee23b97f8a2a9c8f70397c6cf05270e2788b62ec5b26559c17241e6bbd2a5c`  
		Last Modified: Tue, 18 Oct 2016 20:35:59 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afe9bae2e86ba899889998b31a9ec3bdbad097a02bcfcbd01b0c5e070b8a9e3`  
		Last Modified: Tue, 18 Oct 2016 20:35:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6.3-windowsservercore`

```console
$ docker pull golang@sha256:131b11505a2fa0b1cf37e67abf0b6c37364fd1b3110ff40ab7088dfcdb41fc5f
```

-	Platforms:
	-	windows; amd64

### `golang:1.6.3-windowsservercore` - windows; amd64

-	Docker Version: 1.12.2-cs2-ws-beta
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 GB (4667925412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6f55de8f8daf70483eecc616298ac5d347f5663b2f2c7b0f303e7cfbd69b48`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Wed, 12 Oct 2016 19:25:22 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Oct 2016 19:25:27 GMT
ENV GIT_VERSION=2.9.2
# Wed, 12 Oct 2016 19:25:32 GMT
ENV GIT_TAG=v2.9.2.windows.1
# Wed, 12 Oct 2016 19:25:35 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.9.2.windows.1/Git-2.9.2-64-bit.exe
# Wed, 12 Oct 2016 19:25:39 GMT
ENV GIT_DOWNLOAD_SHA256=006d971bcbe73cc8d841a100a4eb20d22e135142bf5b0f2120722fd420e166e5
# Tue, 18 Oct 2016 20:43:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.exe -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-Wait 		-FilePath ./git.exe 		-ArgumentList @( 			'/VERYSILENT', 			'/NORESTART', 			'/NOCANCEL', 			'/SP-', 			'/SUPPRESSMSGBOXES', 						'/COMPONENTS=assoc_sh', 						'/DIR=C:\git' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\bin;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 	Write-Host '  bash --version'; bash --version; 	Write-Host '  curl --version'; curl.exe --version; 		Write-Host 'Removing installer ...'; 	Remove-Item git.exe -Force; 		Write-Host 'Complete.';
# Tue, 18 Oct 2016 20:43:13 GMT
ENV GOPATH=C:\gopath
# Tue, 18 Oct 2016 20:43:34 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 18 Oct 2016 20:43:37 GMT
ENV GOLANG_VERSION=1.6.3
# Tue, 18 Oct 2016 20:43:39 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.windows-amd64.zip
# Tue, 18 Oct 2016 20:43:42 GMT
ENV GOLANG_DOWNLOAD_SHA256=6a18e5ed8b39785338986aecc6a3f36f5c4be286ff52db0ae3bcd2275ab70df0
# Tue, 18 Oct 2016 20:47:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GOLANG_DOWNLOAD_URL -OutFile 'go.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Tue, 18 Oct 2016 20:47:51 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:9c7f9c7d9bc2915388ecc5d08e89a7583658285469d7325281f95d8ee279cc60`  
		Size: 3.7 GB (3737824348 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:de5064718b3f2749727c8b5ffddf2da7698189277afe0df6fc0a57ad573bca0f`  
		Size: 613.1 MB (613059969 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ce8c033b9d9ab0f42b7bc1457fc9094bbf37079117ad712092b3e48f11a6e218`  
		Last Modified: Wed, 12 Oct 2016 19:49:17 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac669cb897e39ec11f318c297f4d37f4fcee666f73329a87d682d483650eb81`  
		Last Modified: Wed, 12 Oct 2016 20:12:47 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637e390ccc606ceb43ffe429ad2eba95a67bbe497de0ac9394d09faee98cb647`  
		Last Modified: Wed, 12 Oct 2016 20:12:47 GMT  
		Size: 1.2 KB (1222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e960bb9bf7ba980b3a5aa3bbbe2e43cbbbbb8bb179e56609a2325db86aab69f`  
		Last Modified: Wed, 12 Oct 2016 20:12:46 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c43be2eca6ba8658363340237b0999be111d6e4b4e76e8bf42f801737692de4`  
		Last Modified: Wed, 12 Oct 2016 20:12:43 GMT  
		Size: 1.2 KB (1205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e0e4bf1429e0a8e00029f128ffac0b63d9f984ce3733deb814d188e3a505ea`  
		Last Modified: Tue, 18 Oct 2016 21:03:28 GMT  
		Size: 215.4 MB (215353361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0185773a0a17452f7ec01e4963e4d512f4831e3a40e9bb1258b9081dec9c4934`  
		Last Modified: Tue, 18 Oct 2016 21:01:48 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a07a6f6ea11b197fcf5338624e85603ff44b33e9a7d1f0aa5c6da047ad5133`  
		Last Modified: Tue, 18 Oct 2016 21:01:51 GMT  
		Size: 4.3 MB (4331070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9c3b20ded01430ff6cedd6880acbdd4b668cb6de3e9938783eb0c800be3bb1`  
		Last Modified: Tue, 18 Oct 2016 21:01:42 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47eb60a503f1648d5cf7fb3123f7e3fbc042cf1e5dab7d5d29290edd2ada73ee`  
		Last Modified: Tue, 18 Oct 2016 21:01:43 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da9f3df809dd196c7953176ffd1bbbd47055c4bc3655b559a12d48c61347e80`  
		Last Modified: Tue, 18 Oct 2016 21:01:42 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddaff25b53b01c9464071defcefbc69f4e7285f120c4b8877c51f1645431307`  
		Last Modified: Tue, 18 Oct 2016 21:03:08 GMT  
		Size: 97.3 MB (97344534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8f09523adac39246acc2d3e302996397ee19c67f035ca19e2183026d08b5e8`  
		Last Modified: Tue, 18 Oct 2016 21:01:42 GMT  
		Size: 1.2 KB (1217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6-windowsservercore`

```console
$ docker pull golang@sha256:131b11505a2fa0b1cf37e67abf0b6c37364fd1b3110ff40ab7088dfcdb41fc5f
```

-	Platforms:
	-	windows; amd64

### `golang:1.6-windowsservercore` - windows; amd64

-	Docker Version: 1.12.2-cs2-ws-beta
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 GB (4667925412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6f55de8f8daf70483eecc616298ac5d347f5663b2f2c7b0f303e7cfbd69b48`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Wed, 12 Oct 2016 19:25:22 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Oct 2016 19:25:27 GMT
ENV GIT_VERSION=2.9.2
# Wed, 12 Oct 2016 19:25:32 GMT
ENV GIT_TAG=v2.9.2.windows.1
# Wed, 12 Oct 2016 19:25:35 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.9.2.windows.1/Git-2.9.2-64-bit.exe
# Wed, 12 Oct 2016 19:25:39 GMT
ENV GIT_DOWNLOAD_SHA256=006d971bcbe73cc8d841a100a4eb20d22e135142bf5b0f2120722fd420e166e5
# Tue, 18 Oct 2016 20:43:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.exe -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-Wait 		-FilePath ./git.exe 		-ArgumentList @( 			'/VERYSILENT', 			'/NORESTART', 			'/NOCANCEL', 			'/SP-', 			'/SUPPRESSMSGBOXES', 						'/COMPONENTS=assoc_sh', 						'/DIR=C:\git' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\bin;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 	Write-Host '  bash --version'; bash --version; 	Write-Host '  curl --version'; curl.exe --version; 		Write-Host 'Removing installer ...'; 	Remove-Item git.exe -Force; 		Write-Host 'Complete.';
# Tue, 18 Oct 2016 20:43:13 GMT
ENV GOPATH=C:\gopath
# Tue, 18 Oct 2016 20:43:34 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 18 Oct 2016 20:43:37 GMT
ENV GOLANG_VERSION=1.6.3
# Tue, 18 Oct 2016 20:43:39 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.windows-amd64.zip
# Tue, 18 Oct 2016 20:43:42 GMT
ENV GOLANG_DOWNLOAD_SHA256=6a18e5ed8b39785338986aecc6a3f36f5c4be286ff52db0ae3bcd2275ab70df0
# Tue, 18 Oct 2016 20:47:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GOLANG_DOWNLOAD_URL -OutFile 'go.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Tue, 18 Oct 2016 20:47:51 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:9c7f9c7d9bc2915388ecc5d08e89a7583658285469d7325281f95d8ee279cc60`  
		Size: 3.7 GB (3737824348 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:de5064718b3f2749727c8b5ffddf2da7698189277afe0df6fc0a57ad573bca0f`  
		Size: 613.1 MB (613059969 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ce8c033b9d9ab0f42b7bc1457fc9094bbf37079117ad712092b3e48f11a6e218`  
		Last Modified: Wed, 12 Oct 2016 19:49:17 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac669cb897e39ec11f318c297f4d37f4fcee666f73329a87d682d483650eb81`  
		Last Modified: Wed, 12 Oct 2016 20:12:47 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637e390ccc606ceb43ffe429ad2eba95a67bbe497de0ac9394d09faee98cb647`  
		Last Modified: Wed, 12 Oct 2016 20:12:47 GMT  
		Size: 1.2 KB (1222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e960bb9bf7ba980b3a5aa3bbbe2e43cbbbbb8bb179e56609a2325db86aab69f`  
		Last Modified: Wed, 12 Oct 2016 20:12:46 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c43be2eca6ba8658363340237b0999be111d6e4b4e76e8bf42f801737692de4`  
		Last Modified: Wed, 12 Oct 2016 20:12:43 GMT  
		Size: 1.2 KB (1205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e0e4bf1429e0a8e00029f128ffac0b63d9f984ce3733deb814d188e3a505ea`  
		Last Modified: Tue, 18 Oct 2016 21:03:28 GMT  
		Size: 215.4 MB (215353361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0185773a0a17452f7ec01e4963e4d512f4831e3a40e9bb1258b9081dec9c4934`  
		Last Modified: Tue, 18 Oct 2016 21:01:48 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a07a6f6ea11b197fcf5338624e85603ff44b33e9a7d1f0aa5c6da047ad5133`  
		Last Modified: Tue, 18 Oct 2016 21:01:51 GMT  
		Size: 4.3 MB (4331070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9c3b20ded01430ff6cedd6880acbdd4b668cb6de3e9938783eb0c800be3bb1`  
		Last Modified: Tue, 18 Oct 2016 21:01:42 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47eb60a503f1648d5cf7fb3123f7e3fbc042cf1e5dab7d5d29290edd2ada73ee`  
		Last Modified: Tue, 18 Oct 2016 21:01:43 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da9f3df809dd196c7953176ffd1bbbd47055c4bc3655b559a12d48c61347e80`  
		Last Modified: Tue, 18 Oct 2016 21:01:42 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddaff25b53b01c9464071defcefbc69f4e7285f120c4b8877c51f1645431307`  
		Last Modified: Tue, 18 Oct 2016 21:03:08 GMT  
		Size: 97.3 MB (97344534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8f09523adac39246acc2d3e302996397ee19c67f035ca19e2183026d08b5e8`  
		Last Modified: Tue, 18 Oct 2016 21:01:42 GMT  
		Size: 1.2 KB (1217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6.3-nanoserver`

```console
$ docker pull golang@sha256:7d468eff87ed3ca4f61d455b4607d5645c4a606ec770a297161250a2541bec64
```

-	Platforms:
	-	windows; amd64

### `golang:1.6.3-nanoserver` - windows; amd64

-	Docker Version: 1.12.2-cs2-ws-beta
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.1 MB (393060169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c0f2c5a0c0942f9cdbfcd1041cafc945ea5a20419b9f19e195cd35253ba8ec`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 18 Oct 2016 20:47:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 18 Oct 2016 20:48:00 GMT
ENV GOPATH=C:\gopath
# Tue, 18 Oct 2016 20:48:30 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath;
# Tue, 18 Oct 2016 20:48:33 GMT
ENV GOLANG_VERSION=1.6.3
# Tue, 18 Oct 2016 20:48:35 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.windows-amd64.zip
# Tue, 18 Oct 2016 20:48:37 GMT
ENV GOLANG_DOWNLOAD_SHA256=6a18e5ed8b39785338986aecc6a3f36f5c4be286ff52db0ae3bcd2275ab70df0
# Tue, 18 Oct 2016 20:52:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GOLANG_DOWNLOAD_URL -OutFile 'go.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Tue, 18 Oct 2016 20:52:42 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:5496abde368a3dd39999745bf998c877ddc6a390a943bc3fd99ffaabf728ed88`  
		Size: 242.6 MB (242646586 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:94b4ce7ac4c7c7d4ed75ac2bd9359a87204ad2d5a909759d8e77953874d8e7c2`  
		Size: 56.4 MB (56434068 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12ba288c0d1d424b4832b58c8d542b2b1cc0c8ed873e0f4805a83f705f351eb7`  
		Last Modified: Tue, 18 Oct 2016 21:03:45 GMT  
		Size: 954.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aabf8dca125e29a1422adc206ada519107e390cdc61e481410b7fe3f75538b`  
		Last Modified: Tue, 18 Oct 2016 21:03:45 GMT  
		Size: 962.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3844df32288b9b5de39acf93cc8fd2e0d5662b9b8cefc58c9d5382fc2b6d16d0`  
		Last Modified: Tue, 18 Oct 2016 21:03:46 GMT  
		Size: 819.6 KB (819629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f087fa7aaa8af52a77dbdb8f40e3d5b9b022368e23ec7034840c69fce08a53d`  
		Last Modified: Tue, 18 Oct 2016 21:03:41 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ca7b76e833956562d5c324f880d2a13e19886b6cfcb092e7e97954bd62dddd`  
		Last Modified: Tue, 18 Oct 2016 21:03:42 GMT  
		Size: 963.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe10e4bc2be84557cef02cefd9db0d6eef489831726869477bfeb11f203270`  
		Last Modified: Tue, 18 Oct 2016 21:03:40 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1351e87f31ebdb04a3978a60076d1f762f49a14ba25abd51de233f6a3cc7d11c`  
		Last Modified: Tue, 18 Oct 2016 21:04:26 GMT  
		Size: 93.2 MB (93154124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e256dff31d0d477f616053f2a462dac16a0d86ccf3a0f10dc7ce642b52b2260`  
		Last Modified: Tue, 18 Oct 2016 21:03:40 GMT  
		Size: 969.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6-nanoserver`

```console
$ docker pull golang@sha256:7d468eff87ed3ca4f61d455b4607d5645c4a606ec770a297161250a2541bec64
```

-	Platforms:
	-	windows; amd64

### `golang:1.6-nanoserver` - windows; amd64

-	Docker Version: 1.12.2-cs2-ws-beta
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.1 MB (393060169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c0f2c5a0c0942f9cdbfcd1041cafc945ea5a20419b9f19e195cd35253ba8ec`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 18 Oct 2016 20:47:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 18 Oct 2016 20:48:00 GMT
ENV GOPATH=C:\gopath
# Tue, 18 Oct 2016 20:48:30 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath;
# Tue, 18 Oct 2016 20:48:33 GMT
ENV GOLANG_VERSION=1.6.3
# Tue, 18 Oct 2016 20:48:35 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.windows-amd64.zip
# Tue, 18 Oct 2016 20:48:37 GMT
ENV GOLANG_DOWNLOAD_SHA256=6a18e5ed8b39785338986aecc6a3f36f5c4be286ff52db0ae3bcd2275ab70df0
# Tue, 18 Oct 2016 20:52:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GOLANG_DOWNLOAD_URL -OutFile 'go.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Tue, 18 Oct 2016 20:52:42 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:5496abde368a3dd39999745bf998c877ddc6a390a943bc3fd99ffaabf728ed88`  
		Size: 242.6 MB (242646586 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:94b4ce7ac4c7c7d4ed75ac2bd9359a87204ad2d5a909759d8e77953874d8e7c2`  
		Size: 56.4 MB (56434068 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12ba288c0d1d424b4832b58c8d542b2b1cc0c8ed873e0f4805a83f705f351eb7`  
		Last Modified: Tue, 18 Oct 2016 21:03:45 GMT  
		Size: 954.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aabf8dca125e29a1422adc206ada519107e390cdc61e481410b7fe3f75538b`  
		Last Modified: Tue, 18 Oct 2016 21:03:45 GMT  
		Size: 962.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3844df32288b9b5de39acf93cc8fd2e0d5662b9b8cefc58c9d5382fc2b6d16d0`  
		Last Modified: Tue, 18 Oct 2016 21:03:46 GMT  
		Size: 819.6 KB (819629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f087fa7aaa8af52a77dbdb8f40e3d5b9b022368e23ec7034840c69fce08a53d`  
		Last Modified: Tue, 18 Oct 2016 21:03:41 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ca7b76e833956562d5c324f880d2a13e19886b6cfcb092e7e97954bd62dddd`  
		Last Modified: Tue, 18 Oct 2016 21:03:42 GMT  
		Size: 963.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe10e4bc2be84557cef02cefd9db0d6eef489831726869477bfeb11f203270`  
		Last Modified: Tue, 18 Oct 2016 21:03:40 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1351e87f31ebdb04a3978a60076d1f762f49a14ba25abd51de233f6a3cc7d11c`  
		Last Modified: Tue, 18 Oct 2016 21:04:26 GMT  
		Size: 93.2 MB (93154124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e256dff31d0d477f616053f2a462dac16a0d86ccf3a0f10dc7ce642b52b2260`  
		Last Modified: Tue, 18 Oct 2016 21:03:40 GMT  
		Size: 969.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7.3`

```console
$ docker pull golang@sha256:dcde4549a6bff65a921c4dc7d3e4ebe8b6c698cf71a0c1045f0011370f7ed9b9
```

-	Platforms:
	-	linux; amd64

### `golang:1.7.3` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.7 MB (253667784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f69c27b2f59a8bb999623f4f7bf426596f82c74da522910c96e52b42a80d9360`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_VERSION=1.7.3
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:37:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=508028aac0654e993564b6e2014bf2d4a9751e3b286661b0b0040046cf18028e
# Fri, 21 Oct 2016 19:37:32 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:37:33 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:37:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:37:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:37:34 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:37:35 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
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
	-	`sha256:25ffd5f08b9d0c29dc200ae6f4c5adc48838bef9b27b80f4620de526719d4a16`  
		Last Modified: Fri, 21 Oct 2016 19:38:00 GMT  
		Size: 59.7 MB (59651478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d869811918905f9737bf4634f234d8d86be8ed6d31d2f3cada9eb7b412d4a30d`  
		Last Modified: Fri, 21 Oct 2016 19:38:11 GMT  
		Size: 81.6 MB (81632761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34cb59feb7bc276d20da5cd3f6c941a8d26974c224cfbd11d923038950d0aff`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb527c679d40028610f89d7225500b6bfb106de36a3e83521889a723da02fd3a`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7`

```console
$ docker pull golang@sha256:dcde4549a6bff65a921c4dc7d3e4ebe8b6c698cf71a0c1045f0011370f7ed9b9
```

-	Platforms:
	-	linux; amd64

### `golang:1.7` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.7 MB (253667784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f69c27b2f59a8bb999623f4f7bf426596f82c74da522910c96e52b42a80d9360`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_VERSION=1.7.3
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:37:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=508028aac0654e993564b6e2014bf2d4a9751e3b286661b0b0040046cf18028e
# Fri, 21 Oct 2016 19:37:32 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:37:33 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:37:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:37:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:37:34 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:37:35 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
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
	-	`sha256:25ffd5f08b9d0c29dc200ae6f4c5adc48838bef9b27b80f4620de526719d4a16`  
		Last Modified: Fri, 21 Oct 2016 19:38:00 GMT  
		Size: 59.7 MB (59651478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d869811918905f9737bf4634f234d8d86be8ed6d31d2f3cada9eb7b412d4a30d`  
		Last Modified: Fri, 21 Oct 2016 19:38:11 GMT  
		Size: 81.6 MB (81632761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34cb59feb7bc276d20da5cd3f6c941a8d26974c224cfbd11d923038950d0aff`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb527c679d40028610f89d7225500b6bfb106de36a3e83521889a723da02fd3a`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1`

```console
$ docker pull golang@sha256:dcde4549a6bff65a921c4dc7d3e4ebe8b6c698cf71a0c1045f0011370f7ed9b9
```

-	Platforms:
	-	linux; amd64

### `golang:1` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.7 MB (253667784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f69c27b2f59a8bb999623f4f7bf426596f82c74da522910c96e52b42a80d9360`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_VERSION=1.7.3
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:37:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=508028aac0654e993564b6e2014bf2d4a9751e3b286661b0b0040046cf18028e
# Fri, 21 Oct 2016 19:37:32 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:37:33 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:37:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:37:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:37:34 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:37:35 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
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
	-	`sha256:25ffd5f08b9d0c29dc200ae6f4c5adc48838bef9b27b80f4620de526719d4a16`  
		Last Modified: Fri, 21 Oct 2016 19:38:00 GMT  
		Size: 59.7 MB (59651478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d869811918905f9737bf4634f234d8d86be8ed6d31d2f3cada9eb7b412d4a30d`  
		Last Modified: Fri, 21 Oct 2016 19:38:11 GMT  
		Size: 81.6 MB (81632761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34cb59feb7bc276d20da5cd3f6c941a8d26974c224cfbd11d923038950d0aff`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb527c679d40028610f89d7225500b6bfb106de36a3e83521889a723da02fd3a`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:latest`

```console
$ docker pull golang@sha256:dcde4549a6bff65a921c4dc7d3e4ebe8b6c698cf71a0c1045f0011370f7ed9b9
```

-	Platforms:
	-	linux; amd64

### `golang:latest` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.7 MB (253667784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f69c27b2f59a8bb999623f4f7bf426596f82c74da522910c96e52b42a80d9360`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_VERSION=1.7.3
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:37:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=508028aac0654e993564b6e2014bf2d4a9751e3b286661b0b0040046cf18028e
# Fri, 21 Oct 2016 19:37:32 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:37:33 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:37:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:37:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:37:34 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:37:35 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
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
	-	`sha256:25ffd5f08b9d0c29dc200ae6f4c5adc48838bef9b27b80f4620de526719d4a16`  
		Last Modified: Fri, 21 Oct 2016 19:38:00 GMT  
		Size: 59.7 MB (59651478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d869811918905f9737bf4634f234d8d86be8ed6d31d2f3cada9eb7b412d4a30d`  
		Last Modified: Fri, 21 Oct 2016 19:38:11 GMT  
		Size: 81.6 MB (81632761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34cb59feb7bc276d20da5cd3f6c941a8d26974c224cfbd11d923038950d0aff`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb527c679d40028610f89d7225500b6bfb106de36a3e83521889a723da02fd3a`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7.3-onbuild`

```console
$ docker pull golang@sha256:ab4324504842d107d0254d0d5eddf44dbacd529193f81c67edc9f81c8fb7e1bd
```

-	Platforms:
	-	linux; amd64

### `golang:1.7.3-onbuild` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.7 MB (253667916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1391d767c35edbbb44c0827990dc28b2982c05cb349eaabb20caa618be96d777`
-	Default Command: `["go-wrapper","run"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_VERSION=1.7.3
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:37:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=508028aac0654e993564b6e2014bf2d4a9751e3b286661b0b0040046cf18028e
# Fri, 21 Oct 2016 19:37:32 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:37:33 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:37:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:37:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:37:34 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:37:35 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
# Fri, 21 Oct 2016 19:38:55 GMT
RUN mkdir -p /go/src/app
# Fri, 21 Oct 2016 19:38:56 GMT
WORKDIR /go/src/app
# Fri, 21 Oct 2016 19:38:56 GMT
CMD ["go-wrapper" "run"]
# Fri, 21 Oct 2016 19:38:56 GMT
ONBUILD COPY . /go/src/app
# Fri, 21 Oct 2016 19:38:57 GMT
ONBUILD RUN go-wrapper download
# Fri, 21 Oct 2016 19:38:57 GMT
ONBUILD RUN go-wrapper install
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
	-	`sha256:25ffd5f08b9d0c29dc200ae6f4c5adc48838bef9b27b80f4620de526719d4a16`  
		Last Modified: Fri, 21 Oct 2016 19:38:00 GMT  
		Size: 59.7 MB (59651478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d869811918905f9737bf4634f234d8d86be8ed6d31d2f3cada9eb7b412d4a30d`  
		Last Modified: Fri, 21 Oct 2016 19:38:11 GMT  
		Size: 81.6 MB (81632761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34cb59feb7bc276d20da5cd3f6c941a8d26974c224cfbd11d923038950d0aff`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb527c679d40028610f89d7225500b6bfb106de36a3e83521889a723da02fd3a`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07ead829cc2f7d25f8179ff30bff8146efdc62901896235dea4a6c7da1150e0`  
		Last Modified: Fri, 21 Oct 2016 19:39:06 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7-onbuild`

```console
$ docker pull golang@sha256:ab4324504842d107d0254d0d5eddf44dbacd529193f81c67edc9f81c8fb7e1bd
```

-	Platforms:
	-	linux; amd64

### `golang:1.7-onbuild` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.7 MB (253667916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1391d767c35edbbb44c0827990dc28b2982c05cb349eaabb20caa618be96d777`
-	Default Command: `["go-wrapper","run"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_VERSION=1.7.3
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:37:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=508028aac0654e993564b6e2014bf2d4a9751e3b286661b0b0040046cf18028e
# Fri, 21 Oct 2016 19:37:32 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:37:33 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:37:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:37:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:37:34 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:37:35 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
# Fri, 21 Oct 2016 19:38:55 GMT
RUN mkdir -p /go/src/app
# Fri, 21 Oct 2016 19:38:56 GMT
WORKDIR /go/src/app
# Fri, 21 Oct 2016 19:38:56 GMT
CMD ["go-wrapper" "run"]
# Fri, 21 Oct 2016 19:38:56 GMT
ONBUILD COPY . /go/src/app
# Fri, 21 Oct 2016 19:38:57 GMT
ONBUILD RUN go-wrapper download
# Fri, 21 Oct 2016 19:38:57 GMT
ONBUILD RUN go-wrapper install
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
	-	`sha256:25ffd5f08b9d0c29dc200ae6f4c5adc48838bef9b27b80f4620de526719d4a16`  
		Last Modified: Fri, 21 Oct 2016 19:38:00 GMT  
		Size: 59.7 MB (59651478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d869811918905f9737bf4634f234d8d86be8ed6d31d2f3cada9eb7b412d4a30d`  
		Last Modified: Fri, 21 Oct 2016 19:38:11 GMT  
		Size: 81.6 MB (81632761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34cb59feb7bc276d20da5cd3f6c941a8d26974c224cfbd11d923038950d0aff`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb527c679d40028610f89d7225500b6bfb106de36a3e83521889a723da02fd3a`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07ead829cc2f7d25f8179ff30bff8146efdc62901896235dea4a6c7da1150e0`  
		Last Modified: Fri, 21 Oct 2016 19:39:06 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-onbuild`

```console
$ docker pull golang@sha256:ab4324504842d107d0254d0d5eddf44dbacd529193f81c67edc9f81c8fb7e1bd
```

-	Platforms:
	-	linux; amd64

### `golang:1-onbuild` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.7 MB (253667916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1391d767c35edbbb44c0827990dc28b2982c05cb349eaabb20caa618be96d777`
-	Default Command: `["go-wrapper","run"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_VERSION=1.7.3
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:37:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=508028aac0654e993564b6e2014bf2d4a9751e3b286661b0b0040046cf18028e
# Fri, 21 Oct 2016 19:37:32 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:37:33 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:37:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:37:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:37:34 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:37:35 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
# Fri, 21 Oct 2016 19:38:55 GMT
RUN mkdir -p /go/src/app
# Fri, 21 Oct 2016 19:38:56 GMT
WORKDIR /go/src/app
# Fri, 21 Oct 2016 19:38:56 GMT
CMD ["go-wrapper" "run"]
# Fri, 21 Oct 2016 19:38:56 GMT
ONBUILD COPY . /go/src/app
# Fri, 21 Oct 2016 19:38:57 GMT
ONBUILD RUN go-wrapper download
# Fri, 21 Oct 2016 19:38:57 GMT
ONBUILD RUN go-wrapper install
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
	-	`sha256:25ffd5f08b9d0c29dc200ae6f4c5adc48838bef9b27b80f4620de526719d4a16`  
		Last Modified: Fri, 21 Oct 2016 19:38:00 GMT  
		Size: 59.7 MB (59651478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d869811918905f9737bf4634f234d8d86be8ed6d31d2f3cada9eb7b412d4a30d`  
		Last Modified: Fri, 21 Oct 2016 19:38:11 GMT  
		Size: 81.6 MB (81632761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34cb59feb7bc276d20da5cd3f6c941a8d26974c224cfbd11d923038950d0aff`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb527c679d40028610f89d7225500b6bfb106de36a3e83521889a723da02fd3a`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07ead829cc2f7d25f8179ff30bff8146efdc62901896235dea4a6c7da1150e0`  
		Last Modified: Fri, 21 Oct 2016 19:39:06 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:onbuild`

```console
$ docker pull golang@sha256:ab4324504842d107d0254d0d5eddf44dbacd529193f81c67edc9f81c8fb7e1bd
```

-	Platforms:
	-	linux; amd64

### `golang:onbuild` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.7 MB (253667916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1391d767c35edbbb44c0827990dc28b2982c05cb349eaabb20caa618be96d777`
-	Default Command: `["go-wrapper","run"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_VERSION=1.7.3
# Fri, 21 Oct 2016 19:37:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:37:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=508028aac0654e993564b6e2014bf2d4a9751e3b286661b0b0040046cf18028e
# Fri, 21 Oct 2016 19:37:32 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:37:33 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:37:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:37:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:37:34 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:37:35 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
# Fri, 21 Oct 2016 19:38:55 GMT
RUN mkdir -p /go/src/app
# Fri, 21 Oct 2016 19:38:56 GMT
WORKDIR /go/src/app
# Fri, 21 Oct 2016 19:38:56 GMT
CMD ["go-wrapper" "run"]
# Fri, 21 Oct 2016 19:38:56 GMT
ONBUILD COPY . /go/src/app
# Fri, 21 Oct 2016 19:38:57 GMT
ONBUILD RUN go-wrapper download
# Fri, 21 Oct 2016 19:38:57 GMT
ONBUILD RUN go-wrapper install
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
	-	`sha256:25ffd5f08b9d0c29dc200ae6f4c5adc48838bef9b27b80f4620de526719d4a16`  
		Last Modified: Fri, 21 Oct 2016 19:38:00 GMT  
		Size: 59.7 MB (59651478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d869811918905f9737bf4634f234d8d86be8ed6d31d2f3cada9eb7b412d4a30d`  
		Last Modified: Fri, 21 Oct 2016 19:38:11 GMT  
		Size: 81.6 MB (81632761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34cb59feb7bc276d20da5cd3f6c941a8d26974c224cfbd11d923038950d0aff`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb527c679d40028610f89d7225500b6bfb106de36a3e83521889a723da02fd3a`  
		Last Modified: Fri, 21 Oct 2016 19:37:45 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07ead829cc2f7d25f8179ff30bff8146efdc62901896235dea4a6c7da1150e0`  
		Last Modified: Fri, 21 Oct 2016 19:39:06 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7.3-wheezy`

```console
$ docker pull golang@sha256:fc4401cc133fbfd258b4dcefa2f0d6e21eeba0c5e49890a00cd77a71e146b44d
```

-	Platforms:
	-	linux; amd64

### `golang:1.7.3-wheezy` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.4 MB (199410319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd5ad5cdf71869fbb307e6aae5fa315aa64c203014f4bc8df84f7c3a806783c4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2016 16:26:06 GMT
ADD file:93883f863ccd9e401e4f945206887f251075a63d25a8129c9bd73e707397f109 in / 
# Fri, 21 Oct 2016 16:26:06 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:38:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:39:58 GMT
ENV GOLANG_VERSION=1.7.3
# Fri, 21 Oct 2016 19:39:58 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:39:58 GMT
ENV GOLANG_DOWNLOAD_SHA256=508028aac0654e993564b6e2014bf2d4a9751e3b286661b0b0040046cf18028e
# Fri, 21 Oct 2016 19:40:07 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:40:07 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:40:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:40:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:40:09 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:40:09 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
```

-	Layers:
	-	`sha256:d44a3b2e3fc2a79a071282b2ad5f6bcbefc929c0e816750b0b76f6ec5580ae23`  
		Last Modified: Fri, 21 Oct 2016 16:26:27 GMT  
		Size: 37.2 MB (37215139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5089ed91d3c0db1d6aaf79fbdf9593e28c1ea9bdabfab75dfb1b5fc1fcdf05a`  
		Last Modified: Fri, 21 Oct 2016 16:38:41 GMT  
		Size: 6.7 MB (6748520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cdd795dcc65ffd51af821a9dc9542376781af0feeb7e66d11fc5aaad7abdd`  
		Last Modified: Fri, 21 Oct 2016 16:39:37 GMT  
		Size: 37.4 MB (37366571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec030508dc3da4f5ec84d2187a65f569d53f21122e7dbdf491ba2f336e354eaf`  
		Last Modified: Fri, 21 Oct 2016 19:40:31 GMT  
		Size: 36.4 MB (36445852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d527fc1d9a9572d7630082a41d2bf20337bf16ed5b7c1732832db3db1dbf27e3`  
		Last Modified: Fri, 21 Oct 2016 19:40:44 GMT  
		Size: 81.6 MB (81632761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8f111576daff2495188f0fcc02d43de4989cdd41246f1dfec106db2ffd41b0`  
		Last Modified: Fri, 21 Oct 2016 19:40:19 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4125fc9fbdfadac00d475a85d14d11a0288c29f84e541b5764e2005db103c82d`  
		Last Modified: Fri, 21 Oct 2016 19:40:19 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7-wheezy`

```console
$ docker pull golang@sha256:fc4401cc133fbfd258b4dcefa2f0d6e21eeba0c5e49890a00cd77a71e146b44d
```

-	Platforms:
	-	linux; amd64

### `golang:1.7-wheezy` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.4 MB (199410319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd5ad5cdf71869fbb307e6aae5fa315aa64c203014f4bc8df84f7c3a806783c4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2016 16:26:06 GMT
ADD file:93883f863ccd9e401e4f945206887f251075a63d25a8129c9bd73e707397f109 in / 
# Fri, 21 Oct 2016 16:26:06 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:38:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:39:58 GMT
ENV GOLANG_VERSION=1.7.3
# Fri, 21 Oct 2016 19:39:58 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:39:58 GMT
ENV GOLANG_DOWNLOAD_SHA256=508028aac0654e993564b6e2014bf2d4a9751e3b286661b0b0040046cf18028e
# Fri, 21 Oct 2016 19:40:07 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:40:07 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:40:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:40:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:40:09 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:40:09 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
```

-	Layers:
	-	`sha256:d44a3b2e3fc2a79a071282b2ad5f6bcbefc929c0e816750b0b76f6ec5580ae23`  
		Last Modified: Fri, 21 Oct 2016 16:26:27 GMT  
		Size: 37.2 MB (37215139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5089ed91d3c0db1d6aaf79fbdf9593e28c1ea9bdabfab75dfb1b5fc1fcdf05a`  
		Last Modified: Fri, 21 Oct 2016 16:38:41 GMT  
		Size: 6.7 MB (6748520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cdd795dcc65ffd51af821a9dc9542376781af0feeb7e66d11fc5aaad7abdd`  
		Last Modified: Fri, 21 Oct 2016 16:39:37 GMT  
		Size: 37.4 MB (37366571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec030508dc3da4f5ec84d2187a65f569d53f21122e7dbdf491ba2f336e354eaf`  
		Last Modified: Fri, 21 Oct 2016 19:40:31 GMT  
		Size: 36.4 MB (36445852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d527fc1d9a9572d7630082a41d2bf20337bf16ed5b7c1732832db3db1dbf27e3`  
		Last Modified: Fri, 21 Oct 2016 19:40:44 GMT  
		Size: 81.6 MB (81632761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8f111576daff2495188f0fcc02d43de4989cdd41246f1dfec106db2ffd41b0`  
		Last Modified: Fri, 21 Oct 2016 19:40:19 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4125fc9fbdfadac00d475a85d14d11a0288c29f84e541b5764e2005db103c82d`  
		Last Modified: Fri, 21 Oct 2016 19:40:19 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-wheezy`

```console
$ docker pull golang@sha256:fc4401cc133fbfd258b4dcefa2f0d6e21eeba0c5e49890a00cd77a71e146b44d
```

-	Platforms:
	-	linux; amd64

### `golang:1-wheezy` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.4 MB (199410319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd5ad5cdf71869fbb307e6aae5fa315aa64c203014f4bc8df84f7c3a806783c4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2016 16:26:06 GMT
ADD file:93883f863ccd9e401e4f945206887f251075a63d25a8129c9bd73e707397f109 in / 
# Fri, 21 Oct 2016 16:26:06 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:38:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:39:58 GMT
ENV GOLANG_VERSION=1.7.3
# Fri, 21 Oct 2016 19:39:58 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:39:58 GMT
ENV GOLANG_DOWNLOAD_SHA256=508028aac0654e993564b6e2014bf2d4a9751e3b286661b0b0040046cf18028e
# Fri, 21 Oct 2016 19:40:07 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:40:07 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:40:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:40:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:40:09 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:40:09 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
```

-	Layers:
	-	`sha256:d44a3b2e3fc2a79a071282b2ad5f6bcbefc929c0e816750b0b76f6ec5580ae23`  
		Last Modified: Fri, 21 Oct 2016 16:26:27 GMT  
		Size: 37.2 MB (37215139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5089ed91d3c0db1d6aaf79fbdf9593e28c1ea9bdabfab75dfb1b5fc1fcdf05a`  
		Last Modified: Fri, 21 Oct 2016 16:38:41 GMT  
		Size: 6.7 MB (6748520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cdd795dcc65ffd51af821a9dc9542376781af0feeb7e66d11fc5aaad7abdd`  
		Last Modified: Fri, 21 Oct 2016 16:39:37 GMT  
		Size: 37.4 MB (37366571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec030508dc3da4f5ec84d2187a65f569d53f21122e7dbdf491ba2f336e354eaf`  
		Last Modified: Fri, 21 Oct 2016 19:40:31 GMT  
		Size: 36.4 MB (36445852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d527fc1d9a9572d7630082a41d2bf20337bf16ed5b7c1732832db3db1dbf27e3`  
		Last Modified: Fri, 21 Oct 2016 19:40:44 GMT  
		Size: 81.6 MB (81632761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8f111576daff2495188f0fcc02d43de4989cdd41246f1dfec106db2ffd41b0`  
		Last Modified: Fri, 21 Oct 2016 19:40:19 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4125fc9fbdfadac00d475a85d14d11a0288c29f84e541b5764e2005db103c82d`  
		Last Modified: Fri, 21 Oct 2016 19:40:19 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:wheezy`

```console
$ docker pull golang@sha256:fc4401cc133fbfd258b4dcefa2f0d6e21eeba0c5e49890a00cd77a71e146b44d
```

-	Platforms:
	-	linux; amd64

### `golang:wheezy` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.4 MB (199410319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd5ad5cdf71869fbb307e6aae5fa315aa64c203014f4bc8df84f7c3a806783c4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2016 16:26:06 GMT
ADD file:93883f863ccd9e401e4f945206887f251075a63d25a8129c9bd73e707397f109 in / 
# Fri, 21 Oct 2016 16:26:06 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:38:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 16:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:39:58 GMT
ENV GOLANG_VERSION=1.7.3
# Fri, 21 Oct 2016 19:39:58 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.linux-amd64.tar.gz
# Fri, 21 Oct 2016 19:39:58 GMT
ENV GOLANG_DOWNLOAD_SHA256=508028aac0654e993564b6e2014bf2d4a9751e3b286661b0b0040046cf18028e
# Fri, 21 Oct 2016 19:40:07 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 21 Oct 2016 19:40:07 GMT
ENV GOPATH=/go
# Fri, 21 Oct 2016 19:40:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:40:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 21 Oct 2016 19:40:09 GMT
WORKDIR /go
# Fri, 21 Oct 2016 19:40:09 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
```

-	Layers:
	-	`sha256:d44a3b2e3fc2a79a071282b2ad5f6bcbefc929c0e816750b0b76f6ec5580ae23`  
		Last Modified: Fri, 21 Oct 2016 16:26:27 GMT  
		Size: 37.2 MB (37215139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5089ed91d3c0db1d6aaf79fbdf9593e28c1ea9bdabfab75dfb1b5fc1fcdf05a`  
		Last Modified: Fri, 21 Oct 2016 16:38:41 GMT  
		Size: 6.7 MB (6748520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cdd795dcc65ffd51af821a9dc9542376781af0feeb7e66d11fc5aaad7abdd`  
		Last Modified: Fri, 21 Oct 2016 16:39:37 GMT  
		Size: 37.4 MB (37366571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec030508dc3da4f5ec84d2187a65f569d53f21122e7dbdf491ba2f336e354eaf`  
		Last Modified: Fri, 21 Oct 2016 19:40:31 GMT  
		Size: 36.4 MB (36445852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d527fc1d9a9572d7630082a41d2bf20337bf16ed5b7c1732832db3db1dbf27e3`  
		Last Modified: Fri, 21 Oct 2016 19:40:44 GMT  
		Size: 81.6 MB (81632761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8f111576daff2495188f0fcc02d43de4989cdd41246f1dfec106db2ffd41b0`  
		Last Modified: Fri, 21 Oct 2016 19:40:19 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4125fc9fbdfadac00d475a85d14d11a0288c29f84e541b5764e2005db103c82d`  
		Last Modified: Fri, 21 Oct 2016 19:40:19 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7.3-alpine`

```console
$ docker pull golang@sha256:25ad25d8bece9d403be107b07c86fb6b2b588a5b26133baa9d1215c07bdbfa39
```

-	Platforms:
	-	linux; amd64

### `golang:1.7.3-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73275541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e874ba5240682d53411752d2186e74418a9d33d04238ef07b19e7a09db7eeda`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:32:36 GMT
RUN apk add --no-cache ca-certificates
# Wed, 19 Oct 2016 21:55:10 GMT
ENV GOLANG_VERSION=1.7.3
# Wed, 19 Oct 2016 21:55:10 GMT
ENV GOLANG_SRC_URL=https://golang.org/dl/go1.7.3.src.tar.gz
# Wed, 19 Oct 2016 21:55:11 GMT
ENV GOLANG_SRC_SHA256=79430a0027a09b0b3ad57e214c4c1acfdd7af290961dd08d322818895af1ef44
# Wed, 19 Oct 2016 21:55:11 GMT
COPY file:b54d7d4313a41e3729d6f4b7aa6e6f33a1e99759cb2a04149fae89f8211c3a65 in / 
# Wed, 19 Oct 2016 21:56:10 GMT
RUN set -ex 	&& apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 		&& export GOROOT_BOOTSTRAP="$(go env GOROOT)" 		&& wget -q "$GOLANG_SRC_URL" -O golang.tar.gz 	&& echo "$GOLANG_SRC_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz 	&& cd /usr/local/go/src 	&& patch -p2 -i /no-pic.patch 	&& ./make.bash 		&& rm -rf /*.patch 	&& apk del .build-deps
# Wed, 19 Oct 2016 21:56:10 GMT
ENV GOPATH=/go
# Wed, 19 Oct 2016 21:56:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2016 21:56:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 19 Oct 2016 21:56:12 GMT
WORKDIR /go
# Wed, 19 Oct 2016 21:56:12 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c311f66f3ac9a1d4b9fdfa8ac09821993c24d540e6147d25793c861c67892238`  
		Last Modified: Tue, 18 Oct 2016 20:36:01 GMT  
		Size: 344.0 KB (343962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd6f06a512616af4cc963a6a480772417ae6454ddd3449bb322a0c0f7f641`  
		Last Modified: Wed, 19 Oct 2016 22:01:02 GMT  
		Size: 438.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303de2b017481f849acabcedfcd72acd64a9b9fe01ac390d22d745124c878cfc`  
		Last Modified: Wed, 19 Oct 2016 22:01:26 GMT  
		Size: 70.6 MB (70616711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e14a610b962f19fdf5ed742d2d73dd9e0032bb653c6aa4fdbcae4e3156d686b`  
		Last Modified: Wed, 19 Oct 2016 22:01:02 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8c4ac4e92604b79006337436a5b5028212cf8b7bc1dfbd82d68f7034ca03eb`  
		Last Modified: Wed, 19 Oct 2016 22:01:02 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7-alpine`

```console
$ docker pull golang@sha256:25ad25d8bece9d403be107b07c86fb6b2b588a5b26133baa9d1215c07bdbfa39
```

-	Platforms:
	-	linux; amd64

### `golang:1.7-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73275541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e874ba5240682d53411752d2186e74418a9d33d04238ef07b19e7a09db7eeda`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:32:36 GMT
RUN apk add --no-cache ca-certificates
# Wed, 19 Oct 2016 21:55:10 GMT
ENV GOLANG_VERSION=1.7.3
# Wed, 19 Oct 2016 21:55:10 GMT
ENV GOLANG_SRC_URL=https://golang.org/dl/go1.7.3.src.tar.gz
# Wed, 19 Oct 2016 21:55:11 GMT
ENV GOLANG_SRC_SHA256=79430a0027a09b0b3ad57e214c4c1acfdd7af290961dd08d322818895af1ef44
# Wed, 19 Oct 2016 21:55:11 GMT
COPY file:b54d7d4313a41e3729d6f4b7aa6e6f33a1e99759cb2a04149fae89f8211c3a65 in / 
# Wed, 19 Oct 2016 21:56:10 GMT
RUN set -ex 	&& apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 		&& export GOROOT_BOOTSTRAP="$(go env GOROOT)" 		&& wget -q "$GOLANG_SRC_URL" -O golang.tar.gz 	&& echo "$GOLANG_SRC_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz 	&& cd /usr/local/go/src 	&& patch -p2 -i /no-pic.patch 	&& ./make.bash 		&& rm -rf /*.patch 	&& apk del .build-deps
# Wed, 19 Oct 2016 21:56:10 GMT
ENV GOPATH=/go
# Wed, 19 Oct 2016 21:56:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2016 21:56:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 19 Oct 2016 21:56:12 GMT
WORKDIR /go
# Wed, 19 Oct 2016 21:56:12 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c311f66f3ac9a1d4b9fdfa8ac09821993c24d540e6147d25793c861c67892238`  
		Last Modified: Tue, 18 Oct 2016 20:36:01 GMT  
		Size: 344.0 KB (343962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd6f06a512616af4cc963a6a480772417ae6454ddd3449bb322a0c0f7f641`  
		Last Modified: Wed, 19 Oct 2016 22:01:02 GMT  
		Size: 438.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303de2b017481f849acabcedfcd72acd64a9b9fe01ac390d22d745124c878cfc`  
		Last Modified: Wed, 19 Oct 2016 22:01:26 GMT  
		Size: 70.6 MB (70616711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e14a610b962f19fdf5ed742d2d73dd9e0032bb653c6aa4fdbcae4e3156d686b`  
		Last Modified: Wed, 19 Oct 2016 22:01:02 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8c4ac4e92604b79006337436a5b5028212cf8b7bc1dfbd82d68f7034ca03eb`  
		Last Modified: Wed, 19 Oct 2016 22:01:02 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-alpine`

```console
$ docker pull golang@sha256:25ad25d8bece9d403be107b07c86fb6b2b588a5b26133baa9d1215c07bdbfa39
```

-	Platforms:
	-	linux; amd64

### `golang:1-alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73275541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e874ba5240682d53411752d2186e74418a9d33d04238ef07b19e7a09db7eeda`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:32:36 GMT
RUN apk add --no-cache ca-certificates
# Wed, 19 Oct 2016 21:55:10 GMT
ENV GOLANG_VERSION=1.7.3
# Wed, 19 Oct 2016 21:55:10 GMT
ENV GOLANG_SRC_URL=https://golang.org/dl/go1.7.3.src.tar.gz
# Wed, 19 Oct 2016 21:55:11 GMT
ENV GOLANG_SRC_SHA256=79430a0027a09b0b3ad57e214c4c1acfdd7af290961dd08d322818895af1ef44
# Wed, 19 Oct 2016 21:55:11 GMT
COPY file:b54d7d4313a41e3729d6f4b7aa6e6f33a1e99759cb2a04149fae89f8211c3a65 in / 
# Wed, 19 Oct 2016 21:56:10 GMT
RUN set -ex 	&& apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 		&& export GOROOT_BOOTSTRAP="$(go env GOROOT)" 		&& wget -q "$GOLANG_SRC_URL" -O golang.tar.gz 	&& echo "$GOLANG_SRC_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz 	&& cd /usr/local/go/src 	&& patch -p2 -i /no-pic.patch 	&& ./make.bash 		&& rm -rf /*.patch 	&& apk del .build-deps
# Wed, 19 Oct 2016 21:56:10 GMT
ENV GOPATH=/go
# Wed, 19 Oct 2016 21:56:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2016 21:56:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 19 Oct 2016 21:56:12 GMT
WORKDIR /go
# Wed, 19 Oct 2016 21:56:12 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c311f66f3ac9a1d4b9fdfa8ac09821993c24d540e6147d25793c861c67892238`  
		Last Modified: Tue, 18 Oct 2016 20:36:01 GMT  
		Size: 344.0 KB (343962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd6f06a512616af4cc963a6a480772417ae6454ddd3449bb322a0c0f7f641`  
		Last Modified: Wed, 19 Oct 2016 22:01:02 GMT  
		Size: 438.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303de2b017481f849acabcedfcd72acd64a9b9fe01ac390d22d745124c878cfc`  
		Last Modified: Wed, 19 Oct 2016 22:01:26 GMT  
		Size: 70.6 MB (70616711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e14a610b962f19fdf5ed742d2d73dd9e0032bb653c6aa4fdbcae4e3156d686b`  
		Last Modified: Wed, 19 Oct 2016 22:01:02 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8c4ac4e92604b79006337436a5b5028212cf8b7bc1dfbd82d68f7034ca03eb`  
		Last Modified: Wed, 19 Oct 2016 22:01:02 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:alpine`

```console
$ docker pull golang@sha256:25ad25d8bece9d403be107b07c86fb6b2b588a5b26133baa9d1215c07bdbfa39
```

-	Platforms:
	-	linux; amd64

### `golang:alpine` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73275541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e874ba5240682d53411752d2186e74418a9d33d04238ef07b19e7a09db7eeda`

```dockerfile
# Tue, 18 Oct 2016 20:31:22 GMT
ADD file:7afbc23fda8b0b3872623c16af8e3490b2cee951aed14b3794389c2f946cc8c7 in / 
# Tue, 18 Oct 2016 20:32:36 GMT
RUN apk add --no-cache ca-certificates
# Wed, 19 Oct 2016 21:55:10 GMT
ENV GOLANG_VERSION=1.7.3
# Wed, 19 Oct 2016 21:55:10 GMT
ENV GOLANG_SRC_URL=https://golang.org/dl/go1.7.3.src.tar.gz
# Wed, 19 Oct 2016 21:55:11 GMT
ENV GOLANG_SRC_SHA256=79430a0027a09b0b3ad57e214c4c1acfdd7af290961dd08d322818895af1ef44
# Wed, 19 Oct 2016 21:55:11 GMT
COPY file:b54d7d4313a41e3729d6f4b7aa6e6f33a1e99759cb2a04149fae89f8211c3a65 in / 
# Wed, 19 Oct 2016 21:56:10 GMT
RUN set -ex 	&& apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 		&& export GOROOT_BOOTSTRAP="$(go env GOROOT)" 		&& wget -q "$GOLANG_SRC_URL" -O golang.tar.gz 	&& echo "$GOLANG_SRC_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz 	&& cd /usr/local/go/src 	&& patch -p2 -i /no-pic.patch 	&& ./make.bash 		&& rm -rf /*.patch 	&& apk del .build-deps
# Wed, 19 Oct 2016 21:56:10 GMT
ENV GOPATH=/go
# Wed, 19 Oct 2016 21:56:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2016 21:56:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 19 Oct 2016 21:56:12 GMT
WORKDIR /go
# Wed, 19 Oct 2016 21:56:12 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
```

-	Layers:
	-	`sha256:3690ec4760f95690944da86dc4496148a63d85c9e3100669a318110092f6862f`  
		Last Modified: Tue, 18 Oct 2016 20:32:39 GMT  
		Size: 2.3 MB (2312958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c311f66f3ac9a1d4b9fdfa8ac09821993c24d540e6147d25793c861c67892238`  
		Last Modified: Tue, 18 Oct 2016 20:36:01 GMT  
		Size: 344.0 KB (343962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd6f06a512616af4cc963a6a480772417ae6454ddd3449bb322a0c0f7f641`  
		Last Modified: Wed, 19 Oct 2016 22:01:02 GMT  
		Size: 438.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303de2b017481f849acabcedfcd72acd64a9b9fe01ac390d22d745124c878cfc`  
		Last Modified: Wed, 19 Oct 2016 22:01:26 GMT  
		Size: 70.6 MB (70616711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e14a610b962f19fdf5ed742d2d73dd9e0032bb653c6aa4fdbcae4e3156d686b`  
		Last Modified: Wed, 19 Oct 2016 22:01:02 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8c4ac4e92604b79006337436a5b5028212cf8b7bc1dfbd82d68f7034ca03eb`  
		Last Modified: Wed, 19 Oct 2016 22:01:02 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7.3-windowsservercore`

```console
$ docker pull golang@sha256:3ece56dc086d601f92602cd2b028ec3ac72b6fa1f1314b2dead8ef1a728898cd
```

-	Platforms:
	-	windows; amd64

### `golang:1.7.3-windowsservercore` - windows; amd64

-	Docker Version: 1.12.2-cs2-ws-beta
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 GB (4665037934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7570817d9b7efd26c5537a4908274451beb25be732cb5c58ebc3cf24810d60`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Wed, 12 Oct 2016 19:25:22 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Oct 2016 19:25:27 GMT
ENV GIT_VERSION=2.9.2
# Wed, 12 Oct 2016 19:25:32 GMT
ENV GIT_TAG=v2.9.2.windows.1
# Wed, 12 Oct 2016 19:25:35 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.9.2.windows.1/Git-2.9.2-64-bit.exe
# Wed, 12 Oct 2016 19:25:39 GMT
ENV GIT_DOWNLOAD_SHA256=006d971bcbe73cc8d841a100a4eb20d22e135142bf5b0f2120722fd420e166e5
# Tue, 18 Oct 2016 20:43:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.exe -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-Wait 		-FilePath ./git.exe 		-ArgumentList @( 			'/VERYSILENT', 			'/NORESTART', 			'/NOCANCEL', 			'/SP-', 			'/SUPPRESSMSGBOXES', 						'/COMPONENTS=assoc_sh', 						'/DIR=C:\git' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\bin;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 	Write-Host '  bash --version'; bash --version; 	Write-Host '  curl --version'; curl.exe --version; 		Write-Host 'Removing installer ...'; 	Remove-Item git.exe -Force; 		Write-Host 'Complete.';
# Tue, 18 Oct 2016 20:43:13 GMT
ENV GOPATH=C:\gopath
# Tue, 18 Oct 2016 20:43:34 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 19 Oct 2016 21:56:07 GMT
ENV GOLANG_VERSION=1.7.3
# Wed, 19 Oct 2016 21:56:10 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.windows-amd64.zip
# Wed, 19 Oct 2016 21:56:13 GMT
ENV GOLANG_DOWNLOAD_SHA256=9fe41313b97e2a6a703f5ae22938c7d9ac4336a128b522376c224ba97e8c7f01
# Wed, 19 Oct 2016 22:00:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GOLANG_DOWNLOAD_URL -OutFile 'go.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Wed, 19 Oct 2016 22:00:54 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:9c7f9c7d9bc2915388ecc5d08e89a7583658285469d7325281f95d8ee279cc60`  
		Size: 3.7 GB (3737824348 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:de5064718b3f2749727c8b5ffddf2da7698189277afe0df6fc0a57ad573bca0f`  
		Size: 613.1 MB (613059969 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ce8c033b9d9ab0f42b7bc1457fc9094bbf37079117ad712092b3e48f11a6e218`  
		Last Modified: Wed, 12 Oct 2016 19:49:17 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac669cb897e39ec11f318c297f4d37f4fcee666f73329a87d682d483650eb81`  
		Last Modified: Wed, 12 Oct 2016 20:12:47 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637e390ccc606ceb43ffe429ad2eba95a67bbe497de0ac9394d09faee98cb647`  
		Last Modified: Wed, 12 Oct 2016 20:12:47 GMT  
		Size: 1.2 KB (1222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e960bb9bf7ba980b3a5aa3bbbe2e43cbbbbb8bb179e56609a2325db86aab69f`  
		Last Modified: Wed, 12 Oct 2016 20:12:46 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c43be2eca6ba8658363340237b0999be111d6e4b4e76e8bf42f801737692de4`  
		Last Modified: Wed, 12 Oct 2016 20:12:43 GMT  
		Size: 1.2 KB (1205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e0e4bf1429e0a8e00029f128ffac0b63d9f984ce3733deb814d188e3a505ea`  
		Last Modified: Tue, 18 Oct 2016 21:03:28 GMT  
		Size: 215.4 MB (215353361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0185773a0a17452f7ec01e4963e4d512f4831e3a40e9bb1258b9081dec9c4934`  
		Last Modified: Tue, 18 Oct 2016 21:01:48 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a07a6f6ea11b197fcf5338624e85603ff44b33e9a7d1f0aa5c6da047ad5133`  
		Last Modified: Tue, 18 Oct 2016 21:01:51 GMT  
		Size: 4.3 MB (4331070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2bc3fddc893e1a2676c7654121555de160ff68d0329fdc1a0d4b1bc29a8212`  
		Last Modified: Wed, 19 Oct 2016 22:05:26 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb42e03d9415149c5600145a73c72e93598c59f8a0e090041e1e8362690fb43`  
		Last Modified: Wed, 19 Oct 2016 22:05:27 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d05e7fc5ed47ceeb30954754126330b6bef7a07482e97c2fded04c84939fb5`  
		Last Modified: Wed, 19 Oct 2016 22:05:26 GMT  
		Size: 1.2 KB (1215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094da97afa0007ada50fcbe3990dfb8ebbbf606b8989eddc1e00cace479fcf9c`  
		Last Modified: Wed, 19 Oct 2016 22:05:46 GMT  
		Size: 94.5 MB (94457059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6958c270ca502bfe0c9417bbcc74d63de5e46a82a69c7869690eb493fef2f7`  
		Last Modified: Wed, 19 Oct 2016 22:05:26 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7-windowsservercore`

```console
$ docker pull golang@sha256:3ece56dc086d601f92602cd2b028ec3ac72b6fa1f1314b2dead8ef1a728898cd
```

-	Platforms:
	-	windows; amd64

### `golang:1.7-windowsservercore` - windows; amd64

-	Docker Version: 1.12.2-cs2-ws-beta
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 GB (4665037934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7570817d9b7efd26c5537a4908274451beb25be732cb5c58ebc3cf24810d60`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Wed, 12 Oct 2016 19:25:22 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Oct 2016 19:25:27 GMT
ENV GIT_VERSION=2.9.2
# Wed, 12 Oct 2016 19:25:32 GMT
ENV GIT_TAG=v2.9.2.windows.1
# Wed, 12 Oct 2016 19:25:35 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.9.2.windows.1/Git-2.9.2-64-bit.exe
# Wed, 12 Oct 2016 19:25:39 GMT
ENV GIT_DOWNLOAD_SHA256=006d971bcbe73cc8d841a100a4eb20d22e135142bf5b0f2120722fd420e166e5
# Tue, 18 Oct 2016 20:43:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.exe -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-Wait 		-FilePath ./git.exe 		-ArgumentList @( 			'/VERYSILENT', 			'/NORESTART', 			'/NOCANCEL', 			'/SP-', 			'/SUPPRESSMSGBOXES', 						'/COMPONENTS=assoc_sh', 						'/DIR=C:\git' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\bin;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 	Write-Host '  bash --version'; bash --version; 	Write-Host '  curl --version'; curl.exe --version; 		Write-Host 'Removing installer ...'; 	Remove-Item git.exe -Force; 		Write-Host 'Complete.';
# Tue, 18 Oct 2016 20:43:13 GMT
ENV GOPATH=C:\gopath
# Tue, 18 Oct 2016 20:43:34 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 19 Oct 2016 21:56:07 GMT
ENV GOLANG_VERSION=1.7.3
# Wed, 19 Oct 2016 21:56:10 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.windows-amd64.zip
# Wed, 19 Oct 2016 21:56:13 GMT
ENV GOLANG_DOWNLOAD_SHA256=9fe41313b97e2a6a703f5ae22938c7d9ac4336a128b522376c224ba97e8c7f01
# Wed, 19 Oct 2016 22:00:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GOLANG_DOWNLOAD_URL -OutFile 'go.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Wed, 19 Oct 2016 22:00:54 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:9c7f9c7d9bc2915388ecc5d08e89a7583658285469d7325281f95d8ee279cc60`  
		Size: 3.7 GB (3737824348 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:de5064718b3f2749727c8b5ffddf2da7698189277afe0df6fc0a57ad573bca0f`  
		Size: 613.1 MB (613059969 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ce8c033b9d9ab0f42b7bc1457fc9094bbf37079117ad712092b3e48f11a6e218`  
		Last Modified: Wed, 12 Oct 2016 19:49:17 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac669cb897e39ec11f318c297f4d37f4fcee666f73329a87d682d483650eb81`  
		Last Modified: Wed, 12 Oct 2016 20:12:47 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637e390ccc606ceb43ffe429ad2eba95a67bbe497de0ac9394d09faee98cb647`  
		Last Modified: Wed, 12 Oct 2016 20:12:47 GMT  
		Size: 1.2 KB (1222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e960bb9bf7ba980b3a5aa3bbbe2e43cbbbbb8bb179e56609a2325db86aab69f`  
		Last Modified: Wed, 12 Oct 2016 20:12:46 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c43be2eca6ba8658363340237b0999be111d6e4b4e76e8bf42f801737692de4`  
		Last Modified: Wed, 12 Oct 2016 20:12:43 GMT  
		Size: 1.2 KB (1205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e0e4bf1429e0a8e00029f128ffac0b63d9f984ce3733deb814d188e3a505ea`  
		Last Modified: Tue, 18 Oct 2016 21:03:28 GMT  
		Size: 215.4 MB (215353361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0185773a0a17452f7ec01e4963e4d512f4831e3a40e9bb1258b9081dec9c4934`  
		Last Modified: Tue, 18 Oct 2016 21:01:48 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a07a6f6ea11b197fcf5338624e85603ff44b33e9a7d1f0aa5c6da047ad5133`  
		Last Modified: Tue, 18 Oct 2016 21:01:51 GMT  
		Size: 4.3 MB (4331070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2bc3fddc893e1a2676c7654121555de160ff68d0329fdc1a0d4b1bc29a8212`  
		Last Modified: Wed, 19 Oct 2016 22:05:26 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb42e03d9415149c5600145a73c72e93598c59f8a0e090041e1e8362690fb43`  
		Last Modified: Wed, 19 Oct 2016 22:05:27 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d05e7fc5ed47ceeb30954754126330b6bef7a07482e97c2fded04c84939fb5`  
		Last Modified: Wed, 19 Oct 2016 22:05:26 GMT  
		Size: 1.2 KB (1215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094da97afa0007ada50fcbe3990dfb8ebbbf606b8989eddc1e00cace479fcf9c`  
		Last Modified: Wed, 19 Oct 2016 22:05:46 GMT  
		Size: 94.5 MB (94457059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6958c270ca502bfe0c9417bbcc74d63de5e46a82a69c7869690eb493fef2f7`  
		Last Modified: Wed, 19 Oct 2016 22:05:26 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-windowsservercore`

```console
$ docker pull golang@sha256:3ece56dc086d601f92602cd2b028ec3ac72b6fa1f1314b2dead8ef1a728898cd
```

-	Platforms:
	-	windows; amd64

### `golang:1-windowsservercore` - windows; amd64

-	Docker Version: 1.12.2-cs2-ws-beta
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 GB (4665037934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7570817d9b7efd26c5537a4908274451beb25be732cb5c58ebc3cf24810d60`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Wed, 12 Oct 2016 19:25:22 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Oct 2016 19:25:27 GMT
ENV GIT_VERSION=2.9.2
# Wed, 12 Oct 2016 19:25:32 GMT
ENV GIT_TAG=v2.9.2.windows.1
# Wed, 12 Oct 2016 19:25:35 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.9.2.windows.1/Git-2.9.2-64-bit.exe
# Wed, 12 Oct 2016 19:25:39 GMT
ENV GIT_DOWNLOAD_SHA256=006d971bcbe73cc8d841a100a4eb20d22e135142bf5b0f2120722fd420e166e5
# Tue, 18 Oct 2016 20:43:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.exe -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-Wait 		-FilePath ./git.exe 		-ArgumentList @( 			'/VERYSILENT', 			'/NORESTART', 			'/NOCANCEL', 			'/SP-', 			'/SUPPRESSMSGBOXES', 						'/COMPONENTS=assoc_sh', 						'/DIR=C:\git' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\bin;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 	Write-Host '  bash --version'; bash --version; 	Write-Host '  curl --version'; curl.exe --version; 		Write-Host 'Removing installer ...'; 	Remove-Item git.exe -Force; 		Write-Host 'Complete.';
# Tue, 18 Oct 2016 20:43:13 GMT
ENV GOPATH=C:\gopath
# Tue, 18 Oct 2016 20:43:34 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 19 Oct 2016 21:56:07 GMT
ENV GOLANG_VERSION=1.7.3
# Wed, 19 Oct 2016 21:56:10 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.windows-amd64.zip
# Wed, 19 Oct 2016 21:56:13 GMT
ENV GOLANG_DOWNLOAD_SHA256=9fe41313b97e2a6a703f5ae22938c7d9ac4336a128b522376c224ba97e8c7f01
# Wed, 19 Oct 2016 22:00:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GOLANG_DOWNLOAD_URL -OutFile 'go.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Wed, 19 Oct 2016 22:00:54 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:9c7f9c7d9bc2915388ecc5d08e89a7583658285469d7325281f95d8ee279cc60`  
		Size: 3.7 GB (3737824348 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:de5064718b3f2749727c8b5ffddf2da7698189277afe0df6fc0a57ad573bca0f`  
		Size: 613.1 MB (613059969 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ce8c033b9d9ab0f42b7bc1457fc9094bbf37079117ad712092b3e48f11a6e218`  
		Last Modified: Wed, 12 Oct 2016 19:49:17 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac669cb897e39ec11f318c297f4d37f4fcee666f73329a87d682d483650eb81`  
		Last Modified: Wed, 12 Oct 2016 20:12:47 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637e390ccc606ceb43ffe429ad2eba95a67bbe497de0ac9394d09faee98cb647`  
		Last Modified: Wed, 12 Oct 2016 20:12:47 GMT  
		Size: 1.2 KB (1222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e960bb9bf7ba980b3a5aa3bbbe2e43cbbbbb8bb179e56609a2325db86aab69f`  
		Last Modified: Wed, 12 Oct 2016 20:12:46 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c43be2eca6ba8658363340237b0999be111d6e4b4e76e8bf42f801737692de4`  
		Last Modified: Wed, 12 Oct 2016 20:12:43 GMT  
		Size: 1.2 KB (1205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e0e4bf1429e0a8e00029f128ffac0b63d9f984ce3733deb814d188e3a505ea`  
		Last Modified: Tue, 18 Oct 2016 21:03:28 GMT  
		Size: 215.4 MB (215353361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0185773a0a17452f7ec01e4963e4d512f4831e3a40e9bb1258b9081dec9c4934`  
		Last Modified: Tue, 18 Oct 2016 21:01:48 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a07a6f6ea11b197fcf5338624e85603ff44b33e9a7d1f0aa5c6da047ad5133`  
		Last Modified: Tue, 18 Oct 2016 21:01:51 GMT  
		Size: 4.3 MB (4331070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2bc3fddc893e1a2676c7654121555de160ff68d0329fdc1a0d4b1bc29a8212`  
		Last Modified: Wed, 19 Oct 2016 22:05:26 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb42e03d9415149c5600145a73c72e93598c59f8a0e090041e1e8362690fb43`  
		Last Modified: Wed, 19 Oct 2016 22:05:27 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d05e7fc5ed47ceeb30954754126330b6bef7a07482e97c2fded04c84939fb5`  
		Last Modified: Wed, 19 Oct 2016 22:05:26 GMT  
		Size: 1.2 KB (1215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094da97afa0007ada50fcbe3990dfb8ebbbf606b8989eddc1e00cace479fcf9c`  
		Last Modified: Wed, 19 Oct 2016 22:05:46 GMT  
		Size: 94.5 MB (94457059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6958c270ca502bfe0c9417bbcc74d63de5e46a82a69c7869690eb493fef2f7`  
		Last Modified: Wed, 19 Oct 2016 22:05:26 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:windowsservercore`

```console
$ docker pull golang@sha256:3ece56dc086d601f92602cd2b028ec3ac72b6fa1f1314b2dead8ef1a728898cd
```

-	Platforms:
	-	windows; amd64

### `golang:windowsservercore` - windows; amd64

-	Docker Version: 1.12.2-cs2-ws-beta
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 GB (4665037934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7570817d9b7efd26c5537a4908274451beb25be732cb5c58ebc3cf24810d60`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Wed, 12 Oct 2016 19:25:22 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Oct 2016 19:25:27 GMT
ENV GIT_VERSION=2.9.2
# Wed, 12 Oct 2016 19:25:32 GMT
ENV GIT_TAG=v2.9.2.windows.1
# Wed, 12 Oct 2016 19:25:35 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.9.2.windows.1/Git-2.9.2-64-bit.exe
# Wed, 12 Oct 2016 19:25:39 GMT
ENV GIT_DOWNLOAD_SHA256=006d971bcbe73cc8d841a100a4eb20d22e135142bf5b0f2120722fd420e166e5
# Tue, 18 Oct 2016 20:43:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.exe -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-Wait 		-FilePath ./git.exe 		-ArgumentList @( 			'/VERYSILENT', 			'/NORESTART', 			'/NOCANCEL', 			'/SP-', 			'/SUPPRESSMSGBOXES', 						'/COMPONENTS=assoc_sh', 						'/DIR=C:\git' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\bin;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 	Write-Host '  bash --version'; bash --version; 	Write-Host '  curl --version'; curl.exe --version; 		Write-Host 'Removing installer ...'; 	Remove-Item git.exe -Force; 		Write-Host 'Complete.';
# Tue, 18 Oct 2016 20:43:13 GMT
ENV GOPATH=C:\gopath
# Tue, 18 Oct 2016 20:43:34 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 19 Oct 2016 21:56:07 GMT
ENV GOLANG_VERSION=1.7.3
# Wed, 19 Oct 2016 21:56:10 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.windows-amd64.zip
# Wed, 19 Oct 2016 21:56:13 GMT
ENV GOLANG_DOWNLOAD_SHA256=9fe41313b97e2a6a703f5ae22938c7d9ac4336a128b522376c224ba97e8c7f01
# Wed, 19 Oct 2016 22:00:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GOLANG_DOWNLOAD_URL -OutFile 'go.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Wed, 19 Oct 2016 22:00:54 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:9c7f9c7d9bc2915388ecc5d08e89a7583658285469d7325281f95d8ee279cc60`  
		Size: 3.7 GB (3737824348 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:de5064718b3f2749727c8b5ffddf2da7698189277afe0df6fc0a57ad573bca0f`  
		Size: 613.1 MB (613059969 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ce8c033b9d9ab0f42b7bc1457fc9094bbf37079117ad712092b3e48f11a6e218`  
		Last Modified: Wed, 12 Oct 2016 19:49:17 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac669cb897e39ec11f318c297f4d37f4fcee666f73329a87d682d483650eb81`  
		Last Modified: Wed, 12 Oct 2016 20:12:47 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637e390ccc606ceb43ffe429ad2eba95a67bbe497de0ac9394d09faee98cb647`  
		Last Modified: Wed, 12 Oct 2016 20:12:47 GMT  
		Size: 1.2 KB (1222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e960bb9bf7ba980b3a5aa3bbbe2e43cbbbbb8bb179e56609a2325db86aab69f`  
		Last Modified: Wed, 12 Oct 2016 20:12:46 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c43be2eca6ba8658363340237b0999be111d6e4b4e76e8bf42f801737692de4`  
		Last Modified: Wed, 12 Oct 2016 20:12:43 GMT  
		Size: 1.2 KB (1205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e0e4bf1429e0a8e00029f128ffac0b63d9f984ce3733deb814d188e3a505ea`  
		Last Modified: Tue, 18 Oct 2016 21:03:28 GMT  
		Size: 215.4 MB (215353361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0185773a0a17452f7ec01e4963e4d512f4831e3a40e9bb1258b9081dec9c4934`  
		Last Modified: Tue, 18 Oct 2016 21:01:48 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a07a6f6ea11b197fcf5338624e85603ff44b33e9a7d1f0aa5c6da047ad5133`  
		Last Modified: Tue, 18 Oct 2016 21:01:51 GMT  
		Size: 4.3 MB (4331070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2bc3fddc893e1a2676c7654121555de160ff68d0329fdc1a0d4b1bc29a8212`  
		Last Modified: Wed, 19 Oct 2016 22:05:26 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb42e03d9415149c5600145a73c72e93598c59f8a0e090041e1e8362690fb43`  
		Last Modified: Wed, 19 Oct 2016 22:05:27 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d05e7fc5ed47ceeb30954754126330b6bef7a07482e97c2fded04c84939fb5`  
		Last Modified: Wed, 19 Oct 2016 22:05:26 GMT  
		Size: 1.2 KB (1215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094da97afa0007ada50fcbe3990dfb8ebbbf606b8989eddc1e00cace479fcf9c`  
		Last Modified: Wed, 19 Oct 2016 22:05:46 GMT  
		Size: 94.5 MB (94457059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6958c270ca502bfe0c9417bbcc74d63de5e46a82a69c7869690eb493fef2f7`  
		Last Modified: Wed, 19 Oct 2016 22:05:26 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7.3-nanoserver`

```console
$ docker pull golang@sha256:6a0a6a5f9b7966c8e47bd929fe7263a222c3c298e2d94fb6ef7402f2e160cd7e
```

-	Platforms:
	-	windows; amd64

### `golang:1.7.3-nanoserver` - windows; amd64

-	Docker Version: 1.12.2-cs2-ws-beta
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.2 MB (390173157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b1bd5027ee5c46c1b7ec7a2e5ff391ff8b65ee7ec706cdf50a56cef0828117`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 18 Oct 2016 20:47:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 18 Oct 2016 20:48:00 GMT
ENV GOPATH=C:\gopath
# Tue, 18 Oct 2016 20:48:30 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath;
# Wed, 19 Oct 2016 22:00:57 GMT
ENV GOLANG_VERSION=1.7.3
# Wed, 19 Oct 2016 22:00:59 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.windows-amd64.zip
# Wed, 19 Oct 2016 22:01:01 GMT
ENV GOLANG_DOWNLOAD_SHA256=9fe41313b97e2a6a703f5ae22938c7d9ac4336a128b522376c224ba97e8c7f01
# Wed, 19 Oct 2016 22:05:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GOLANG_DOWNLOAD_URL -OutFile 'go.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Wed, 19 Oct 2016 22:05:05 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:5496abde368a3dd39999745bf998c877ddc6a390a943bc3fd99ffaabf728ed88`  
		Size: 242.6 MB (242646586 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:94b4ce7ac4c7c7d4ed75ac2bd9359a87204ad2d5a909759d8e77953874d8e7c2`  
		Size: 56.4 MB (56434068 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12ba288c0d1d424b4832b58c8d542b2b1cc0c8ed873e0f4805a83f705f351eb7`  
		Last Modified: Tue, 18 Oct 2016 21:03:45 GMT  
		Size: 954.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aabf8dca125e29a1422adc206ada519107e390cdc61e481410b7fe3f75538b`  
		Last Modified: Tue, 18 Oct 2016 21:03:45 GMT  
		Size: 962.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3844df32288b9b5de39acf93cc8fd2e0d5662b9b8cefc58c9d5382fc2b6d16d0`  
		Last Modified: Tue, 18 Oct 2016 21:03:46 GMT  
		Size: 819.6 KB (819629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5158e3477b73253cb99d39d049a107b7afa8ddd39f3cc59a28ccbb12d5f477d4`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5e2bb6eccbca69bea5a98ad6568405b210c37cebdd78f5fdb66cfaeea9bb54`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd062b023f999eca0b5d53eea246a998768a2b3419652b492f11a860cb835e3`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03042fad0011efd612ff284853805f358d60146c1c42cb824c5f2d27a5d843e8`  
		Last Modified: Wed, 19 Oct 2016 22:06:23 GMT  
		Size: 90.3 MB (90267137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6024ecc84e3f3810e40761f8eac8e8db0c60b98d1a26bf95f992068ac24ca1`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 953.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7-nanoserver`

```console
$ docker pull golang@sha256:6a0a6a5f9b7966c8e47bd929fe7263a222c3c298e2d94fb6ef7402f2e160cd7e
```

-	Platforms:
	-	windows; amd64

### `golang:1.7-nanoserver` - windows; amd64

-	Docker Version: 1.12.2-cs2-ws-beta
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.2 MB (390173157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b1bd5027ee5c46c1b7ec7a2e5ff391ff8b65ee7ec706cdf50a56cef0828117`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 18 Oct 2016 20:47:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 18 Oct 2016 20:48:00 GMT
ENV GOPATH=C:\gopath
# Tue, 18 Oct 2016 20:48:30 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath;
# Wed, 19 Oct 2016 22:00:57 GMT
ENV GOLANG_VERSION=1.7.3
# Wed, 19 Oct 2016 22:00:59 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.windows-amd64.zip
# Wed, 19 Oct 2016 22:01:01 GMT
ENV GOLANG_DOWNLOAD_SHA256=9fe41313b97e2a6a703f5ae22938c7d9ac4336a128b522376c224ba97e8c7f01
# Wed, 19 Oct 2016 22:05:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GOLANG_DOWNLOAD_URL -OutFile 'go.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Wed, 19 Oct 2016 22:05:05 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:5496abde368a3dd39999745bf998c877ddc6a390a943bc3fd99ffaabf728ed88`  
		Size: 242.6 MB (242646586 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:94b4ce7ac4c7c7d4ed75ac2bd9359a87204ad2d5a909759d8e77953874d8e7c2`  
		Size: 56.4 MB (56434068 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12ba288c0d1d424b4832b58c8d542b2b1cc0c8ed873e0f4805a83f705f351eb7`  
		Last Modified: Tue, 18 Oct 2016 21:03:45 GMT  
		Size: 954.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aabf8dca125e29a1422adc206ada519107e390cdc61e481410b7fe3f75538b`  
		Last Modified: Tue, 18 Oct 2016 21:03:45 GMT  
		Size: 962.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3844df32288b9b5de39acf93cc8fd2e0d5662b9b8cefc58c9d5382fc2b6d16d0`  
		Last Modified: Tue, 18 Oct 2016 21:03:46 GMT  
		Size: 819.6 KB (819629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5158e3477b73253cb99d39d049a107b7afa8ddd39f3cc59a28ccbb12d5f477d4`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5e2bb6eccbca69bea5a98ad6568405b210c37cebdd78f5fdb66cfaeea9bb54`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd062b023f999eca0b5d53eea246a998768a2b3419652b492f11a860cb835e3`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03042fad0011efd612ff284853805f358d60146c1c42cb824c5f2d27a5d843e8`  
		Last Modified: Wed, 19 Oct 2016 22:06:23 GMT  
		Size: 90.3 MB (90267137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6024ecc84e3f3810e40761f8eac8e8db0c60b98d1a26bf95f992068ac24ca1`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 953.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-nanoserver`

```console
$ docker pull golang@sha256:6a0a6a5f9b7966c8e47bd929fe7263a222c3c298e2d94fb6ef7402f2e160cd7e
```

-	Platforms:
	-	windows; amd64

### `golang:1-nanoserver` - windows; amd64

-	Docker Version: 1.12.2-cs2-ws-beta
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.2 MB (390173157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b1bd5027ee5c46c1b7ec7a2e5ff391ff8b65ee7ec706cdf50a56cef0828117`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 18 Oct 2016 20:47:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 18 Oct 2016 20:48:00 GMT
ENV GOPATH=C:\gopath
# Tue, 18 Oct 2016 20:48:30 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath;
# Wed, 19 Oct 2016 22:00:57 GMT
ENV GOLANG_VERSION=1.7.3
# Wed, 19 Oct 2016 22:00:59 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.windows-amd64.zip
# Wed, 19 Oct 2016 22:01:01 GMT
ENV GOLANG_DOWNLOAD_SHA256=9fe41313b97e2a6a703f5ae22938c7d9ac4336a128b522376c224ba97e8c7f01
# Wed, 19 Oct 2016 22:05:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GOLANG_DOWNLOAD_URL -OutFile 'go.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Wed, 19 Oct 2016 22:05:05 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:5496abde368a3dd39999745bf998c877ddc6a390a943bc3fd99ffaabf728ed88`  
		Size: 242.6 MB (242646586 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:94b4ce7ac4c7c7d4ed75ac2bd9359a87204ad2d5a909759d8e77953874d8e7c2`  
		Size: 56.4 MB (56434068 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12ba288c0d1d424b4832b58c8d542b2b1cc0c8ed873e0f4805a83f705f351eb7`  
		Last Modified: Tue, 18 Oct 2016 21:03:45 GMT  
		Size: 954.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aabf8dca125e29a1422adc206ada519107e390cdc61e481410b7fe3f75538b`  
		Last Modified: Tue, 18 Oct 2016 21:03:45 GMT  
		Size: 962.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3844df32288b9b5de39acf93cc8fd2e0d5662b9b8cefc58c9d5382fc2b6d16d0`  
		Last Modified: Tue, 18 Oct 2016 21:03:46 GMT  
		Size: 819.6 KB (819629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5158e3477b73253cb99d39d049a107b7afa8ddd39f3cc59a28ccbb12d5f477d4`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5e2bb6eccbca69bea5a98ad6568405b210c37cebdd78f5fdb66cfaeea9bb54`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd062b023f999eca0b5d53eea246a998768a2b3419652b492f11a860cb835e3`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03042fad0011efd612ff284853805f358d60146c1c42cb824c5f2d27a5d843e8`  
		Last Modified: Wed, 19 Oct 2016 22:06:23 GMT  
		Size: 90.3 MB (90267137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6024ecc84e3f3810e40761f8eac8e8db0c60b98d1a26bf95f992068ac24ca1`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 953.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:nanoserver`

```console
$ docker pull golang@sha256:6a0a6a5f9b7966c8e47bd929fe7263a222c3c298e2d94fb6ef7402f2e160cd7e
```

-	Platforms:
	-	windows; amd64

### `golang:nanoserver` - windows; amd64

-	Docker Version: 1.12.2-cs2-ws-beta
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.2 MB (390173157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b1bd5027ee5c46c1b7ec7a2e5ff391ff8b65ee7ec706cdf50a56cef0828117`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 18 Oct 2016 20:47:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 18 Oct 2016 20:48:00 GMT
ENV GOPATH=C:\gopath
# Tue, 18 Oct 2016 20:48:30 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath;
# Wed, 19 Oct 2016 22:00:57 GMT
ENV GOLANG_VERSION=1.7.3
# Wed, 19 Oct 2016 22:00:59 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.3.windows-amd64.zip
# Wed, 19 Oct 2016 22:01:01 GMT
ENV GOLANG_DOWNLOAD_SHA256=9fe41313b97e2a6a703f5ae22938c7d9ac4336a128b522376c224ba97e8c7f01
# Wed, 19 Oct 2016 22:05:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GOLANG_DOWNLOAD_URL -OutFile 'go.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Wed, 19 Oct 2016 22:05:05 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:5496abde368a3dd39999745bf998c877ddc6a390a943bc3fd99ffaabf728ed88`  
		Size: 242.6 MB (242646586 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:94b4ce7ac4c7c7d4ed75ac2bd9359a87204ad2d5a909759d8e77953874d8e7c2`  
		Size: 56.4 MB (56434068 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12ba288c0d1d424b4832b58c8d542b2b1cc0c8ed873e0f4805a83f705f351eb7`  
		Last Modified: Tue, 18 Oct 2016 21:03:45 GMT  
		Size: 954.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aabf8dca125e29a1422adc206ada519107e390cdc61e481410b7fe3f75538b`  
		Last Modified: Tue, 18 Oct 2016 21:03:45 GMT  
		Size: 962.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3844df32288b9b5de39acf93cc8fd2e0d5662b9b8cefc58c9d5382fc2b6d16d0`  
		Last Modified: Tue, 18 Oct 2016 21:03:46 GMT  
		Size: 819.6 KB (819629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5158e3477b73253cb99d39d049a107b7afa8ddd39f3cc59a28ccbb12d5f477d4`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5e2bb6eccbca69bea5a98ad6568405b210c37cebdd78f5fdb66cfaeea9bb54`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd062b023f999eca0b5d53eea246a998768a2b3419652b492f11a860cb835e3`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03042fad0011efd612ff284853805f358d60146c1c42cb824c5f2d27a5d843e8`  
		Last Modified: Wed, 19 Oct 2016 22:06:23 GMT  
		Size: 90.3 MB (90267137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6024ecc84e3f3810e40761f8eac8e8db0c60b98d1a26bf95f992068ac24ca1`  
		Last Modified: Wed, 19 Oct 2016 22:06:04 GMT  
		Size: 953.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
