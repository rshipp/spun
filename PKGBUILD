# Maintainer: george <rpubaddr0 {at} gmail [dot] com>

pkgname=spun-git
_pkgname=spun
pkgver=20120516
pkgrel=1
pkgdesc='A simple pacman update notifier, using notify-send.'
arch=('any')
url='http://github.com/george2/spun/'
screenshot='http://github.com/george2/spun/raw/master/spun.png'
license=('none')
conflicts=('spun' 'spun-live')
depends=('libnotify' 'bash')
optdepends=('kde-baseapps: for the kdialog gui')

_gitname="${_pkgname}"
_gitroot="git://github.com/george2/${_gitname}.git"
_locales=( ca de el es fr it nl_BE nl_NL pl pt_BR )


build() {
  cd "${srcdir}"
  msg "Connecting to GIT server...."

  if [ -d $_gitname ] ; then
    cd $_gitname && git pull origin
    msg "The local files are updated."
    cd ..
  else
    git clone $_gitroot $_gitname
  fi

  msg "GIT checkout done or server timeout"
}

package() {
  cd "${srcdir}/${_pkgname}"
  install -Dm755 spun "${pkgdir}/usr/bin/spun"
  install -Dm644 spun.conf "${pkgdir}/etc/spun.conf"
  install -Dm755 spun.desktop "${pkgdir}/usr/share/autostart/spun.desktop"

  # localization
  for lc in ${_locales[@]}; do
    install -dm755 "${pkgdir}/usr/share/locale/$lc/LC_MESSAGES/"
    msgfmt -o "${pkgdir}/usr/share/locale/$lc/LC_MESSAGES/spun.mo" \
      "lang/$lc.po"
  done
}
