# Maintainer: RustMail <hello@rustmail.app>
pkgname=rustmail-bin
pkgver=0.4.0
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

sha256sums_x86_64=('c92789a5be020dc97ce9b8c4db053119218534c430c38f2cf1c8b85f4100f3cf')
sha256sums_aarch64=('606c19a31ec2315653801625b3703ab2ee5c75c8a43bcc0dfb890f23deff6a9f')

package() {
  install -Dm755 rustmail "${pkgdir}/usr/bin/rustmail"
}
