# Maintainer: VHSgunzo <vhsgunzo.github.io>

pkgname='runimage-chisel'
pkgver='1.10.1'
pkgrel='1'
pkgdesc='Patched chisel for RunImage container'
url='https://github.com/VHSgunzo/chisel'
arch=('x86_64' 'aarch64')
license=('MIT')
options=(!strip)
provides=("chisel=$pkgver-$pkgrel")
depends=('runimage-static')
source=("chisel-${CARCH}::$url/releases/download/v$pkgver/chisel-linux-${CARCH}")
sha256sums=('SKIP')

package() {
  install -Dm755 "chisel-${CARCH}" "${pkgdir}/var/RunDir/sharun/bin/chisel"
}
