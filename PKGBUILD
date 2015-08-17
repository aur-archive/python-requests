# Maintainer: Patrice Peterson <runiq at archlinux dot us>
# Contributor: Wieland Hoffmann <the_mineo@web.de>

pkgname=python-requests
pkgver=0.14.1
pkgrel=2
pkgdesc="Python HTTP for Humans, Python 3 version."
url="http://python-requests.org"
depends=('python' 'python-chardet')
makedepends=('python-distribute')
license=('custom: ISC')
arch=('any')
source=("http://pypi.python.org/packages/source/r/requests/requests-$pkgver.tar.gz")
md5sums=('3de30600072cbc7214ae342d1d08aa46')

package() {
    cd "${srcdir}/requests-${pkgver}"
    python setup.py install --root=${pkgdir}/
    install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}

# vim:set ts=2 sw=2 et:
