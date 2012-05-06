# Maintainer: george <rpubaddr0 {at} gmail [dot] com>

pkgname=
pkgver=
pkgrel=1
pkgdesc=''
arch=('i686' 'x86_64')
url=''
license=('')
depends=()
makedepends=()
optdepends=()
conflicts=()
source=("${pkgname}-${pkgver}.tar.gz")
sha256sums=('')

build() {
  cd "${pkgname}-${pkgver}"
  ./configure --prefix=/usr
  make
}

package() {
  cd "/${pkgname}-${pkgver}"
  make DESTDIR="${pkgdir}" install
}
