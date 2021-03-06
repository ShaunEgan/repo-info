## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:50776f5a1c70ae08a6ec86324df7d2e06c2121e7bc790485b62aa0f5e22b9bba
```

-	Platforms:
	-	linux; amd64

### `kapacitor:latest` - linux; amd64

-	Docker Version: 1.12.1
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.7 MB (80714933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d19abac1419e724552a647777a173c4053524baca92dc116b7203ff2d69b4c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 16:36:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Oct 2016 17:00:58 GMT
RUN gpg     --keyserver hkp://ha.pool.sks-keyservers.net     --recv-keys 05CE15085FC09D18E99EFB22684A14CF2582E0C5
# Fri, 21 Oct 2016 20:23:48 GMT
ENV KAPACITOR_VERSION=1.0.2
# Fri, 21 Oct 2016 20:23:53 GMT
RUN wget -q https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_amd64.deb.asc &&     wget -q https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_amd64.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_amd64.deb.asc kapacitor_${KAPACITOR_VERSION}_amd64.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_amd64.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_amd64.deb*
# Fri, 21 Oct 2016 20:23:54 GMT
COPY file:965f70a8f6603417e3e4564d3c3f35b5941a4ba7cb09a86047810948e33d0831 in /etc/kapacitor/kapacitor.conf 
# Fri, 21 Oct 2016 20:23:54 GMT
EXPOSE 9092/tcp
# Fri, 21 Oct 2016 20:23:54 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 21 Oct 2016 20:23:55 GMT
COPY file:e5d90b0779cb7845ca3a7981c04a97fd959fea211a2ce19c8da8b949f9d9d04c in /entrypoint.sh 
# Fri, 21 Oct 2016 20:23:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Oct 2016 20:23:56 GMT
CMD ["kapacitord"]
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
	-	`sha256:f10198f87fbc28bbf73a456f081f51ecab6d64a371fbc91d492e7703b3d69a00`  
		Last Modified: Fri, 21 Oct 2016 17:01:15 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7c2bfa7e0859c2ecfe010cfbed6174cdc345fa8820450c334b4c12231d5937`  
		Last Modified: Fri, 21 Oct 2016 20:24:09 GMT  
		Size: 10.8 MB (10826476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daae2d4cc9e6024142ab97f21da6afb0b903d4bb44143667b5acd3715e04fc9f`  
		Last Modified: Fri, 21 Oct 2016 20:24:05 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274049b9406262ceab03df0d29f6ee9df3b6d81a8d1a1067c4a3aebee38c4ace`  
		Last Modified: Fri, 21 Oct 2016 20:24:05 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
