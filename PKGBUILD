# Maintainer: Erik Dubois <erik.dubois@gmail.com>
pkgname=cappalinux-calamares-config-zen
_destname1="/etc"
pkgver=24.12
pkgrel=01
pkgdesc="calamares for ALCI"
arch=('any')
url="https://github.com/crystalforceix/arcolinux-calamares-pkgbuild-library"
license=('GPL3')
makedepends=('git')
depends=()
conflicts=('alci-calamares-config' 'alci-calamares-config-pure' 'alci-calamares-config-btrfs' 'alci-calamares-config-dev' 'alci-calamares-config-hardened' 'alci-calamares-config-lts')
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
}
