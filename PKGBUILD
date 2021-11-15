# Maintainer:
pkgname=fbpos-wallpapers
pkgver=22
pkgrel=1
epoch=
pkgdesc="FBP Wallpapers for FBP OS."
arch=('x86_64')
url="https://github.com/FilmaBem2/fbpos-wallpapers-imgs.git"
license=('MIT')
groups=()
depends=()
makedepends=(git)
checkdepends=()
optdepends=()
provides=(fbpos-wallpapers)
conflicts=()
replaces=()
backup=()
options=()
install=${pkgname}.install
changelog=
source=("git+$url")
noextract=()
md5sums=('SKIP')
validpgpkeys=()

pkgver() {
	cd "${_pkgname}"
    printf "22" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
    cd fbpos-wallpapers
    install -Dm644 *.jpg "${pkgdir}/usr/share/wallpapers/fbpos/"
}
