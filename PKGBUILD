# Author: Alexis Sellier <self@cloudhead.net>
# Contributor: The Core Less Team
# Maintainer: cloudhead <self@cloudhead.net>
# Maintainer: agatronic <luke.a.page@gmail.com>
_npmname=less
_npmver=1.7.5
pkgname=nodejs-less # All lowercase
pkgver=1.7.5
pkgrel=1
pkgdesc="Leaner CSS"
arch=(any)
url="http://lesscss.org"
license=(Apache v2)
depends=('nodejs' )
optdepends=()
source=(http://registry.npmjs.org/$_npmname/-/$_npmname-$_npmver.tgz)
noextract=($_npmname-$_npmver.tgz)
sha1sums=('4f220cf7288a27eaca739df6e4808a2d4c0d5756')

package() {
  cd "$srcdir"
  local _npmdir="$pkgdir/usr/lib/node_modules/"
  mkdir -p "$_npmdir"
  cd "$_npmdir"
  npm install -g --prefix "$pkgdir/usr" $_npmname@$_npmver
}

# vim:set ts=2 sw=2 et:
