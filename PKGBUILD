pkgname=linux-firmware-radxa-sc8280xp
pkgver=0.1
pkgrel=1
pkgdesc="Firmware files for Radxa SC8280XP devices"
arch=('any')
url="https://github.com/strongtz/linux-firmware-radxa-sc8280xp"
license=('unknown')
makedepends=('git')
options=('!strip' '!debug')
source=("${pkgname}::git+${url}.git#branch=main")
sha256sums=('SKIP')

pkgver() {
  cd "$pkgname"
  printf '0.r%s.g%s' "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
  cd "$pkgname"

  install -dm755 "$pkgdir/usr/lib/firmware"
  cp -a firmware/. "$pkgdir/usr/lib/firmware/"
}
