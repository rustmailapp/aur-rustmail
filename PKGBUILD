# Maintainer: RustMail <hello@rustmail.app>
pkgname=rustmail-bin
pkgver=0.8.1
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

sha256sums_x86_64=('682a5d9e15d20119aa6491043b7adfcad81d9ca8563987ecd2ac51940856c21f')
sha256sums_aarch64=('8bf6bce6e150b3aafad4cbd1ec56f2b12b8bed6b0123a442e26ef19dd15e3938')

package() {
  install -Dm755 rustmail "${pkgdir}/usr/bin/rustmail"
}
