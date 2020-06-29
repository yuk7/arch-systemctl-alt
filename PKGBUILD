# Maintainer:  yuk7 <yukx00@gmail.com>

pkgname=systemd-altctl
_pkgname=systemd
pkgver=1.4.4181
pkgrel=2
_pkgver=219.0
_pkgrel=1
pkgdesc='systemd systemctl alternative package'
arch=('any')
license=('EUPL')
url="https://github.com/gdraheim/docker-systemctl-replacement"
groups=('base')
depends=('python' 'systemd-libs')
provides=("${_pkgname}=${_pkgver}-${_pkgrel}" "systemd-tools=${_pkgver}" "udev=${_pkgver}")
conflicts=("${_pkgname}")
source=(systemctl.py)
md5sums=('8eee6334850a44ae051fb1cf32d93f45')

package() {
  install -Dm755 systemctl.py "$pkgdir"/usr/bin/systemctl
}
