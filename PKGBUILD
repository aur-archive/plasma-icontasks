 # Contributor: sxe <sxxe at gmx dot de>

pkgname=plasma-icontasks
pkgver=0.9.2
pkgrel=1
pkgdesc="Modified version of KDE 4.7 taskbar applet and taskmanager library. "
arch=('i686' 'x86_64')
url="http://kde-apps.org/content/show.php/Icon+Tasks?content=144808"
license=('GPL')
depends=('kdebase-workspace')
makedepends=('gcc' 'cmake' 'automoc4' 'libdbusmenu-qt')
source=("http://kde-apps.org/CONTENT/content-files/144808-${pkgname}-${pkgver}.tar.bz2")

build() {
  cd $srcdir/${pkgname}-${pkgver}
  mkdir build && cd build
  cmake -DCMAKE_INSTALL_PREFIX=/usr ..
  make
  make DESTDIR="$pkgdir/" install
}

md5sums=('b5f2f0163f0a9ca0292ac6afe4c616b8')
