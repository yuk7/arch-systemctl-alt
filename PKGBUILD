# Maintainer:  yuk7 <yukx00@gmail.com>

pkgname=systemd-altctl
_pkgname=systemd
pkgver=1.4.4181
pkgrel=1
_pkgver=219.0
_pkgrel=1
pkgdesc='systemd systemctl alternative package'
arch=('any')
license=('EUPL')
url="https://github.com/gdraheim/docker-systemctl-replacement"
groups=('base')
depends=('python' 'systemd-libs')
provides=("${_pkgname}=${_pkgver}-${_pkgrel}")
conflicts=("${_pkgname}")
source=(systemctl.py)
md5sums=('0002faf35c345348f0d0a8ad328d86f1')

package() {
  install -Dm755 systemctl.py "$pkgdir"/usr/bin/systemctl
}
