# Author: ~0rAX0 <http://0rax0.deviantart.com/>
# Maintainer: DaimyoKirby <davidsonalden+aur at gmail dot com>

pkgname=gnome-shell-theme-nord
pkgver=1.8
pkgrel=1
pkgdesc="A GNOME Shell theme with a glassy transparent look."
url="http://0rax0.deviantart.com/art/Nord-Gnome-shell-214295138"
license=('cc-by-nc-sa-3.0')
arch=('any')
depends=('gnome-shell' 'wget')
optdepends=('gnome-tweak-tool: A tool to customize advanced GNOME 3 options.')
source=("http://fc04.deviantart.net/fs71/f/2013/167/a/d/gnome_shell__nord_by_0rax0-d3jl36q.zip")
DLAGENTS=('http::/usr/bin/wget -c -t 3 --waitretry=3 -H -U Mozilla -O %o %u')


package() {
  mkdir -p "${pkgdir}/usr/share/themes/"
  cp -r "${srcdir}/Nord" "${pkgdir}/usr/share/themes/"

  mkdir -p "${pkgdir}/usr/share/licenses/gnome-shell-theme-nord"
  mv "${pkgdir}/usr/share/themes/Nord/gnome-shell/COPYING" \
    "${pkgdir}/usr/share/licenses/gnome-shell-theme-nord/"
}

md5sums=('f1ed5b291b69fb7d207213acbe4efccf')
