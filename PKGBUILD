pkgname=gdl-look-and-feel
pkgver=1.0
pkgrel=1
pkgdesc="Set of default settings for Project GDL"
arch=('any')
url="https://github.com/GMDProjectL/gdl-look-and-feel"
license=('MIT')
depends=()
makedepends=()
checkdepends=()
optdepends=()
backup=()
options=()
install=
source=(${pkgname}::"git+file://${PWD}")
md5sums=('SKIP')

package() {
    cd "$srcdir/$pkgname"

    local DEFAULT_XDG_DIST="${pkgdir}/etc/xdg"

    mkdir -p "${DEFAULT_XDG_DIST}"

    install -Dm755 etc/xdg/kdeglobals "${DEFAULT_XDG_DIST}/kdeglobals"
}
