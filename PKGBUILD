# Maintainer: TildeHacker <contact@tildehacker.com>
pkgname=ideapad-cm
pkgver=0.1.0
pkgrel=1
epoch=
license=('GPL')
pkgdesc="A script to enable/disable battery conservation mode in Lenovo Ideapad laptops."
arch=('any')
url="https://github.com/tildehacker/ideapad-conservation-mode"
groups=()
depends=()
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
source=("$pkgname-$pkgver.tar.gz"
        "$pkgname-$pkgver.patch")
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
