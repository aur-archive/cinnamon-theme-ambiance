# Contributor: gareth_c
# Maintainer: Ner0

pkgname=cinnamon-theme-ambiance
pkgver=2.5
pkgrel=1
pkgdesc="A stylish dark grey theme distantly related to the Ambiance gtk theme."
arch=('any')
url="http://cinnamon-spices.linuxmint.com/themes/view/43"
license=('GPL')
depends=('cinnamon')
source=("http://cinnamon-spices.linuxmint.com/uploads/themes/8S61-DD6J-4SPQ.zip")
md5sums=('9c547ad7e57901392e4fcd433c629c31')

package() {
  cd ambiancethemes/
  for i in Ambiance*; do
    find "$i" -type f -not -name *~ -exec install -Dm644 '{}' "$pkgdir/usr/share/themes/{}" \;
  done
}
