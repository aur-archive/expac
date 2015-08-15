# $Id: PKGBUILD 51880 2011-07-17 19:50:14Z dreisner $
# Maintainer: Dave Reisner <d@falconindy.com>

pkgname=expac
pkgver=0.05
pkgrel=1
pkgdesc="pacman database extraction utility"
arch=('i686' 'x86_64')
url="http://github.com/falconindy/expac"
license=('GPL')
depends=('pacman')
makedepends=('perl')
source=("https://github.com/downloads/falconindy/$pkgname/$pkgname-$pkgver.tar.gz")
md5sums=('366d741b21d1029c63a5e977d3fc08db')

build() {
  cd "$srcdir/$pkgname-$pkgver"
  make
}

package() {
  cd "$srcdir/$pkgname-$pkgver"
  make PREFIX=/usr DESTDIR="$pkgdir" install
}

# vim: ft=sh syn=sh
