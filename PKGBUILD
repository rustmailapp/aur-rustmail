# Maintainer: RustMail <hello@rustmail.app>
pkgname=rustmail-bin
pkgver=0.3.0
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

sha256sums_x86_64=('6c34eda2143aeacfdb29ba66659d4c7ba0960421c68024ef4623be0faab496ef')
sha256sums_aarch64=('c974eb8ead99b8a393172d3736ae8d1b1998f1d7e83843fb8ab400ab7af77296')

package() {
  install -Dm755 rustmail "${pkgdir}/usr/bin/rustmail"
}
