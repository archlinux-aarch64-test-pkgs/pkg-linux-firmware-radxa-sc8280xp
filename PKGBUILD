pkgname=linux-firmware-radxa-sc8280xp
pkgver=0.r4.gf1d257f
pkgrel=1
pkgdesc="Firmware files for Radxa SC8280XP devices"
arch=('any')
url="https://github.com/strongtz/linux-firmware-radxa-sc8280xp"
license=('unknown')
makedepends=('git')
options=('!strip' '!debug')
source=("${pkgname}::git+${url}.git#commit=f1d257f462115ef6918207f38d02af91cc825802")
sha256sums=('SKIP')

package() {
  cd "$pkgname"

  install -dm755 "$pkgdir/usr/lib/firmware"
  cp -a firmware/. "$pkgdir/usr/lib/firmware/"
}
