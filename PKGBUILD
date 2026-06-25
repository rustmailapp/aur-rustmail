# Maintainer: RustMail <hello@rustmail.app>
pkgname=rustmail-bin
pkgver=0.5.0
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

sha256sums_x86_64=('3aed9708f863eb21ac289edb86633d9700e774cf87f28bf219e0b3f6248cc42c')
sha256sums_aarch64=('113d863484a751ac6846970ee10dcd5640e125a1e8d15f59e453e9007628d875')

package() {
  install -Dm755 rustmail "${pkgdir}/usr/bin/rustmail"
}
