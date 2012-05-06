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
md5sums=('569cfb1239ddb18bcca4a4f0057aae43')

package() {
  install -Dm755 spun "${pkgdir}/usr/bin/spun"
}
