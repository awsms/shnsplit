pkgname=shntool-git
pkgver=3.0.10
pkgrel=1
pkgdesc="A multi-purpose WAVE data processing and reporting utility"
arch=('x86_64')
url="http://shnutils.freeshell.org/shntool/"
license=('GPL-2.0-only')
options=(!emptydirs)
depends=('glibc')
optdepends=('mac: support for ape format'
            'flac: support for flac format'
            'wavpack: support for wv format')
source=()
sha256sums=()

build() {
	cd "${startdir}"
	./configure --prefix=/usr
	make
}

package() {
	cd "${startdir}"
	make DESTDIR="${pkgdir}" install
}
