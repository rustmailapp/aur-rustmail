# Maintainer: Davide Tacchini <info@rustmail.app>
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

sha256sums_x86_64=('4184bf22cede1e534774a4906d26c2ba4f2959ba09d5ed1a0a7d3e2572f6444f')
sha256sums_aarch64=('bc813033b114c18c16e73a148d4d4d3c7c024d6c924d9d0acf132ea0aee338b6')

package() {
  install -Dm755 rustmail "${pkgdir}/usr/bin/rustmail"
}
