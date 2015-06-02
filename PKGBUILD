# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Your Name <noah.harvey247@gmail.com>
pkgname=texlive-custom
pkgver=0.0.1
pkgrel=1
epoch=
pkgdesc="custom latex package for labreports"
arch=('any')
url="file:///home/noah/src/com/$pkgname/"
license=('GPL')
groups=()
depends=(texlive-core)
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=("$url/$pkgname-$pkgver.tar.gz")
noextract=()
md5sums=('964fccf17d9bfc2f3f704c7bd7a8187c')
validpgpkeys=()

INSTALL_DIR="/usr/share/texmf/tex/latex/labreport"

package() {
	cd "$pkgname-$pkgver"
	mkdir -p "$INSTALL_DIR"
	cp labreport.sty "$INSTALL_DIR"
}
