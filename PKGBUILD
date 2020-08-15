# Maintainer: Hendrik de Bruin
pkgname=stdman
pkgver=0.0.0
pkgrel=1
epoch=
pkgdesc="man pages from cppref"
arch=(x86_64)
url="https://en.cppreference.com/w/"
license=('MIT')

prepare() {
	cd $srcdir
	git clone https://github.com/jeaye/stdman.git
}

build() {
	cd $srcdir
	cd stdman
	./configure --mandir=$pkgdir/usr/local/man
}

package() {
	cd $srcdir
	cd stdman
	make install
}
