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
url="https://github.com/theNerd247/texlive-custom"
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
source=("$url/archive/v0.0.1.tar.gz")
noextract=()
md5sums=('777c760bef67a06552023660aa6e867c')
validpgpkeys=()


package() {
	INSTALL_DIR="$pkgdir/usr/share/texmf/tex/latex/custom"
	cd "$pkgname-$pkgver"
	mkdir -p "$INSTALL_DIR"
	cp labreport.sty "$INSTALL_DIR"
}
