## `odoo:latest`

```console
$ docker pull odoo@sha256:9dda179a2b818130c4346e4ad2ae830d4a44a140070c68cb4e24e53ca7b2514e
```

-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

-	Docker Version: 1.12.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.7 MB (271723061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e0de364896f833048a8ba1ac8d4f79a61c126c06270dc0650181be327241dbe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Fri, 21 Oct 2016 16:22:34 GMT
ADD file:23aa4f893e3288698c017b90be657911b72d54edb3b3a7c4d05c308f50f9228f in / 
# Fri, 21 Oct 2016 16:22:34 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2016 22:46:26 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Mon, 31 Oct 2016 23:38:44 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             node-less             python-gevent             python-pip             python-pyinotify             python-renderpm             python-support         && curl -o wkhtmltox.deb -SL http://nightly.odoo.com/extra/wkhtmltox-0.12.1.2_linux-jessie-amd64.deb         && echo '40e8b906de658a2221b15e4e8cd82565a47d7ee8 wkhtmltox.deb' | sha1sum -c -         && dpkg --force-depends -i wkhtmltox.deb         && apt-get -y install -f --no-install-recommends         && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false -o APT::AutoRemove::SuggestsImportant=false npm         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb         && pip install psycogreen==1.0
# Mon, 31 Oct 2016 23:40:03 GMT
ENV ODOO_VERSION=10.0
# Thu, 03 Nov 2016 19:28:18 GMT
ENV ODOO_RELEASE=20161103
# Thu, 03 Nov 2016 19:29:07 GMT
RUN set -x;         curl -o odoo.deb -SL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo '298b9a3c752fbe8df1e6bc7e5ab9d84ce7d0061b odoo.deb' | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 03 Nov 2016 19:29:09 GMT
COPY file:47d94ca963470d9d965c44f9ee07bdfed21bf7be5b46925e55818de15ce0bdb1 in / 
# Thu, 03 Nov 2016 19:29:09 GMT
COPY file:5cd4425a11ba7c482740572351bc33ea5b877795c1d6240fe07667b118dc3740 in /etc/odoo/ 
# Thu, 03 Nov 2016 19:29:10 GMT
RUN chown odoo /etc/odoo/odoo.conf
# Thu, 03 Nov 2016 19:29:11 GMT
RUN mkdir -p /mnt/extra-addons         && chown -R odoo /mnt/extra-addons
# Thu, 03 Nov 2016 19:29:11 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 03 Nov 2016 19:29:11 GMT
EXPOSE 8069/tcp 8071/tcp
# Thu, 03 Nov 2016 19:29:11 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 03 Nov 2016 19:29:12 GMT
USER [odoo]
# Thu, 03 Nov 2016 19:29:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Nov 2016 19:29:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:43c265008fae5d1f3cbee0dac9697235320b174d85acbed002a4fe44236adec0`  
		Last Modified: Fri, 21 Oct 2016 16:22:58 GMT  
		Size: 51.4 MB (51353125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ffed833a60de1cd27e448c5ce63cb4c8c78e1ac896b4b2da23986e17266ab9`  
		Last Modified: Mon, 31 Oct 2016 23:43:50 GMT  
		Size: 86.0 MB (85980676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c77683ace25f2af113a296edcb0dc42eb6a4b50f37dbe8c3b6575babe107e7f`  
		Last Modified: Thu, 03 Nov 2016 19:32:15 GMT  
		Size: 134.4 MB (134387567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365b0a5bd1ab8c65575e07e5a062631252283adb13941d6367644c9b1cc8eb51`  
		Last Modified: Thu, 03 Nov 2016 19:31:38 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b79415104a9484c3a9143b70d235cca577a98ad0722e86112119c8d06d67e34`  
		Last Modified: Thu, 03 Nov 2016 19:31:41 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa217fe0543fe1c753123206a8f943600650a1a3d795d02a6870489c1ca5090`  
		Last Modified: Thu, 03 Nov 2016 19:31:39 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472160712c3802434e4108921db5318d1fcc7693a00381eb6be70cc5dd975106`  
		Last Modified: Thu, 03 Nov 2016 19:31:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
