# created 21:30:28 - 10/01/10
# Maintainer: Frikilinux <frikilinux at frikilinux.com.ar>
# Contributor: Adria Arrufat <swiftscythe@gmail.com>

pkgname=kdeplasma-addons-applets-mpd-plasma
pkgver=0.3.3
pkgrel=1
pkgdesc="Plasma MPD client to display and control playback"
url="http://code.google.com/p/mpdplasma/"
license=('APACHE')
arch=('any')
depends=('kdebase-workspace' 'kdebindings-python2' 'python-mpd')
makedepends=()

source=("http://mpdplasma.googlecode.com/files/mpd-plasma-${pkgver}.plasmoid")
md5sums=('84e378894ad446952382d794e8162ee5')

build() {
  cd $srcdir

  install -dm755 ${pkgdir}/usr/share/apps/plasma/plasmoids/mpd-plasma || return 1
  cp -R {contents,metadata.desktop} ${pkgdir}/usr/share/apps/plasma/plasmoids/mpd-plasma/ || return 1
  install -Dm644 metadata.desktop ${pkgdir}/usr/share/kde4/services/plasma-applet-mpd-plasma.desktop || return 1
  
}
