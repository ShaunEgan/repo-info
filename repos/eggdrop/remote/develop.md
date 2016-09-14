## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:c0e5fdca41a68d9f6e454624707fa8796cf82dddc08c29f69ad00395ab7197ce
```

-	Platforms:
	-	linux; amd64

### `eggdrop:develop` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8275680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9659a70f9bd4a8cfbd74ca25707bd1aac14d5ab85a0162645338620cb7bdb8d`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 29 Aug 2016 23:49:14 GMT
ADD file:852e9d0cb9d906535af512a89339fc70b2873a0f94defbcbe41cd44942dd6ac8 in / 
# Tue, 30 Aug 2016 00:25:04 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 30 Aug 2016 00:25:05 GMT
RUN adduser -S eggdrop
# Tue, 30 Aug 2016 00:25:06 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 13 Sep 2016 16:51:20 GMT
ENV EGGDROP_SHA256=4e3f1e4b52d2c9ae0df9d7c9cfabf501f8ca39a08c7f8556cc5abe49e280b6e8
# Tue, 13 Sep 2016 16:51:20 GMT
ENV EGGDROP_COMMIT=1a2ac64b9afd3bba52513a41adf8d8ac672177e4
# Tue, 13 Sep 2016 16:51:57 GMT
RUN apk add --no-cache tcl tcl-dev wget ca-certificates make tar gpgme bash build-base   && wget https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz -O develop.tar.gz  && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure --with-tclinc=/usr/include/tcl8.6/tcl.h --with-tcllib=/usr/lib/x86_64-linux-gnu/libtcl8.6.so     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del tcl-dev wget ca-certificates make tar gpgme build-base
# Tue, 13 Sep 2016 16:51:57 GMT
ENV NICK=
# Tue, 13 Sep 2016 16:51:58 GMT
ENV SERVER=
# Tue, 13 Sep 2016 16:51:58 GMT
ENV LISTEN=3333
# Tue, 13 Sep 2016 16:51:58 GMT
ENV OWNER=
# Tue, 13 Sep 2016 16:51:58 GMT
ENV USERFILE=eggdrop.user
# Tue, 13 Sep 2016 16:51:58 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 13 Sep 2016 16:51:59 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 13 Sep 2016 16:51:59 GMT
EXPOSE 3333/tcp
# Tue, 13 Sep 2016 16:51:59 GMT
COPY file:655c2fd77a7cf08b712ee33a15d7dbd177b8489a67560628236c68c2cc66aa58 in /home/eggdrop/eggdrop 
# Tue, 13 Sep 2016 16:52:00 GMT
COPY file:919804e5ddd4c807c178caccfed03e9d75a459fe0f744c3a1ada109817cb44ec in /home/eggdrop/eggdrop/scripts/ 
# Tue, 13 Sep 2016 16:52:00 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 13 Sep 2016 16:52:00 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:e110a4a1794126ef308a49f2d65785af2f25538f06700721aad8283b81fdfa58`  
		Last Modified: Thu, 23 Jun 2016 19:56:16 GMT  
		Size: 2.3 MB (2310286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e774eb22893af3cb3df3cc57fd62fda219bb72a480ca9448ff46545ec20849`  
		Last Modified: Tue, 30 Aug 2016 21:07:32 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57df40530376f1bd1f04e0439e8e09f6d920071c537741a87faeaa6979bc73a2`  
		Last Modified: Tue, 30 Aug 2016 21:07:33 GMT  
		Size: 7.9 KB (7925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba457cd29543b83b527247c3bf1674512e4556dce0ab5863679c70de63c11d24`  
		Last Modified: Tue, 13 Sep 2016 16:52:48 GMT  
		Size: 6.0 MB (5953951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7148df4768eb9517a35f4f3ebc8c9b7e3b2cfe07eca362c438b8aa94869ee389`  
		Last Modified: Tue, 13 Sep 2016 16:52:46 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622344ce4e75891610cb997b4d5a1daac82c9bbe2c0d69316b195b727bbf5553`  
		Last Modified: Tue, 13 Sep 2016 16:52:45 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip