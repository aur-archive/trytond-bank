# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-bank
_pkgname=trytond_bank
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The bank module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-party>=3.4' 'trytond-currency>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("22d0eebbd023eb1af1a40db1ed351434")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}