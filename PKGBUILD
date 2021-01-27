pkgname=opendetex
pkgver=2.8.9
pkgrel=1
pkgdesc='Improved version of Detex - tool for extracting plain text from TeX and LaTeX sources.'
arch=('x86_64')
url='https://github.com/pkubowicz/opendetex'
license=('NCSA')
depends=()
makedepends=('gcc' 'make' 'flex')
source=("https://github.com/pkubowicz/opendetex/releases/download/v${pkgver}/opendetex-${pkgver}.tar.bz2")
noextract=("pandoc-${pkgver}-linux-amd64.tar.gz")
md5sums=('e22646c24cca62f9f7feee4ac68101b8')


package() {
    make
    install -Dm 775 detex ${pkgdir}/usr/bin/detex
    install -D detex.1 ${pkgdir}/usr/local/share/man/man1
}
