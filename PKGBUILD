pkgname=2gis-vladimir
pkgver=18
pkgrel=1
pkgdesc="Map of Vladimir for 2GIS, August 2013"
arch=('i686' 'x86_64')
url="http://vladimir.2gis.ru/how-get/linux/"
license=('custom')
depends=('2gis>=3.13.5.1')
source=("http://download.2gis.ru/arhives/2GISData_Vladimir-18.orig.zip")
md5sums=('81a34b186ba0b1fb415cb1987046e68b')

package() {
  install -D -m 644 "${srcdir}/2gis/3.0/Data_Vladimir.dgdat" "${pkgdir}/opt/2gis/vladimir.dgdat" || return 1
  install -D -m 644 "${srcdir}/2gis/3.0/Plugins/DGisLan/Vladimir.dglf" "${pkgdir}/opt/2gis/Plugins/DGisLan/vladimir.dglf" || return 1
}
