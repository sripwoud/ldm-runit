# Maintainer: sripwoud <me@sripwoud.xyz>
_pkgname=ldm
pkgname=${_pkgname}-runit
pkgver=1.0
pkgrel=1
pkgdesc="Custom ${_pkgname} runit service"
arch=('any')
url="https://github.com/sripwoud/${_pkgname}-runit"
license=('AGPL-3.0-only')
depends=('runit')
source=("run" "run.asc")
validpgpkeys=('D99B40AC0CE81A5FF8B8456F6296216946C1B36A')
sha256sums=('21f2517ae0bb4b9ec1a470727713fcbb5ef1f676a8409a644bdbadaf0e949e90' 'SKIP')
install=run.install

package() {
    install -Dm755 "${srcdir}/run" "${pkgdir}/etc/runit/sv/${_pkgname}/run"
}
