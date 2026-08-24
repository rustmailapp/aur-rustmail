# Maintainer: RustMail <hello@rustmail.app>
pkgname=rustmail-bin
pkgver=0.6.0
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

sha256sums_x86_64=('5847c54840914aa967ac4e9882f4d2c625887eaf1915b439a60260d578ace59e')
sha256sums_aarch64=('617d606214bb8474709f7db415de3feab5c202350020a39a0e738e2ea5332f3b')

package() {
  install -Dm755 rustmail "${pkgdir}/usr/bin/rustmail"
}
