# Maintainer: RustMail <hello@rustmail.app>
pkgname=rustmail-bin
pkgver=0.3.2
pkgrel=1
pkgdesc="Self-hosted SMTP mail catcher with web UI, REST API, and CI assertions"
arch=('x86_64' 'aarch64')
url="https://github.com/rustmailapp/rustmail"
license=('MIT' 'Apache-2.0')
provides=('rustmail')
conflicts=('rustmail')
depends=('glibc')

source_x86_64=("${url}/releases/download/v${pkgver}/rustmail-x86_64-unknown-linux-gnu.tar.gz")
source_aarch64=("${url}/releases/download/v${pkgver}/rustmail-aarch64-unknown-linux-gnu.tar.gz")

sha256sums_x86_64=('e50f1deda3faf2a60603d3d048947fc67be23fffce28359e7181e5a289c0bc81')
sha256sums_aarch64=('d1b9432c847a852baa8025cd72fa026f1bf0b014340594406861c836d7b3a257')

package() {
  install -Dm755 rustmail "${pkgdir}/usr/bin/rustmail"
}
