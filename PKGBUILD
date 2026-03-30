# Maintainer: RustMail <hello@rustmail.app>
pkgname=rustmail-bin
pkgver=0.2.0
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

sha256sums_x86_64=('c5bd203e15217e6cb4fb27be97986939408d63426f09aae7e0bc93f555ecc5d4')
sha256sums_aarch64=('cdfcea62d540d090e8ed4d59e46ffe1eedb29bc8db7b479f27a39e333b810428')

package() {
  install -Dm755 rustmail "${pkgdir}/usr/bin/rustmail"
}
