# Maintainer: Matyas Albert Nagy <albertmatyi@gmail.com>
pkgname=unpaper
pkgver=1.0
pkgrel=1
epoch=
pkgdesc="unpaper sets wallpapers downloaded from unsplash.com"
arch=('any')
url=""
license=('MIT')
groups=()
depends=('curl' 'xorg-xrandr' 'feh')
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=("unpaper")
noextract=()
md5sums=()
validpgpkeys=()

prepare() {
	cd "$pkgname-$pkgver"
	patch -p1 -i "$srcdir/$pkgname-$pkgver.patch"
}

build() {
	cd "$pkgname-$pkgver"
	./configure --prefix=/usr
	make
}

check() {
	cd "$pkgname-$pkgver"
	make -k check
}

package() {
	cd "$pkgname-$pkgver"
	make DESTDIR="$pkgdir/" install
}
