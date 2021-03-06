## `haskell:latest`

```console
$ docker pull haskell@sha256:f24b5610aa487ea75ea89b27b51bbc9e34185d7a2a88a7715f9f4bd6e076c4a0
```

-	Platforms:
	-	linux; amd64

### `haskell:latest` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.4 MB (252353659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fdc855e1dc5dbd0a3f0229720e116aa22477d93144310773c682d47626c9c5b`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 19:48:26 GMT
MAINTAINER Chris Biscardi <chris@christopherbiscardi.com>
# Fri, 21 Oct 2016 19:48:27 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2016 19:49:49 GMT
RUN echo 'deb http://ppa.launchpad.net/hvr/ghc/ubuntu trusty main' > /etc/apt/sources.list.d/ghc.list &&     echo 'deb http://download.fpcomplete.com/debian/jessie stable main'| tee /etc/apt/sources.list.d/fpco.list &&     apt-key adv --keyserver keyserver.ubuntu.com --recv-keys F6F88286 &&     apt-key adv --keyserver keyserver.ubuntu.com --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     apt-get update &&     apt-get install -y --no-install-recommends cabal-install-1.24 ghc-8.0.1 happy-1.19.5 alex-3.1.7             stack zlib1g-dev libtinfo-dev libsqlite3-0 libsqlite3-dev ca-certificates g++ git &&     rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 19:49:50 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/1.24/bin:/opt/ghc/8.0.1/bin:/opt/happy/1.19.5/bin:/opt/alex/3.1.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2016 19:49:50 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0dc87dd6169c8b7ac5deb134a7823d4c77026b4d928b1968fb19ecf2183a8d`  
		Last Modified: Fri, 21 Oct 2016 19:51:03 GMT  
		Size: 201.0 MB (201000534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
