# Maintainer: RustMail <hello@rustmail.app>
pkgname=rustmail-bin
pkgver=0.2.1
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

sha256sums_x86_64=('bf2323c8508b8b17d332a1313f047ed5fc9f261b85db86871a61aad4abcc12b3')
sha256sums_aarch64=('8bac2f279ef8509e496ee2795eee5d1b4a26c675abb193fe30035f2fd0ccf5d2')

package() {
  install -Dm755 rustmail "${pkgdir}/usr/bin/rustmail"
}
