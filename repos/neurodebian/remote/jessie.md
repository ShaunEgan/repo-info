## `neurodebian:jessie`

```console
$ docker pull neurodebian@sha256:290406e5439b63d4dbb811c3272e0c7ea1b230e3205ea1302b7d9747fedb238e
```

-	Platforms:
	-	linux; amd64

### `neurodebian:jessie` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51356958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba0f6b9cdf10e7b61733578f73085a91174ad43429e340ce9649a60200b3299c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 22:30:03 GMT
RUN which gpg || { apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*; }
# Fri, 21 Oct 2016 22:30:04 GMT
RUN echo 'deb http://neuro.debian.net/debian jessie main' > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 21 Oct 2016 22:30:05 GMT
RUN echo 'deb http://neuro.debian.net/debian data main' >> /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 21 Oct 2016 22:30:06 GMT
RUN echo '#deb-src http://neuro.debian.net/debian-devel jessie main' >> /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 21 Oct 2016 22:30:07 GMT
RUN apt-key adv --recv-keys --keyserver pgp.mit.edu 0xA5D32F012649A5A9
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15699712ef1b5295d8fd90500448673882e661b6fa9633a5fc72e753e93b6227`  
		Last Modified: Fri, 21 Oct 2016 22:30:17 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5dfb88e76ba6455889c4442e9bff2898c865dd6e8caa4379a580360803ac10`  
		Last Modified: Fri, 21 Oct 2016 22:30:17 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceea3c336b780354054c14c5c613dfd8cebc39216ab50a9de7b07a0a494b9f11`  
		Last Modified: Fri, 21 Oct 2016 22:30:17 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7eb0300bf5c19cd3ca1d07ed44e838ba8b435460fb10e844bb13b7d23e2f54`  
		Last Modified: Fri, 21 Oct 2016 22:30:17 GMT  
		Size: 3.2 KB (3167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
