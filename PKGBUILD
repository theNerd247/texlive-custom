# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Your Name <noah.harvey247@gmail.com>
pkgname=texlive-custom
pkgver=0.0.2
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
source=()
noextract=()
md5sums=()
validpgpkeys=()

_gitroot="$url.git"
_gitname=$pkgname

build() 
{
  cd "$srcdir"
  msg "Connecting to GIT server...."

  if [[ -d "$_gitname" ]]; then
    cd "$_gitname" && git pull origin
    msg "The local files are updated."
  else
    git clone "$_gitroot" "$_gitname"
  fi

	git checkout "v$pkgver"

  msg "GIT checkout done or server timeout"
}

package() {
	INSTALL_DIR="$pkgdir/usr/share/texmf/tex/latex/custom"
	cd "$srcdir/$_gitname"
	mkdir -p "$INSTALL_DIR"
	cp -r pkgs/* "$INSTALL_DIR"
}
