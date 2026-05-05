# Maintainer: RustMail <hello@rustmail.app>
pkgname=rustmail-bin
pkgver=0.3.1
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

sha256sums_x86_64=('438a1c1b353604f3e73abc7d37c6e73a48ead3c2e098d95cf8a8c229042f51cb')
sha256sums_aarch64=('592c4274a72e13152d45d8d6487cc2ab500069ee28822233e65837752c6162d6')

package() {
  install -Dm755 rustmail "${pkgdir}/usr/bin/rustmail"
}
