# Maintainer: Your Name <youremail@domain.com>
pkgname=maxflow
pkgver=3.0.5
pkgrel=1
pkgdesc="This software library implements the maxflow algorithm"
arch=('any')
url="https://packages.ubuntu.com/groovy/libmaxflow0"
license=('GPL')
changelog="CHANGES.txt"
source=("https://github.com/gerddie/$pkgname/archive/$pkgver.tar.gz")
md5sums=('SKIP')

build() {
	cd "$pkgname-$pkgver"
	cmake -DCMAKE_INSTALL_PREFIX=/usr ./
	make
}

package() {
	cd "$pkgname-$pkgver"
	sudo make install
}

