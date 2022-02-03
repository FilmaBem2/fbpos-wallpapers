# Maintainer: Filma Bem <filmabemtv2@gmail.com>
pkgname=fbpos-wallpapers
pkgver=22
pkgrel=1
epoch=
pkgdesc="FBP Wallpapers for FBP OS."
arch=('x86_64')
url="https://github.com/FilmaBem2/fbpos-wallpapers"
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
changelog=
source=(imgs.zip)
noextract=()
md5sums=('SKIP')
validpgpkeys=()

pkgver() {
	cd "${_pkgname}"
    printf "22" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
    cd fbpos-wallpapers
    install -Dm644 imgs/* "${pkgdir}/usr/share/wallpapers/fbpos/"
}
