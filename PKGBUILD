# Maintainer: Samuel Tardieu <sam@rfc1149.net>
pkgname=python2-slowaes
pkgver=0.1a1
pkgrel=2
pkgdesc="Implementation of AES in Python"
arch=('any')
url="http://code.google.com/p/slowaes/"
license=('Apache')
groups=()
depends=('python2')
makedepends=('python2-distribute')
provides=()
conflicts=()
replaces=()
backup=()
options=(!emptydirs)
install=
source=("http://pypi.python.org/packages/source/s/slowaes/slowaes-$pkgver.tar.gz")
md5sums=('eafee95a788a795403e972a35e80ce4f')

package() {
  cd "$srcdir/slowaes-$pkgver"
  sed -ie 's#/usr/bin/python#/usr/bin/python2#' aes.py
  python2 setup.py install --root="$pkgdir/" --optimize=1
}

# vim:set ts=2 sw=2 et:
