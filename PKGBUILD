# Maintainer: RustMail <hello@rustmail.app>
pkgname=rustmail-bin
pkgver=0.10.0
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

sha256sums_x86_64=('877a1bf1c9321a2ca7df4f18a8a226549093b3291b29793b56d343b930ccb305')
sha256sums_aarch64=('c92ea7ef09e1ff02309d45da8f3e75f7307e1bee57333ead43e238ee78d79d2b')

package() {
  install -Dm755 rustmail "${pkgdir}/usr/bin/rustmail"
}
