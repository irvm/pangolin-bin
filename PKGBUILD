# Maintainer: vbopk9x3 <vbopk9x3@4wrd.cc>
pkgname=pangolin-bin
pkgver=0.6.1
pkgrel=1
pkgdesc="Pangolin Client - Secure reverse proxy and tunnel (Binary version)"
arch=('x86_64' 'aarch64' 'armv7h' 'armv6h' 'riscv64')
url="https://github.com/fosrl/cli"
license=('AGPL-3.0-or-later')
provides=('pangolin')
conflicts=('pangolin')
install=pangolin-bin.install

source_x86_64=("pangolin::https://github.com/fosrl/cli/releases/download/${pkgver}/pangolin-cli_linux_amd64")
source_aarch64=("pangolin::https://github.com/fosrl/cli/releases/download/${pkgver}/pangolin-cli_linux_arm64")
source_armv7h=("pangolin::https://github.com/fosrl/cli/releases/download/${pkgver}/pangolin-cli_linux_arm32")
source_armv6h=("pangolin::https://github.com/fosrl/cli/releases/download/${pkgver}/pangolin-cli_linux_arm32v6")
source_riscv64=("pangolin::https://github.com/fosrl/cli/releases/download/${pkgver}/pangolin-cli_linux_riscv64")

# SHA256 Checksums (Generate these using 'updpkgsums')
sha256sums_x86_64=('50288001e7f62689abe634b281b6f7a2d1a04f2455b66d7536439b2e57164617')
sha256sums_aarch64=('1107d8ec149c53ea107501c200891ef2344b85267c807155a59efa222a0ed1f3')
sha256sums_armv7h=('869ef9fd077a12b5a61f0225a69b44c3f97a0be7510ee3e6e52883866b897ca5')
sha256sums_armv6h=('872159f8e7add5969a983df793818157c9378b434f2a996f619db257121291a3')
sha256sums_riscv64=('4fbddea1a10b8a1b0967881174cf9b9a16f68abde024dba7ad4d307b118a05cb')

package() {
    # Install the binary to /usr/bin and set executable permissions
    install -Dm755 "${srcdir}/pangolin" "${pkgdir}/usr/bin/pangolin"
}
