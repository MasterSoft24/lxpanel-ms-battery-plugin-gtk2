# Maintainer and Contributor: Vladimir Kamensky   <mastersoft24@yandex.ru>


pkgname=lxpanel-ms-battery-plugin-gtk2
pkgver=0.9.3
pkgrel=1
pkgdesc="Modern graphical battery state monitor, LxPanel plugin"
arch=('i686' 'x86_64')
url="https://github.com/MasterSoft24/lxpanel-ms-battery-plugin-gtk2"
license=('GPL2')
#categories=('network')
#replaces=('grive2')
#conflicts=('grive2')


depends=( 'gtk2>=2.20.0' 'cairo' 'lxpanel>=0.5.8')
makedepends=( 'intltool')
options=(!emptydirs)


source=("https://github.com/MasterSoft24/lxpanel-ms-battery-plugin-gtk2/archive/master.tar.gz" 
	"lxpanel-master.tar.bz::https://git.lxde.org/gitweb/?p=debian/lxpanel.git;a=snapshot;h=HEAD;sf=tbz2")

md5sums=('15425e5fa14bcffc6f6fbd1dcb1d8197'
         '4ebedd0eed1cc9d6e28301670a50a08b')


build() {

SD=`ls|grep HEAD`


cp -R "$srcdir/$pkgname-master/plugins" "$srcdir/$SD"
cd "$srcdir/$SD"
./autogen.sh
./configure

patch  < "$srcdir/$pkgname-master/pb-make.patch"


#	cd "$srcdir/cloudcross-v$pkgver-$pkgrel"
	
#	rm -rf build
#	mkdir build
#	cd build
#	qmake .. 
#	make   
}
 
package() {
#	cd "$srcdir/cloudcross-v$pkgver-$pkgrel/build"
	
#	mkdir -p "${pkgdir}/usr/bin"
 #       mkdir -p "${pkgdir}/usr/share/man/man0"
	
#	cp "$srcdir/cloudcross-v$pkgver-$pkgrel/build/ccross" "${pkgdir}/usr/bin"
 #       cp "$srcdir/cloudcross-v$pkgver-$pkgrel/doc/ccross" "${pkgdir}/usr/share/man/man0"
	
	#ln -s "${pkgdir}/usr/bin/ccross" "${pkgdir}/usr/bin/CloudCross" 
	#ln -s "${pkgdir}/usr/bin/ccross" "${pkgdir}/usr/bin/grive2" 
ls
}
