# Maintainer:  yuk7 <yukx00@gmail.com>

pkgname=systemd-altctl
_pkgname=systemd
pkgver=1.4.3027
pkgrel=1
_pkgver=219.0
_pkgrel=1
pkgdesc='systemd systemctl alternative package'
arch=('i686' 'x86_64' 'armv7h')
license=('EUPL')
url="https://github.com/gdraheim/docker-systemctl-replacement"
groups=('base')
depends=('python' 'systemd-libs')
provides=("${_pkgname}=${_pkgver}-${_pkgrel}")
conflicts=("${_pkgname}")
source=(systemctl.py)
md5sums=('86468c91a6e0d8011e57d3bbbd1a2a1d')

package() {
  install -Dm755 systemctl.py "$pkgdir"/usr/bin/systemctl
}
