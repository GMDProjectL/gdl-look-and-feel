pkgname=gdl-look-and-feel
pkgver=1.0
pkgrel=2
pkgdesc="Set of default settings for Project GDL"
arch=('any')
url="https://github.com/GMDProjectL/gdl-look-and-feel"
license=('MIT')
depends=('adwaita-fonts')
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
    local SDDM_CD_DIST="${pkgdir}/etc/sddm.conf.d"

    mkdir -p "${DEFAULT_XDG_DIST}"
    mkdir -p "${SDDM_CD_DIST}"

    install -Dm755 etc/xdg/kdeglobals "${DEFAULT_XDG_DIST}/kdeglobals"
    install -Dm755 etc/sddm.conf.d/10-wayland.conf "${SDDM_CD_DIST}/10-wayland.conf"
    install -Dm755 etc/sddm.conf.d/kde_settings.conf "${SDDM_CD_DIST}/kde_settings.conf"
}
