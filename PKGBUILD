# Maintainer: SuperBo <supernbo at gmail dot com>
# Contributor: Berseker <berseker86 at gmail dot com
# Based on PKGBUILD by facundes <felipe.facundes at gmail dot com>

pkgname=ubudao-icon-theme
pkgver=1.4.5
pkgrel=2
pkgdesc="ubudao is a colorful icon set compatible with most light GTK themes."
arch=('any')
makedepends=('tar' 'xorg-server')
optdepends=('gnome-icon-theme: GNOME icon theme')
url="http://kde-look.org/content/show.php/Ubudao+Style?content=159086"
license=('GPL')
source=(
https://www.dropbox.com/s/00kdhe421i3wh5a/ubudao-style_1.4.5.tar.gz)

build()
{
 cd "$srcdir"
 install -d 755 "${pkgdir}/usr/share/icons/"
 chmod -R 755 ubudao-style
 cp -rf ubudao-style "${pkgdir}/usr/share/icons/" || return 1
 find -type f -print0 | xargs -0 chmod 644
}

md5sums=('0e90082dd686fa3b94a036d7134cfb49')
