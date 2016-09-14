## `pypy:3-5-slim`

```console
$ docker pull pypy@sha256:0000d7a98f2a801861661c80d254e1cb17df186401b479933e490844330d2988
```

-	Platforms:
	-	linux; amd64

### `pypy:3-5-slim` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80147580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a4e2b44bab4fc6a1dc94db2e1681650de4ecaa3ca067b9bb6734cbf2bae18ed`
-	Default Command: `["pypy3"]`

```dockerfile
# Tue, 30 Aug 2016 21:00:51 GMT
ADD file:f2453b914e7e026efd39c6321c7b14509b6d09dd3cf5567a8f6bd38466e06954 in / 
# Tue, 30 Aug 2016 21:00:52 GMT
CMD ["/bin/bash"]
# Wed, 31 Aug 2016 02:39:27 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Aug 2016 02:39:27 GMT
ENV LANG=C.UTF-8
# Thu, 08 Sep 2016 20:53:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Thu, 08 Sep 2016 20:54:26 GMT
ENV PYPY_VERSION=5.2.0-alpha1
# Thu, 08 Sep 2016 20:54:27 GMT
ENV PYPY_SHA256SUM=f5e66ab24267d6ddf662d07c512d06c10ebc732ae62093dabbd775ac63b9060a
# Thu, 08 Sep 2016 20:54:27 GMT
ENV PYTHON_PIP_VERSION=8.1.2
# Thu, 08 Sep 2016 20:54:54 GMT
RUN set -ex 	&& fetchDeps=' 		bzip2 		wget 	' 	&& apt-get update && apt-get install -y $fetchDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3.3-v${PYPY_VERSION}-linux64.tar.bz2" 	&& echo "$PYPY_SHA256SUM  pypy.tar.bz2" | sha256sum -c 	&& tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2 	&& rm pypy.tar.bz2 		&& if [ ! -e /usr/local/bin/pip3 ]; then : 		&& wget -O /tmp/get-pip.py 'https://bootstrap.pypa.io/get-pip.py' 		&& pypy3 /tmp/get-pip.py "pip==$PYTHON_PIP_VERSION" 		&& rm /tmp/get-pip.py 	; fi 	&& pip3 install --no-cache-dir --upgrade --force-reinstall "pip==$PYTHON_PIP_VERSION" 	&& [ "$(pip list |tac|tac| awk -F '[ ()]+' '$1 == "pip" { print $2; exit }')" = "$PYTHON_PIP_VERSION" ] 		&& apt-get purge -y --auto-remove $fetchDeps 	&& rm -rf ~/.cache
# Thu, 08 Sep 2016 20:54:54 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:8ad8b3f87b378cfae583fef34e47a3c9203847d779961b7351cbf786af0bc09f`  
		Last Modified: Tue, 30 Aug 2016 21:02:02 GMT  
		Size: 51.4 MB (51367268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3201fa3d047251e1cd4d144a7c8182853606fd2d2cd67e45c29632c208c16e7b`  
		Last Modified: Thu, 08 Sep 2016 20:55:48 GMT  
		Size: 3.5 MB (3464735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061b6fe40e37cfb01170de30a0297d4f18d48bcd37c9c0be3d779b20a6336a8d`  
		Last Modified: Thu, 08 Sep 2016 20:58:13 GMT  
		Size: 25.3 MB (25315577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip