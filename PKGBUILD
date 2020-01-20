# Maintainer: ava1ar <mail(at)ava1ar(dot)me>
# Maintainer: Kewl <xrjy@nygb.rh.bet(rot13)>
# Contributor: Star Brilliant <echo bTEzMjUzQGhvdG1haWwuY29tCg== | base64 -d>
_watch=('https://www.realvnc.com/en/connect/download/vnc/linux/' 'VNC-Server-(\d[\d.]*\d+)-Linux-x64\.deb')

pkgname=realvnc-vnc-server
pkgver=6.7.0
pkgrel=1
pkgdesc='VNC remote desktop server software by RealVNC'
arch=('x86_64' 'i686' 'armv7h' 'armv7' 'armv8' 'aarch64')
url='https://www.realvnc.com/'
license=('custom')
depends=('libsm' 'libxtst' 'xorg-xauth')
optdepends=('cups: Printer support')
install='realvnc-vnc-server.install'
conflicts=('tightvnc' 'tigervnc' 'turbovnc')
source_x86_64=("https://www.realvnc.com/download/file/vnc.files/VNC-Server-${pkgver}-Linux-x64.deb")
source_i686=("https://www.realvnc.com/download/file/vnc.files/VNC-Server-${pkgver}-Linux-x86.deb")
source_armv7=("https://www.realvnc.com/download/file/vnc.files/VNC-Server-${pkgver}-Linux-ARM.deb")
source_armv7h=("https://www.realvnc.com/download/file/vnc.files/VNC-Server-${pkgver}-Linux-ARM.deb")
source_armv8=("https://www.realvnc.com/download/file/vnc.files/VNC-Server-${pkgver}-Linux-ARM.deb")
source_aarch64=("https://www.realvnc.com/download/file/vnc.files/VNC-Server-${pkgver}-Linux-ARM.deb")
md5sums_x86_64=('17b8c91bfb67eb585fca6d20f3b0b924')
md5sums_i686=('2ae140b68109d7d065ab13099e6e53bb')
md5sums_armv7h=('04c53f5eae47fcd663e1a89b02f6e3de')
md5sums_armv7=('04c53f5eae47fcd663e1a89b02f6e3de')
md5sums_armv8=('04c53f5eae47fcd663e1a89b02f6e3de')
md5sums_aarch64=('04c53f5eae47fcd663e1a89b02f6e3de')

package() {
    bsdtar -xv -C "${pkgdir}" -f "${srcdir}/"data.tar.*
    mkdir -p "${pkgdir}/usr/share/licenses/${pkgname}"
    ln -s /usr/share/doc/${pkgname}/copyright "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
