# Maintainer: danb <danielbusch1992@googlemail.com>

pkgname=makefontpkg
pkgver=20130816
pkgrel=1
pkgdesc="Tool to create packages from TrueType-Fonts"
arch=('x86_64' 'i686')
url="http://github.com/misterdanb/makefontpkg"
license=('Beerware')
depends=('python2' 'makepkg')
makedepends=('git')
options=('!strip' '!emptydirs')
source=('makefontpkg::git://github.com/misterdanb/makefontpkg.git')
md5sums=('SKIP')

package() {
  install -d "$pkgdir/usr/bin"
  cp -dpr --no-preserve=ownership "$srcdir/$pkgname/$pkgname" "$pkgdir/usr/bin/"
  chmod +x "$pkgdir/usr/bin/$pkgname"
}
