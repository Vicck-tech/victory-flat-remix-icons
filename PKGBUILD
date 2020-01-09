# Maintainer: vicck-tech
pkgname=victory-flat-remix-icons-git
_pkgname=victory-flat-remix-icons
_destname="~/.icons"
_licensedir="/usr/share/arcolinux/licenses/"
pkgver=1.0.1
pkgrel=1
pkgdesc="Icons for Arcolinux-Victory Edition"
arch=('any')
url="https://github.com/Vicck-tech/victory-repo/x86_64/${_pkgname}"
license=('GPL3')
makedepends=('git')
depends=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${_pkgname}::"git+https://github.com/Vicck-tech/victory-repo/x86_64/${pkgname}")
sha256sums=('SKIP')
package() {
	mkdir -p "${pkgdir}${_licensedir}${_pkgname}"
	mv "${srcdir}/${_pkgname}/"LICENSE "${pkgdir}${_licensedir}${_pkgname}/LICENSE"
	mkdir -p "${pkgdir}${_destname}"
	cp -r "${srcdir}/${_pkgname}/calamares/"* "${pkgdir}${_destname}"
}