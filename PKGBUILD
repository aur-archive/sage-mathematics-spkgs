# $Id: PKGBUILD 64234 2012-02-11 00:28:07Z arodseth $
# Maintainer: Thomas Dziedzic < gostrc at gmail >

pkgname=sage-mathematics-spkgs
pkgver=4.7.2
pkgrel=1
pkgdesc='Open Source Mathematics Software, a viable free alternative to Magma, Maple, Mathematica, and Matlab. Source packages only.'
url='http://www.sagemath.org'
arch=('any')
license=('GPL')
source=("http://sage.math.washington.edu/home/release/sage-${pkgver}/sage-${pkgver}.tar")
md5sums=('b3073997e6c7ec00a269f84ff2e54973')

package() {
  for i in base standard ; do
    install -d ${pkgdir}/opt/sage/spkg/${i}
    install -m644 ${srcdir}/sage-${pkgver}/spkg/${i}/*spkg \
      ${pkgdir}/opt/sage/spkg/${i}
  done
}
