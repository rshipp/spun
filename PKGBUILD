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
md5sums=('c175a69f6b4729d9ac60209c2ee270ac')

package() {
  install -Dm755 spun "${pkgdir}/usr/bin/spun"
}
