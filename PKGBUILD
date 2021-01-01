# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Bangduo Chen <1413563527@qq.com>
pkgname=HillstoneVPN
pkgver=1.0.0
pkgrel=1
epoch=
pkgdesc="The Hillstone Secure Connect VPN client for Linux. "
arch=(x86_64)
url="http://docs.hillstonenet.com/en/Content/7_VPN/SSL_VPN_Client_L.htm#"
license=('unknown')
groups=()
depends=()
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
source=("https://github.com/JackMoriarty/HillstoneVPN/releases/download/v1.0.0/$pkgname-$pkgver.tar.gz")
noextract=()
md5sums=('bb0301e31bdaf7c6bcbafae8e74cd3d6')
validpgpkeys=()

package() {
	tar -zxvf "$pkgname-$pkgver.tar.gz" -C "${srcdir}"
	
	install -d "${pkgdir}/opt"
	cp -r "${srcdir}/$pkgname" "${pkgdir}/opt"
	
	install -d "${pkgdir}/usr/share/applications"
	install -Dm755 "${srcdir}/$pkgname/HillstoneVPN.desktop" "${pkgdir}/usr/share/applications"
}
