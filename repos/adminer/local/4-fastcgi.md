# `adminer:4.3.1-fastcgi`

## Docker Metadata

- Image ID: `sha256:b64b35f15146907653732eb746b8a938815f7b7cfa6aec912fd3812af382e9f1`
- Created: `2017-12-14T01:52:11.455657202Z`
- Virtual Size: ~ 71.39 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
- Command: `["php-fpm"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c`
  - `PHP_INI_DIR=/usr/local/etc/php`
  - `PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data`
  - `PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2`
  - `PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2`
  - `PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie`
  - `GPG_KEYS=1A4E8B7277C42E53DBA9C7B9BCAA30EA9C0D5763 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3`
  - `PHP_VERSION=7.0.26`
  - `PHP_URL=https://secure.php.net/get/php-7.0.26.tar.xz/from/this/mirror`
  - `PHP_ASC_URL=https://secure.php.net/get/php-7.0.26.tar.xz.asc/from/this/mirror`
  - `PHP_SHA256=ed5cbb4bbb0ddef8985f100bba2e94002ad22a230b5da2dccfe148915df5f199`
  - `PHP_MD5=`
  - `ADMINER_VERSION=4.3.1`
  - `ADMINER_DOWNLOAD_SHA256=71688c5db4d4e504c48c26ec2966ad85e721ef61e0377c5505cfb50b026d5491`
  - `ADMINER_SRC_DOWNLOAD_SHA256=fd016c93bb3bb8e85ed9cf826064584012c4db83f30c4948d701250e29a6d953`
