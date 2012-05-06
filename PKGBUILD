# Maintainer: george <rpubaddr0 {at} gmail [dot] com>

pkgname=spun
pkgver=0.1
pkgrel=2
pkgdesc='A simple pacman update notifier, using notify-send.'
arch=('any')
url='http://github.com/george2/spun/'
screenshot='http://i.imgur.com/8eIE0.png'
license=('none')
depends=('libnotify' 'bash' 'kde-baseapps')
install=$pkgname.install
source=('spun')
md5sums=('12b1b8f9e7a04fd91e5f4be2242cc459')

package() {
  install -Dm755 spun "${pkgdir}/usr/bin/spun"
}
