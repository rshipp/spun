# Maintainer: george <rpubaddr0 {at} gmail [dot] com>

pkgname=spun
pkgver=0.1
pkgrel=1
pkgdesc='A simple pacman update notifier, using notify-send.'
arch=('any')
url='http://github.com/george2/spun/'
license=('none')
depends=('libnotify' 'bash' 'kde-baseapps')
install=$pkgname.install
source=('spun')
md5sums=('a1129cc83f52c182ce69356d138b0ceb')

package() {
  install -Dm755 spun "${pkgdir}/usr/bin/spun"
}
