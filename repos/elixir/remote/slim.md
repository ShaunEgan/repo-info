## `elixir:slim`

```console
$ docker pull elixir@sha256:483b361f40ce1d18f75df8c93c03d1d2d0ce88fd4226434e8a853c7f4db3c134
```

-	Platforms:
	-	linux; amd64

### `elixir:slim` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120539671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbf33b2f7d6b015d32015044c58b91c2f8ed84c2784d86e927b3897e1f3d5b6a`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 28 Jul 2016 17:47:54 GMT
ADD file:0e0565652aa852f62033d99f84892216020d30f64521ded5e72d4940bc4c9697 in /
# Thu, 28 Jul 2016 17:47:55 GMT
CMD ["/bin/bash"]
# Mon, 22 Aug 2016 17:12:51 GMT
ENV OTP_VERSION=19.0.5
# Mon, 22 Aug 2016 17:30:10 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="1cf9e6e9519b7191607f37045a7660bb0c70c285bb591dd2b3fca62e06403540" 	&& runtimeDeps=' 		libodbc1 		libssl1.0.0 		libsctp1 	' 	&& buildDeps=' 		curl 		ca-certificates 		autoconf 		gcc 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256 otp-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/otp-src 	&& tar -xzf otp-src.tar.gz -C /usr/src/otp-src --strip-components=1 	&& rm otp-src.tar.gz 	&& cd /usr/src/otp-src 	&& ./otp_build autoconf 	&& ./configure --enable-sctp 	&& make -j$(nproc) 	&& make install 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/otp-src /var/lib/apt/lists/*
# Mon, 22 Aug 2016 17:30:11 GMT
CMD ["erl"]
# Mon, 22 Aug 2016 19:14:50 GMT
ENV ELIXIR_VERSION=v1.3.2 LANG=C.UTF-8
# Mon, 22 Aug 2016 19:16:22 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/releases/download/${ELIXIR_VERSION}/Precompiled.zip" 	&& ELIXIR_DOWNLOAD_SHA256="45fdb9464b0fbe44c919482f1247740cc9c5d399280ef07e386aa7402b085be7" 	&& buildDeps=' 		ca-certificates 		curl 		unzip 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-precompiled.zip $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256 elixir-precompiled.zip" | sha256sum -c - 	&& unzip -d /usr/local elixir-precompiled.zip 	&& rm elixir-precompiled.zip 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 22 Aug 2016 19:16:23 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:357ea8c3d80bc25792e010facfc98aee5972ebc47e290eb0d5aea3671a901cab`  
		Last Modified: Thu, 28 Jul 2016 17:49:58 GMT  
		Size: 51.4 MB (51365611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0779269a676b5211f1201a7411e37ba368fe6fef1cbd9a7fa5ab24ee699ef65f`  
		Last Modified: Mon, 22 Aug 2016 17:54:11 GMT  
		Size: 65.4 MB (65438269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc889f4b9e8f125e8a52e03718b7516ea24cb56e9d776d05dfff5a674e9f0a67`  
		Last Modified: Mon, 22 Aug 2016 19:16:38 GMT  
		Size: 3.7 MB (3735791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip