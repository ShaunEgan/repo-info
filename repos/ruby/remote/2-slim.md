## `ruby:2-slim`

```console
$ docker pull ruby@sha256:7404c632cf47f36fb78e00e9c12477e1f9c82e5f50fef498e59fc5b6ca40caee
```

-	Platforms:
	-	linux; amd64

### `ruby:2-slim` - linux; amd64

-	Docker Version: 1.12.2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97482462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35b7fbbbe32c9768d5691db1aa75b5a33b30f91007f655802cc4b5cee79789c5`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Oct 2016 01:14:55 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgdbm3 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/*
# Sat, 22 Oct 2016 01:14:56 GMT
RUN mkdir -p /usr/local/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 22 Oct 2016 01:14:56 GMT
ENV RUBY_MAJOR=2.3
# Sat, 22 Oct 2016 01:14:57 GMT
ENV RUBY_VERSION=2.3.1
# Sat, 22 Oct 2016 01:14:57 GMT
ENV RUBY_DOWNLOAD_SHA256=b87c738cb2032bf4920fef8e3864dc5cf8eae9d89d8d523ce0236945c5797dcd
# Tue, 01 Nov 2016 18:19:42 GMT
ENV RUBYGEMS_VERSION=2.6.8
# Tue, 01 Nov 2016 18:22:23 GMT
RUN set -ex 		&& buildDeps=' 		autoconf 		bison 		gcc 		libbz2-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O ruby.tar.gz "https://cache.ruby-lang.org/pub/ruby/$RUBY_MAJOR/ruby-$RUBY_VERSION.tar.gz" 	&& echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.gz" | sha256sum -c - 		&& mkdir -p /usr/src/ruby 	&& tar -xzf ruby.tar.gz -C /usr/src/ruby --strip-components=1 	&& rm ruby.tar.gz 		&& cd /usr/src/ruby 		&& { 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new 	&& mv file.c.new file.c 		&& autoconf 	&& ./configure --disable-install-doc 	&& make -j"$(nproc)" 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& cd / 	&& rm -r /usr/src/ruby 		&& gem update --system "$RUBYGEMS_VERSION"
# Tue, 01 Nov 2016 18:22:24 GMT
ENV BUNDLER_VERSION=1.13.6
# Tue, 01 Nov 2016 18:22:25 GMT
RUN gem install bundler --version "$BUNDLER_VERSION"
# Tue, 01 Nov 2016 18:22:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 01 Nov 2016 18:22:25 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_BIN=/usr/local/bundle/bin BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 01 Nov 2016 18:22:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2016 18:22:26 GMT
RUN mkdir -p "$GEM_HOME" "$BUNDLE_BIN" 	&& chmod 777 "$GEM_HOME" "$BUNDLE_BIN"
# Tue, 01 Nov 2016 18:22:27 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0a11f098842dc14361e47f8a50f59accbe7a4a4efb4842c4492b949cde211a`  
		Last Modified: Sat, 22 Oct 2016 01:17:57 GMT  
		Size: 10.0 MB (9980336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832c79cd44b54926d1eb92d221168d7f5a5a0562524e427861493f037a568c75`  
		Last Modified: Sat, 22 Oct 2016 01:17:53 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da24b8939d0dfef1233f86910c9f7761210af8df19eed696b11f0bfb3376bbb`  
		Last Modified: Tue, 01 Nov 2016 18:32:29 GMT  
		Size: 35.5 MB (35536062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a632bbae2b7197cf453e32910157502e60828816a06a762a016c7c2f3d3ddaa`  
		Last Modified: Tue, 01 Nov 2016 18:32:12 GMT  
		Size: 612.6 KB (612577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993615004a4ea4b109d8784d3d48b531c285bebac925220a67a9e9dded606560`  
		Last Modified: Tue, 01 Nov 2016 18:32:12 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
