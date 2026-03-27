# Maintainer: RustMail <hello@rustmail.app>
pkgname=rustmail-bin
pkgver=0.1.2
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

sha256sums_x86_64=('SKIP')
sha256sums_aarch64=('SKIP')

package() {
  install -Dm755 rustmail "${pkgdir}/usr/bin/rustmail"
}
