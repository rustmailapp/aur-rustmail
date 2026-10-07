# Maintainer: RustMail <hello@rustmail.app>
pkgname=rustmail-bin
pkgver=0.9.0
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

sha256sums_x86_64=('821971309a48419c55bfe9a58ce54940d030d19f373b1e01a4febc8e06e8c7f9')
sha256sums_aarch64=('d5c6e7fd90e37d41592a98aab616cb959b60b2caf0d3e617e7f8735b0b4038ea')

package() {
  install -Dm755 rustmail "${pkgdir}/usr/bin/rustmail"
}
